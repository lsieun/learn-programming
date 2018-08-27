# Character sets, encodings, and Unicode

URL: https://www.gammon.com.au/unicode/

character: cultrue
encoding: mapping
bytes: computer

我的目标是想了解：Unicode是否在内存当中用4个字节存储。

## Windows下用记事本查询ASCII码

新建一个文本文档，按住ALT+要查询的码值（注意，这里是十进制），
松开即可显示出对应字符。例如：按住ALT+97,则会显示出'a'。

> 按数字时，如果无效，可以使用小键盘。

code point: 让我想起，一个小数只要足够精确，就可以代表一本书的内容
font: A font is a way of displaying a code point. There are thousands of fonts available for modern computers and printers. 

## Difference Between Carriage Return, Line Feed and End of Line Characters

URL: https://knowledge.ni.com/KnowledgeArticleDetails?id=kA00Z0000019KZDSA2

The **Carriage Return** (CR) character (`0x0D`, `\r`) moves the cursor to the beginning of the **line** without advancing to the **next line**. ... The **Line Feed** (LF) character (`0x0A`, `\n`) moves the cursor down to the **next line** without returning to the beginning of the line.

## big Endian or little Endian

URL: https://serverfault.com/questions/163487/how-to-tell-if-a-linux-system-is-big-endian-or-little-endian

If you are on a fairly recent Linux machine (most anything after 2012) then lscpu now contains this information:

```bash
$ lscpu | grep Endian
Byte Order:            Little Endian
```

This was added to `lscpu` in version 2.19, which is found in Fedora >= 17, CentOS >= 6.0, Ubuntu >= 12.04.

```python
import sys
print(sys.byteorder)
```

```c
#include<endian.h>
#include<stdio.h>

int main(int argc, char *args[])
{
    printf("Byte Order: ");
    if (BYTE_ORDER == LITTLE_ENDIAN)
    {
        printf("little");
    }
    else
    {
        printf("big");
    }
    printf(" endian.\n");
    return 0;
}
```

if you are on a system that does not have `endian.h`:

```c
#include<stdio.h>

int main(int argc, char *args[])
{
    int test = 0;
    char *bytes = (char *) &test;
    *bytes = 0x01;

    printf("Byte Order: ");
    if (test == 1)
    {
        printf("little");
    }
    else
    {
        printf("big");
    }
    printf(" endian.\n");
    return 0;
}
```

## Unicode vs ASCII memory

URL: https://stackoverflow.com/questions/42168303/unicode-vs-ascii-memory

What is the difference between Unicode and ASCII in terms of memory? How much memory does Unicode and ASCII take in memory? I know that in Unicode it depends on the encoding type (UTF-8, UTF-16 etc..). But I need deeper understanding!

In short, ASCII uses 7 bit code points (ie 7 bits uniquely identifies every character) where as Unicode is defined using 21 bit code points. How much memory that uses depends on the way it is encoded in memory (not necessarily the same as the serialisation encoding used to externalise that data in files, typically one of UTF encodings for Unicode).

In practice ASCII is stored as one character per byte in RAM, and it is very rare to see pure ASCII, particularly outside of the USA - it is more common to see ISO8859-1 (an 8 bit encoding that is completely compatible with ASCII, but with other characters that use the extra bit that is available, eg for the £ and ¡ characters needed in some European countries).

Unicode is more complex, and representations vary considerably:

- Java uses 16 bit characters with the idea of a 'surrogate pair' to represent values that are outside the 'basic multilingual plane' (essentially any character added after Unicode 2.0). This is historic; early versions of Unicode used only 16 bits per character.
- In C it may often make sense to use the variable-length UTF-8 encoding as the in-memory representation - char is a byte after all, but with such encoding comes **a small performance hit** when decoding (it makes trying to find the n-th code point more difficult as one has to effectively iterate through the encoded byte array identifying the start of each character).
- It may also make sense to use UTF-32 (formerly known as UCS-4) as this encodes all Unicode codepoints in a 32 bit integer in a similar way to ASCII being stored in an 8 bit integer.

## Unicode and Character Sets

The Absolute Minimum Every Software Developer Absolutely, Positively Must Know About Unicode and Character Sets (No Excuses!)
https://www.joelonsoftware.com/2003/10/08/the-absolute-minimum-every-software-developer-absolutely-positively-must-know-about-unicode-and-character-sets-no-excuses/


