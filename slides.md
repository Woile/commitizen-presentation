---
title: Commitizen | Automating release cycles
theme: black
revealOptions:
  transition: "convex"
---

# Commitizen

Automating release cycles

[![github logo](./assets/github.png)](https://github.com/commitizen-tools/commitizen)

---

## Agenda

1. History
2. Commands <!-- .element: class="fragment" data-fragment-index="2" -->
3. Automating release cycle <!-- .element: class="fragment" data-fragment-index="3" -->
4. Customizing <!-- .element: class="fragment" data-fragment-index="4" -->

---

## History 📜

Born as a prompt to avoid remembering commit conventions

<small>
conventional commits, work conventions, etc <!-- .element: class="fragment" data-fragment-index="1" -->
</small>

---

## Beginning

- Customizable
- Automatic version inference planned <!-- .element: class="fragment" data-fragment-index="1" -->
- Wait, I can also generate the changelog 🤔 <!-- .element: class="fragment" data-fragment-index="2" -->

---

## Evolution

Built prompt

Built auto bump version <!-- .element: class="fragment" data-fragment-index="1" -->

@Lee-W starting contributing more and more <!-- .element: class="fragment" data-fragment-index="2" -->

@Lee-W created first autochangelog MVP <!-- .element: class="fragment" data-fragment-index="3" -->

I found motivation again and finished the auto-changelog feature <!-- .element: class="fragment" data-fragment-index="4" -->

---

## Commands

> Aim for intuitiveness and sane defaults

----

`cz init`

Assists in the creation of the `toml` file, with some automatic detections.

----

`cz commit` or `cz c`

Assist in the creation of a commit with matching the defined rules.

Defaults: <!-- .element: class="fragment" data-fragment-index="0" -->
[conventional commitis](https://www.conventionalcommits.org/en/v1.0.0/) <!-- .element: class="fragment" data-fragment-index="0" -->

----

`cz changelog`

----

`cz bump --changelog`

----

### And more

`cz ls` ➡️ list installed commit rules

`cz check` ➡️ validate the commit (useful for git hooks)

`cz schema` ➡️ show the schema of the commit rule

`cz example` ➡️ show an example

`cz info` ➡️ explain rationale behind the commit rule

---

## Release workflow

🧑 Merge PR

⬇️ <!-- .element: class="fragment" data-fragment-index="0" -->

🤖 Create changelog and new tag <!-- .element: class="fragment" data-fragment-index="0" -->

⬇️ <!-- .element: class="fragment" data-fragment-index="1" -->

🤖 Push back to your branch <!-- .element: class="fragment" data-fragment-index="1" -->

⬇️ <!-- .element: class="fragment" data-fragment-index="2" -->

🤖 Trigger deploy/release for new tag <!-- .element: class="fragment" data-fragment-index="2" -->

---

## Fear semver no more

---

## MAJOR.MINOR.PATCH

---

## PATCH

---

[conventional_commits]: https://www.conventionalcommits.org/en/v1.0.0/