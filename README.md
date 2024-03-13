# my technical perspectives
This is my (Samuel Squire) document of technical perspectives on technical matters.

Should you listen to me?

# precursor + invite

You can email me at sam@samsquire.com If you think there's a critical insight I haven't understood or not aware of please tell me.

# my background

I've been playing with computers since I was 2 years old, such as in Windows mspaint, Commander Keen. I played with Visual Basic 6 when I tried to create an antivirus and created toy game engines in Javascript ([canvaspace](https://github.com/fuz/canvaspace), [JSPKMNe](https://github.com/fuz/jspkmnengine). I became a software consultant, did Java backend and Javascript frontend development and then I worked doing devops type tasks with Terraform and AWS. I do a lot of hobby work in Java, C, Javascript, Python. I enjoy a certain kind of technical detail in programming such as database internals (btrees, query execution), distributed systems, Jepsen, multithreading, multithreaded server architecture design, scalability, parallelism, coroutines, async, programming language design and implementation. **I think of myself as a beginner in every topic since there is so much to learn.** But I prioritise what I learn what I think is interesting, valuable or useful. My most satisfying piece of work is a [simple incomplete JIT compiler](https://github.com/samsquire/compiler). I am particularly interested in elegance of problem and solution representation. I do not try do anything clever but I do try use insight and understanding to make complexity go away. But you can't make all complexity go away.

# my thoughts on technology as it is today

I think the software industry is unevenly distributed. The software industry is a patchwork of solutions of different maturities and complexities and depths. I think some technologies go too deep and we don't go deep enough in places where we should go deeper. I think the problems that people should be working on improving are too boring for people to work on. I feel that once you deploy your preferred Linux virtual machine or Kubernetes cluster, you still have a very large amount of work and Yak shaving to do to and administer a fleet of servers. When you decide to use React and build a frontend, you have a lot of work to do. **There is a lot of unsatisfyingly, unsolved problems in computing**. They all take lots of work to do properly. And if you mention security everything has to be rethought and redesigned and rehardened.

I don't like working on effort that only benefits my own day and is done identically by everybody else. I think the industry is repeatedly solving the same problems everyday and that problems are solved again and again. It's such a waste of everyone's time.

What I've noticed is that technology is kingdoms that are understood by small groups of people. Any given codebase is really well understood by a one person, the person(s) that wrote it. Then when those people stop working on that project, it becomes "complete" and slowly becomes less used. Mozilla Thunderbird or Firefox is an example of this. **The code is sufficiently complicated that you cannot informally work on the software without a large investment in understanding how it works.**

Conways law produces software that reflects the architecture of organisations and relationships between people. **I think it's a miracle that software runs at all.**

I am simultaneously unsatisfied with software of today and amazed by it. Maybe because I do not feel competent in any particular technology.



# my desires for technology

I prefer code that suits my mental model of the problem of expression, of what I want to do to the data or what is on the screen and what I can do with it. So this includes mental ideas such as rotations, associations, traversals of graphs or trees and pipelines. I also enjoy mechanical sympathy. This is one of the ways how my mind works. You could say this is data structure thinking or transformation pipeline thinking.

I want software to be trivially easy to change but it is not. I love the idea of late architecture: we can defer decisions until we really need to do them. And I want something else: **transformative architecture** which I cover later in this document.

# gratitude

I want to say I am grateful for all the development of all the products that I use and I appreciate that software development is actually really difficult to do right.

# Some summaries

|Topic|Comments|
|--|--|
|Microsoft Windows|I grew up on Windows and then used Ubuntu as a desktop but I am back on Windows. Windows generally works fine for me. Windows graphics, audio and network stacks just work. Occasionally my monitor does not wake up the machine and I need to hard reset. Occasionally the monitor flickers on-and-off and I have to power cycle the monitor. Windows automatic update can be annoying because it automatically reboots/restarts but otherwise the computer is fine.|
|Linux|Linux is great. How many people genuinely understand sched.c?|
|XMonad|XMonad is an effective window manager. I used this at work but don't use it at home.|
|DWM|DWM is easy to use and is similar to XMonad - such as its keyboard shortcuts.|
|Tmux|Tmux is helpful to keep processes persisted between SSH sessions and as a general workspace organisation. I change the bindings to ctrl-a rather than ctrl-b|
|The terminal|I am unsatisfied with the Linux terminal. It only affects the machine I am on, not a fleet of servers.|
|Mac|Apple hardware is high quality but I have never wanted to pay for Apple hardware.|

# -4. Does LISP scale for large teams?



# -3. Web framework busywork

Writing endpoints that handle HTTP responses feels like busy work to me.



# -2. Ruby on rails is an example of how we need advanced intermediate representations for programming

it can be used for interoperability and reuseability.

 

# -1. Each technology is its own kingdom

Software reuseability and composeability is difficult if you're integrating stuff that you didn't fully decide. Is the interface API or control flow direction suitable for your use case? What do you need to do to wrap it so it does what you want with the semantics you want it to have?



# 1. Preferring learning new kinds of things over optimisation of existing things I am already using

