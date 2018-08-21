# State Machines – Basics of Computer Science

URL: https://blog.markshead.com/869/state-machines-computer-science/

Computer science is what enables programming, but it is possible to do a lot of programming without understanding the computer science concepts underlying the process of computation. This isn’t always a bad thing. When we program we work at a much higher level of abstraction. When we drive a car, we only concern ourselves with two or three pedals, a gearshift, and a steering wheel. You can safely operate a car without having any clear idea of how it works. However, if you want to operate a car at the very limits of its capabilities, you need to know a lot more about automobiles than just the three pedals, gearshift and steering wheel.

> 讲了一个很不错的例子。如果使用一件东西，或许并不需要太多的了解它；但要发挥一件东西的最大极限，那就必须得足够的了解它。

The same is true of programming. Much mundane everyday work that can be accomplished with little or no understanding of computer science. You don’t need to understand computational theory to build a “contact us” form in PHP. However, if you plan to write code that requires serious computation, you are going to need to understand a bit more about how computation works under the hood.

> 编程亦是如此。

The purpose of this article is to provide some fundamental background for computation. 

## Finite State Machine

A finite state machine is a mathematical abstraction used to design algorithms. In simple terms, a state machine will read a series of inputs. When it reads an input it will switch to a different state. Each state specifies which state to switch for a given input. This sounds complicated but it is really quite simple.

> 这里分清三个概念：finite state machine， input 和 state。  

The circles are “states” that the machine can be in. The arrows are the transitions. So if you are in state `s` and read an a you’ll transition to state `q`. If you read a `b`, you’ll stay in state `s`.

> 这里只粘贴了一部分，看不懂可以看原文。后来的认识：finite machine 由state，input，transition三个部分组成。

这(finite state machine)有什么用呢？它可以解决许多问题。一个很简单的例子就是可以判断html代码是否按顺序包含那些标签（html/head/body）。

## Deterministic Finite State Machine

The state machines we’ve looked at so far are all deterministic state machines. From any state there is only one transition for any allowed input. In other words there aren’t two paths leading out of a state when you read the letter `a`. At first this sounds silly to even make this distinction.

> 到目前为止，谈论的都是deterministic state machines。一个input对应一个transition。并没有谈到对于一个input有两个transition。

**The output of a state machine** is its **final state**. It goes through all its processing and then the final state is read and then an action is taken. A state machine doesn’t do anything as it moves from state to state. It processes and then when it gets to the end, the state is read and something external triggers the desired action. This is an important concept when it comes to non-deterministic finite state machines.

> 第一点：state machine的输出称为final state。  
> 第二点：处理完成后，final state会被读取，然后触发action。  
> 第三点：处理过程中，state machine只是进行state之间的切换，并不会做其他的事情。

## Non-deterministic Finite State Machine

Non-deterministic finite state machines are finite state machines where a given input from a particular state can lead to more than one different state. 

> Non-deterministic finite state machines对于同一个输入，在一个state处可以向多个state进行转换。

Do you see the problem? From starting point `s`, we don’t know which path to take. If we read the letter `a`, we don’t know whether to go to the state `q` or `r`. **There are a few ways to solve this problem**. One is by `back tracking`. You simply take all the possible paths and ignore or back out of the ones where you get stuck.

> 遇到的问题是，我们不知道如何往下走。  
> 有许多解决这个问题的方法，其中一个就是使用back tracking。

**The other option** is to **convert the non-deterministic machine into a deterministic machine**. One of the interesting attributes of a non-deterministic machine is that **there exists an algorithm to turn any non-deterministic machine into a deterministic one**. However, it is often much more complicated. 

> 另一种解决方法就是将non-deterministic machine转换成deterministic machine。

## Regular Expression

If you have done any type of programming, you’ve probably encountered regular expressions. Regular expressions and finite state machines are functionally equivalent. Anything you can accept or match with a regular expression can be accepted or matched with a state machine. 

> 这里将regular expressions和finite state machines进行对比，它们有相似性。

Regular expressions and finite state machines also have the same limitations. In particular they both can only match or accept patterns that can be handled with finite memory. 

> 两者有相同的limitation。

## Turing Machines （图灵机）

So how do you recognize non-regular patterns? There is a theoretical device that is similar to a state machine called a Turing Machine. It is similar to a finite state machine that it has a paper strip that it reads, but a Turing Machine can erase and write on the paper tape. 

## Why does this matter?

So whats the point? How is this going to help you? Regardless of their limitations, state machines are a very central concept to computing. In particular, the recognition that **for any non-deterministic state machine you can design, there exists a deterministic state machine that does the same thing**. This is a very key point because it means **you can design your algorithm in whichever way is the easiest to think about. Once you have a proper algorithm, you can convert it into whatever form is most efficient.**

> 第一点：对于任意的non-deterministic state machine，都可以转换成a deterministic state machine  
> 第二点：设计算法时，可以从“易于理解”为切入点，等算法完成后，可以再进行效率的优化。  

A foundation in computer science allows you to take a problem X that you don’t know how to solve and reason, “I don’t know how to solve X, but I do know how to solve Y and I know how to convert a solution for Y into a solution for X. Therefore I now know how to solve X.”

> 解决问题的能力的推广


