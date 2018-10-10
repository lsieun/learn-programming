# Top 10 Apache License Questions Answered

URL: https://resources.whitesourcesoftware.com/blog-whitesource/top-10-apache-license-questions-answered

![](https://www.whitesourcesoftware.com/wp-content/uploads/2015/08/apache2.jpg)

**The Apache License** is an open source software license released by the Apache Software Foundation (ASF). It’s a popular and widely deployed license backed by a strong community. The Apache License allows you to freely use, modify, and distribute any Apache licensed product. However, while doing so, you’re required to follow the terms of the Apache License.

## 1. What are the Apache License terms & conditions?

The Apache License is a [permissive open source software license](https://en.wikipedia.org/wiki/Permissive_software_licence) — so you can release your modified version of the Apache licensed product **under any license of your choice**.

> A **permissive software license**, sometimes also called **BSD-like** or **BSD-style** license, is a free software license with minimal requirements about how the software can be redistributed. Examples include the MIT License, BSD licenses, Apple Public Source License and the Apache license. As of 2016, **the most popular free software license** is the permissive **MIT license**.

You can freely use, modify, distribute and sell a software licensed under the Apache License without worrying about the use of software: personal, internal or commercial.

> 这里是Apache License关于软件(Software/Code)的限制：可以 use（使用），modify（修改），distribute（分发），sell（售卖）

This license explicitly grants rights to users that can be applied to both copyrights and patents, unlike other permissive licenses that are applicable only to copyrights and not patents. The rights given are perpetual(时限), worldwide(地域范围), irrevocable, but also non-exclusive(非独占) — so you can use the licensed work, and so can anyone else.

> 这里是Apache License关于copyright和patent的限制：没有限制。
> 关于copyright和patent的区别可以参考这里： [Link](copyright-and-patent.md) 

If you redistribute software with any Apache licensed components, you must include a copy of the license, provide a clear Apache License attribution, and add modification notices to all the files that you modify.

> 这里是Apache License提出的要求。

You can choose to release the modified or derived products **under different licenses**, the unmodified parts of the software, however, must retain the Apache License, and you cannot name your modified version in any way that suggests that the final product is endorsed or created by the ASF.

> 这里是Apache License提出的要求。

Additionally, if you want to add a copyright statement about all the modifications that you’ve done to any Apache licensed software; you are free to do so. Since the Apache License doesn’t require you to release the modified code under the same license, you can choose to add specific license terms and conditions that govern how others use, reproduce, or distribute your modified code.

## 2. What is the difference between the versions?

The Apache Group (later named the Apache Software Foundation) released the first version of its license in **1995**, but it’s rare that you’ll come across components that still carry this license.

In **2000**, when Berkeley accepted the argument put to it by the Free Software Foundation and retired their advertising clause from the BSD license and formed the modified BSD license, Apache did likewise and created the Apache License version 1.1.

**Removing the advertising clause** meant that the advertising materials of the derivative works of any Apache licensed product were no longer required to include the Apache License attribution. It became ok to include the attribution in the documentation alone.

In **2004**, the ASF decided to depart from the BSD model a little more radically and produced the **Apache License version 2.0** by **granting patents rights** and defining solid definitions of the concepts it uses to make it more coherent.

## 3. Is the Apache considered copyleft?

**Copyleft licenses** require **the derivative works or modified versions of existing software to be released under the same license**. The Apache License doesn’t have any such requirements. It’s a permissive license. It permits you to release the modified parts of the code under any license of your choice. However, you are required to release all the unmodified parts of the software under the same license (the Apache License).

Additionally, every licensed file must contain any original copyright, patent, trademark, and attribution notices in its redistributed code. Each modified file must also contain a notice about all the changes made to the original file.

## 4. What is the difference between the Apache License 2.0 and the GNU GPL?

The **GNU GPL** is **a copyleft license**. So software that uses any GPL-licensed component has to release its full source code and all rights to modify and distribute the entire code. **The Apache License 2.0** doesn’t impose any such terms. You’re not forced to release your modified version. Besides, you can choose to release your modified version under a different license (however, you’re required to retain the Apache License for the unmodified parts of the code).

## 5. Is the Apache License compatible with the GNU GPL?

**Apache License 2.0** is compatible with **GPLv3**, so you can freely mix the code that’s released under these two licenses. The resulting software, however, must be released under GPLv3.

However, the **Apache License 2.0** in **incompatible** with **GPLv2** due to the restriction that terminates **the grant of patent rights** if the license sues over patent infringement(侵权；侵犯). Previous Apache versions, being heavily based on the BSD license, are compatible.

## 6. What is the difference between Apache License 2.0 and MIT?

MIT is one of the most permissive free software licenses. Basically, you can do whatever you want with a software licensed under the MIT license - just make sure that you add **a copy of the original MIT license** and **copyright notice** to it.

The Apache License is also a permissive license. However, it has stringent(严格的；严厉的) terms when it comes to **modifications**. It requires you to explicitly list out all the modifications that you’ve done in the original software, i.e., you’re required to preserve modification notices. The Apache License also states clearly that you can’t name your product in any way that hints at the product being **endorsed by Apache**. So you can call your product “SuperWonderServer powered by Apache” but not “Apache SuperWonderServer”. The MIT license doesn’t impose any such terms.

**The MIT license** is also gaining popularity with developers due to its short and clear license agreement, in contrast to the Apache license agreement. Although the Apache License is nearly identical in terms of what you can and can't do, it is much more heavily "lawyered" and is significantly more verbose. Heck, the appendix alone, which explains how to apply the license, is longer than the entire MIT license.

## 7. What is the difference between Apache License 2.0 and BSD?

**The BSD license** is another highly permissible license that allows you to modify and redistribute software licensed under the BSD license as you like. Earlier versions of the Apache License were identical to the original (and later the modified) BSD licenses, but Apache License 2.0 sets them apart. The key differences between the two licenses are:

- **Explicit grant of patent rights**: Apache License 2.0 explicitly lays down the grant of patent rights while using, modifying or distributing Apache licensed software; it also lists the circumstances when such grant gets withdrawn.
- **Clear definitions of the used concepts**: Apache License 2.0 explicitly defines all the terms and concepts that it uses. This leaves little scope for ambiguity.
- **Reusable without rewording**: Apache License 2.0 can be easily used by other projects without any rewording in the license document itself.


## 8. How to Use Apache License 2.0 in commercial products?

You can use any Apache License 2.0 licensed software in your commercial products for free. However, you must not name your product in a way that it looks like an endorsement from Apache. You must also not use any of the **Apache marks** (like the multi-colored feather) anywhere in your product or its documentation.

While using Apache licensed software in your commercial product, you’re still required to follow the terms and conditions that the Apache License imposes.

## 9. Can you license your own software under the Apache License?

Yes. The Apache License 2.0 allows you to release your own software under the Apache license.

## 10. Can you sell Apache open source software/code?

Yes. You can sell any Apache licensed software/code.






- Software
    - Use 使用
    - Modify 修改
    - Distribute 分发
    - Sell 售卖
- copyright
- patent