I am uninterested with neverending tweaking or lots of customisation of existing things. I would change CAPS LOCK to CMD and turn off natural scrolling on Mac. I would be uninterested in something that would only apply to my own machine and not a fleet of servers. I once learned and used DVORAK daily and used vimperator on Firefox. But I no longer. I lost taste for that level of customisation. **The return on investment doesn't exist for me** 

I never became interested in optimising my choice of shell on Mac or Ubuntu. I am satisfied with bash. I do recommend Terminator for Ubuntu though because it splits terminal windows in a useful way. I used it to run 8 tabs of `redis-benchmark`. I would rather spend time learning completely new kinds of things than change my shell or get a mechanical keyboard. I don't see that the value is beyond the friction of changing shells or learning how to type again on a split keyboard. I've heard fish is good and I struggle to see what zsh adds to shells that it is an advantage that means it is worth changing the defaults.

The benefits feel marginal.

# 2. GUIs are good, even for servers

GUIs can talk to servers over administration protocols. Observability is good. Java's JMX was a great idea but I was never exposed to it in the right way. It seems it has languished.

# 3. Browser engines, programming languages and preventing unnecessary effort

We have previously had multiple browser engines (Trident, Opera Presto, Chakra), but unfortunately many have been stopped because it's Too Much Work.

# 3. Flat map loses information

# 4. Programming languages should bundle performant serialization

# 5. Rust and C++ twist your idea into a strange shape due to language interactions

I am frustrated how language features interact - look at Rust and C++. Async, move semantics, borrow checking, lifetimes, traits affect how you design your software because they can only be used in certain ways.



# 6. Kubernetes

# 7. Emacs

# 8. Runtime abstractions

I am thinking of Java's reflection, Object Proxies in Javascript and Java.  

# 9. Types are important but isn't control flow and what the code actually does interesting?

The algebra behind types is extremely useful.

# 10. Facts, Information systems and hardcoding

If you were writing an assembler or compiler, you have opcodes to think about. You need to encode that information somewhere. You want to map rules to the right opcode. But programming language files aren't databases. As a result we get some hardcoded resolution rule or constants, that doesn't have documentation - because the code is the source of truth and the rules, facts and resolution rules are implemented specifically bespoke for every codebase. The facts of a codebase are poorly captured through sourcecode.



# 11. I'm unsatisfied with other's high level systems

# 12. The value of types and attention applied to types: Isn't code structure and control flow just as interesting?

Static typing, in the sense that your IDE detects that your callsite signature matches the declaration of the function is extremely helpful. I understand the value of this.

Data passes through code, as types.

The structure of the code is like the river banks of a stream. The water is the data and the type of water that is flowing through the river banks. But I feel all attention is applied to types.

Types decide control flow based on the compiler's dispatch algorithm.

But code structure helps inform performance.



 # 13. Is everyone working at the wrong level of abstraction?

I don't think the business logic of GUIs should be programmed in C or C++. I can understand the tiling algorithm or anything that touches scenegraphs or graphics programming or rendering to be in these low level languages. But the business logic and creation of the arrangement of behaviour should be in high level languages.

# 14. Is it really better or is it that you understand it fully?

[I read this comment on HN by clusterhacks and I agreed](https://news.ycombinator.com/item?id=37138063). Many times through technical history people have presented better ways of doing things. But not all gained traction.

Maybe it truly is better, but the person advocating it understands it completely and they prefer that approach. 

# 15. "You're holding it wrong"

Some programming languages cannot effectively represent our intent and require contortions for the programming language to accept it. What we want to do is actually really simple or something that has the same effect but the language doesn't let you do it.

* Anything in Rust async is an example of this.

# 16. Exalting ideas

Some people take an idea to its extremes because they think it is good.

# 17. Programming is mostly logistics

# 18. Some solutions don't stick, generating type safe API stubs for example

# 19. The tip of execution management is very important

The tip of execution is my own definition of what is running right now, it is decided by something and how you define it determines how maintainable and flexible your software is. Like a dispatcher. For example, `systemd` is at the tip of execution when your Linux server boots up. Kubernetes is the tip of execution for your Kubernetes cluster. The Erlang virtual machine or the Go language scheduler runtime is the tip of execution for your processes or goroutines.

 # 20. Arrangement busy work

Compilers arrange things into the right location for a function call. Presumably when we wrote in assembly, we would have to arrange data into the registers for our calling convention. RDI, RSI, RDX, RCX, R8, R9 in System V ABI. Or syscalls parameters which libc handles.

People working with REST APIs nowadays are doing the same thing, manually, to talk to networked services.

* Provide security token
* Handle result code. 

# 21. We're working at the wrong layer of abstraction

# 22. Software and infrastructure Architecture is more important than code quality

# 23. Software maintenance

Software is really difficult to get running.

# 24. Complicated semantics

# 25. Organisation complexity

The build procedure or steps to understand file system and interactions of any software and Linux project.

# 26. Complicated fiction

# 27. Type systems should be part of the package manager and test framework

# 28. I am unsatisfied with symbols in LISP

# 29. Every idea in modern computing is applied to the wrong place

See LISP macros, ASTs

parser generators

REST APIs, swagger

type systems















