---
description: >-
  My personal, highly opinionated ESLint configuration for use in the roblox-ts
  ecosystem.
---

# 🎨 ESLint Config

{% embed url="https://github.com/christopher-buss/roblox-ts-eslint-config" %}

***

This configuration was originally derived from [Antfu's eslint-config](https://github.com/antfu/eslint-config), but has been modified to support my preferred coding style. Prettier has been preferred over eslint stylistic due to no autofixable line-length limits, a stricter set of rules than the default has been employed, along with native support for the [**eslint-plugin-roblox-ts**](https://github.com/roblox-ts/eslint-plugin-roblox-ts). Notably, numerous rules that are irrelevant to the roblox-ts ecosystem have been disabled.

This configuration reflects my commitment to maintaining clean code. I believe that an entire project should exhibit a cohesive writing style, even if it involes contributions from 100 different programmers. Achieving consistency across codebases necessitates the use of professional tooling. I firmly believe that addressing inconsistencies in a project is best approached by identifying rules capable of easily rectifying any discrepancies (bonus points if it's auto-fixable!).
