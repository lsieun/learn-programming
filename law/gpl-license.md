# Top 10 GPL License Questions Answered

URL: https://resources.whitesourcesoftware.com/blog-whitesource/top-10-gpl-license-questions-answered

![](https://www.whitesourcesoftware.com/wp-content/uploads/2015/07/GPL-e1435820834468.jpg)

**GPL** is the acronym for GNU’s **G**eneral **P**ublic **L**icense, and it’s one of the most popular open source licenses. **Richard Stallman** created the GPL to protect the GNU software from being made proprietary. It is a specific implementation of his "copyleft" concept.

## 1. What is copyleft?

**Copyright** is a law that restricts the right to use, modify, and share creative works without the permission of the copyright holder. When an author releases a program under a **copyleft** license, he makes a claim on the copyright of the work and issues a statement that other people have the right to use, modify, and share the work as long as the reciprocity(互惠；互助) obligation is maintained.

This means that **any software that is written based on any GPL component must be released as open source**. The result is that any software that uses any GPL open source component (regardless of its percentage in the entire code) is required to release its full source code and all of the rights to modify and distribute the entire code.

## 2. What are the GPL license terms and conditions?

If you have used a GPL component in your software, then your entire software is considered a ‘work based on’ a GPL and, therefore:

- **You are not allowed to claim patents or copyright on the software**. Moreover, you are obligated to display a copyright notice, disclaimer of warranty, intact GPL notices, and a copy of the GPL.
- You are not allowed to change the license or introduce additional terms and conditions.
- You are under the reciprocity obligation, which means you are obligated to release the source code and all of the rights to modify and distribute the entire code.

## 3. Is GPL enforceable?

GPL is enforceable as it’s essentially a copyright license. The copyright holders of the GPL software can choose to enforce the GPL on the distributed or derivative works of the software.

For example, the FSF holds the copyrights on many pieces of the GNU system, such as the GNU Compiler Collection. As the copyright holder, it can enforce the copyleft requirements of the GNU General Public License (GPL) if copyright infringement occurs on that software.

## 4. Can you sell GPL software/code?

Yes, the GPL license allows users to sell the original as well as the modified software. It may be confusing, but free software is referred to as free in terms of freedom and not in terms of price. As Richard Stallman explains it, **free software means free as in “free speech,” not free as in “free beer.”**

However, if someone buys your program for a fee, GPL gives him/her the liberty to release it to the public, with or without a fee.

## 5. Is GPL safe?

Yes. GPL doesn’t have anything to do with the security of the code. It’s just a license that governs its usage and distribution. In fact, as we argued in previous posts, open source software may sometimes be safer than proprietary software since you have more people checking and fixing problems.

## 6. Does the GPL license require the author to release the modified source code?

GPL requires you to release the modified source code only if you release the modified program. If you’ve modified a program’s source code for personal use, there’s no need to release its source code. However, if you make the modified program available to the public, you will have to make the code public too.


## 7. What is the difference between GPLv2 and GPLv3?

There has always been some confusion regarding what constitutes a ‘work based on’ another work, which in turn triggers the GPL reciprocity obligation. The FSF tried to add more clarity to GPLv3 as to when the reciprocity obligation is triggered. The FSF even wrote a new GPL license, the Affero license, to address a specific confusion referred to as the “ASP loophole”.

In addition, the FSF tried to increase the compatibility of the **GPLv3** with other licenses. To combine two codes into a larger work, both the programs must permit it. If such rights are granted by both the programs' licenses, they are compatible. By making the GPLv3 more compatible, the FSF expanded development options.

The third difference between the two versions is that the GPLv3 was written in an attempt to increase usage worldwide. The language used in GPLv3 to describe the license rights was modified to ensure that international laws will interpret it as the FSF intended, unlike the language used in GPLv2, which is considered very US centric. GPLv3 also allows developers to add local disclaimers, which also helps increasing its usage outside the US.

## 8. Can you mix GPL license with other licenses?

It's often believed that the code covered by the GPL license cannot be mixed with code covered by other open source software licenses. While restrictions exist, it is actually possible under both GPLv2 and GPLv3. The new language used in the GPLv3 establishes this even more clearly. The FSF has stated explicitly that **GPLv3 is compatible with the Apache 2.0 license**. There is, however, an issue with the original BSD license as it imposes a specific requirement that is not in the GPL (the requirement on advertisements of the program).

## 9. What does the LGPL cover?

The **Lesser General Public License** (LGPL) is a more permissive license (weak copyleft). LGPL is used to license free software so that it can be incorporated into both free and proprietary software.

The LGPL and GPL licenses differ with one major exception; with **LGPL** the requirement that **you open up the source code to your own extensions to the software** is removed. You are only obliged to subject your modifications to the original free library to the LGPL. Since the free library is always subject to the LGPL, it must be possible for any user of your software to modify, recompile or replace the free LGPL library and use its modified version with your software.

You are also required to permit (or note prevent) reverse engineering of the work that uses the library in order to enable debugging when the LGPL library is modified replaced with later versions.

Note that the LGPL is compatible with the GPL: you can decide to "upgrade" to GPL and incorporate it in a wholly GPL licensed project if you wish. You can't however go the other way and re-license GPL licensed code as LGPL.

## 10. What does the AGPL cover?

**AGPL** is the **Affero General Public License**, a variation of the GPL that caters to programs that run on a server. If a developer modifies a program released under the GPL, he is expected to release the modified program under the same license, but if this program runs on a server only, the developer is not really releasing it to the rest of the world.

The AGPL covers this case. Under the AGPL, the developer must release the modified version of the program to everyone who uses the service.

