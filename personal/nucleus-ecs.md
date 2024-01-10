# 🖥 Nucleus (ECS)

A high-performance Entity Component System in TypeScript built for the Roblox ecosystem.

<figure><img src="../.gitbook/assets/logo.png" alt="" width="450"><figcaption><p>ECS logo.</p></figcaption></figure>

{% hint style="info" %}
**Information:** originally developed by me during my time as Aether Interactive as part of [Tina](https://github.com/AetherInteractiveLtd/Tina) (a development framework for experiences on Roblox), but has since been moved and maintained in my own personal repository.
{% endhint %}

{% @github-files/github-code-block %}

Nucleus was based on [WolfECS](https://github.com/EnderShadow8/wolf-ecs); a TypeScript ECS for the web, designed to beat benchmarks, but was not fully-fledged enough to be usable in real-world applications. The transformation process included converting the existing ECS to roblox-ts (not all TS functionality exists in Roblox). Subsequent steps included codebase refinement and comprehensive documentation.

Building upon this foundation, Nucleus saw the incorporation of additional features to enhance its utility, such as component storage, system scheduling, reactive queries, inline events, and more. The result was a more robust and versatile ECS tailored for effective use within the Roblox platform.

***

### Key Skills

TypeScript, Prototyping, Profiling, Designing, Building Usable APIs, Documentation writing.

### Technical Skills

1. Using TypeScript to build a functional and high-performance ECS with an easy-to-use API.
2. Understanding and implementing efficient data structures such as sparse sets (a specialized data structure for representing a set of integers; useful when the universe of possible values is very large but used very sparingly and the set is iterated often or cleared often) for storing entities.
3. Profiling and optimizing for better performance, considering Roblox specific nuances.
4. Writing BDD-style unit tests to help minimise regressions and ensure typical usage was always kept bug-free.
5. Applying algorithmic thinking to design efficient algorithms for various ECS operations, such as entity/component retrieval and iteration.
6. Fully-fledged documentation, examples, and caveats to make the codebase easily understandable and usable for others (and my future self!).

