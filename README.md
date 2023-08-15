# my technical perspectives
This is my document of technical perspectives on technical matters.

# precursor + invite

These thoughts are just perspectives. They are mine. You should read everything here as if I'm saying "for me" or "from my perspective". If you have the time and you think I don't understand something then I welcome knowledge sharing of your own perspective to help me. If I don't understand the mainstream perspective, maybe you know something that I don't? You can email me at sam@samsquire.com

# my background

I've been playing with computers since I was 2 years old, such as in Windows mspaint back then. I became a software consultant, did Java backend and Javascript frontend development and then I worked doing devops type tasks with Terraform and AWS. I do a lot of hobby work in Java, C, Javascript, Python. I enjoy a certain kind of technical detail in programming such as database internals (btrees, query execution), distributed systems, Jepsen, multithreading, multithreaded server architecture design, scalability, parallelism, coroutines, async, programming language design and implementation. **I think of myself as a beginner in every topic since there is so much to learn.** But I prioritise what I learn what I think is interesting, valuable or useful. My most satisfying piece of work is a [simple incomplete JIT compiler](https://github.com/samsquire/compiler). I am particularly interested in elegance of problem and solution representation. I do not try do anything clever but I do try use insight and understanding to make complexity go away.

# my thoughts on technology as it is today

I think the software industry is unevenly distributed. The software industry is a patchwork of solutions of different maturities and complexities and depths. I think some technologies go too deep and we don't go deep enough in places where we should go deeper. I think the problems that people should be working on improving are too boring for people to work on. I feel that once you deploy your preferred Linux virtual machine or Kubernetes cluster, you still have a very large amount of work and Yak shaving to do to and administer a fleet of servers. **There is a lot of unsatisfyingly, unsolved problems in computing**. They all take lots of work to do properly. And if you mention security everything has to be rethought and redesigned and rehardened.

I don't like working on effort that only benefits my own day and is done identically by everybody else. I think the industry is repeatedly solving the same problems everyday and that problems are solved again and again. It's such a waste of everyone's time.

What I've noticed is that technology is kingdoms that are understood by small groups of people. Any given codebase is really well understood by a one person, the person that wrote it. Then when those people stop working on that project, it becomes "complete" and slowly becomes less used. Mozilla Thunderbird is an example of this. **The code is sufficiently complicated that you cannot informally work on the software without a large investment in understanding how it works.**

Conways law produces software that reflects the architecture of organisations and relationships between people. **I think it's a miracle that software runs at all.**



# my desires for technology

I prefer code that suits my mental model of the problem of expression, of what I want to do to the data or what is on the screen and what I can do with it. So this includes mental ideas such as rotations, associations, traversals of trees. I also enjoy mechanical sympathy. This is one of the ways how my mind works. You could say this is data structure thinking or transformation pipeline thinking.

I want software to be trivially easy to change but it is not. I love the idea of late architecture: we can defer decisions until we really need to do them.

# gratitude

I want to begin by saying I am grateful for all the development of all the products that I use and I appreciate that software development is actually really difficult to do right.

# Some summaries

|Topic|Comments|
|--|--|
|Microsoft Windows|Windows works fine for me. Windows graphics, audio and network stacks just work.|
|Linux||
|XMonad|XMonad is an effective window manager. I used this at work but don't use it at home.|
|DWM|DWM is easy to use and is similar to XMonad.|
|Tmux|Tmux is useful. I change the bindings to ctrl-a rather than ctrl-b|
|The terminal|I am unsatisfied with the Linux terminal.|
|Mac||

# 1. Preferring learning new kinds of things over optimisation of existing things I am already using

I am uninterested with neverending tweaking or lots of customisation of existing things. I would change CAPS LOCK to cmd and turn off natural scrolling on Mac. I would be uninterested in something that would only apply to my own machine and not a fleet of servers. I once learned and used DVORAK daily and used vimperator on Firefox. But I no longer. I lost taste for that level of customisation. The return on investment doesn't exist. 

I never became interested in optimising my choice of shell on Mac or Ubuntu. I am satisfied with bash. I do recommend Terminator for Ubuntu though because it splits terminal windows in a useful way. I used it to run 8 tabs of `redis-benchmark`. I would rather spend time learning completely new kinds of things than change my shell or get a mechanical keyboard. I don't see that the value is beyond the friction of changing shells or learning how to type again on a split keyboard. I've heard fish is good and Istruggle to see what zsh adds to shells that it is an advantage that means it is worth changing the defaults.

# 2. GUIs are good, even for servers

GUIs can talk to servers over administration protocols. Observability is good. Java's JMX was a great idea but I was never exposed to it in the right way.

# 3. Browser engines, programming languages and preventing unnecessary effort

We have previously had multiple browser engines, but unfortunately many have been stopped because it's Too Much Work.

# 3. Flat map loses information

# 4. Programming languages should bundle performant serialization

# 5. Rust and C++ twist your idea into a strange shape due to language interactions

# 6. Kubernetes

# 7. Emacs

# 8. Runtime abstractions

I am thinking of Java's reflection, Object Proxies in Javascript and Java.  

# 9. Types are important but isn't control flow and what the code actually does interesting?

The algebra behind types is extremely useful.

# 10. Facts, Information systems and hardcoding

If you were writing an assembler or compiler, you have opcodes to think about. You need to encode that information somewhere. You want to map rules to the right opcode. But programming language files aren't databases. As a result we get some hardcoded resolution rule or constants, that doesn't have documentation - because the code is the source of truth and the rules, facts and resolution rules are implemented specifically bespoke for every codebase. The facts of a codebase are poorly captured through sourcecode.



# 11. I'm unsatisfied with other's high level systems













