# DotNet8-AOT-StartupPerformanceComparison
A quick startup perfomance comparison between .NET 8 AOT and .NET FX 4.8

![WADH](screenshot.png)

### What?

Some .NET Framework 4.8 devs ("*the old farts*" 😉) asked me, if a .NET 8 AOT pre-compiled application can really beat a .NET Framework 4.8 runtime/JIT application, when it comes down to startup speed. Cause of the following benefits a .NET Framework 4.8 runtime/JIT application has:

- less complex PE header evaluation
- NGEN performance boost
- caching (repeated starts)
- hot state of CLR/JIT vs. "handling a typical native executable"
- native executable maybe "might" load a trimmed down framwork into memory when started (like i.e. pre-compiled Python does)
- the love of god (subjective)

Therefore i quickly tested this, since i was curious too.

### How?

By using the most simple shit: A batch script.

### Results?

See screenshot above.

### Notes

This was just a quick test on the Windows Command Prompt. Not multi-billion dollar rocket science analytics by the NASA.

Just keep this in mind.

#### Have fun.
