---
layout: default
title: "Start Here"
nav_order: 0
---

# Start Here
{: .no_toc }

Welcome! 👋 This is a prompt library for building **games for learning** in Unity 2D with an AI coding assistant. It's written for classmates who already have some programming experience and want to spend their time on design, not fighting the engine.

## Table of Contents
{: .no_toc .text-delta }

{: .fs-2 }
- TOC
{:toc}

---

## 🎯 Who This Site Is For

This site assumes you:

- Have written code before, in any language (variables, loops, functions, and classes won't be explained here)
- Are interested in **serious games**: games designed so that playing *is* learning
- Want to prototype quickly with AI help, then iterate on your design

Brand new to coding or to Unity? No problem. Start with the free resources in the next section, then come back.

---

## 📚 New to Unity or Coding? Start Here First

Unity's official learning pathways are free and well made. We recommend them over random tutorials, since they stay up to date with the current version of the editor.

<html>
  <div>
<dl>
  <dt><a href="https://learn.unity.com/pathway/unity-essentials">Unity Essentials</a></dt>
  <dd>For everyone new to Unity. A short pathway covering the editor, GameObjects, 2D, audio, and a first taste of scripting. Do this one even if you're an experienced programmer.</dd>
  <dt><a href="https://learn.unity.com/pathway/junior-programmer">Junior Programmer</a></dt>
  <dd>For anyone new to coding. A longer pathway that teaches C# by building small games. Unity recommends finishing Unity Essentials first.</dd>
</dl>
  </div>
</html>

{:.highlight}
You don't need to finish either pathway before using this site. Getting comfortable moving around the editor is enough to get started.

---

## 🤖 What Vibe-Coding in Unity Actually Looks Like

If you've vibe-coded a web app before, Unity will feel different. An AI assistant can write your C# scripts, but it <span class="highlighter">can't click around in the Unity Editor for you</span>. A typical feature takes two kinds of work:

1. **Code:** the AI writes a script, you paste it into a new C# file
2. **Editor setup:** you attach that script to a GameObject, add components (like a `Rigidbody2D` or `Collider2D`), and drag references into slots in the Inspector

Most "it doesn't work!" moments come from step 2, not the code. That's why every prompt on this site asks the AI to give you editor steps alongside its code.

---

## 🧠 Unity for People Who Already Code

Unity has a few habits that surprise experienced programmers. Skim these before you start, and the AI's code will make a lot more sense.

### Composition over inheritance

In Unity, almost everything is a **GameObject** with **Components** attached. Instead of building a deep class hierarchy (`Enemy : Character : Entity`), you snap together small, single-purpose scripts: a `Health` component, a `Mover` component, a `DialogueTrigger` component. A GameObject's behavior is the sum of its parts.

### Scripts are MonoBehaviours

Your scripts usually inherit from `MonoBehaviour`, and Unity calls their methods for you at specific times. You don't write a `main()` loop.

<div class="imp" markdown="block">

The methods you'll see most often, in the order Unity calls them:

```csharp
public class Example : MonoBehaviour
{
    void Awake()       { } // Runs once when the object loads. Set up your own references here.
    void Start()       { } // Runs once before the first frame. Safe to talk to other objects here.
    void Update()      { } // Runs every frame. Use for input and non-physics logic.
    void FixedUpdate() { } // Runs on a fixed timer. Use for physics (Rigidbody2D movement).
}
```
> **NOTE:** Don't write constructors for MonoBehaviours. Unity creates these objects itself, so use `Awake()` or `Start()` for setup instead.

</div>

### The Inspector is your dependency injection

Instead of passing references through constructors, you expose fields in the **Inspector** and drag objects into them in the editor:

```csharp
[SerializeField] private AudioSource correctSound; // shows up as a slot in the Inspector
```

If you forget to fill that slot, you'll get a `NullReferenceException` when you press Play. This is the #1 beginner error in Unity, and it's almost never a code problem. 🙃

### ScriptableObjects keep content out of code

For learning games, this one matters a lot. **ScriptableObjects** let you store data (quiz items, dialogue lines, scenario choices) as asset files you edit in the Inspector. That means you or a teammate can change the *content* of your game without touching the *code*.

---

## 🛠️ Setup Checklist

<div class="task" markdown="block">

- [ ] Install [Unity Hub](https://unity.com/download) and use it to install the latest **LTS** (long-term support) version of the Unity Editor
- [ ] Create a new project using a **2D** template
- [ ] Install [VS Code](https://code.visualstudio.com/) with the **Unity** extension (or use Visual Studio or Rider if you prefer)
- [ ] In Unity, set VS Code as your external script editor: **Edit → Preferences → External Tools** (on Mac: **Unity → Settings → External Tools**)
- [ ] Set up Git for your project (see the warning below for why)

</div>

<div class="warn" markdown="block">

**Use version control before you start vibe-coding.** AI assistants sometimes rewrite more than you asked for. Commit your project with Git before every big change so you can always roll back. Use a Unity-specific `.gitignore` file so you don't commit thousands of auto-generated files.

</div>

---

## 📋 Your Context Block

AI assistants give much better Unity answers when they know your setup. Paste this at the start of every new chat, and edit the brackets to match your project:

```
I'm building a 2D educational game in Unity [version, e.g. Unity 6 LTS].
- I have programming experience but I'm new to Unity.
- I'm using the new Input System package (not the old Input Manager).
- Learning goal of my game: [one sentence].
When you give me code:
- Explain where each script goes and what GameObject it attaches to.
- Include step-by-step Unity Editor setup (components, Inspector fields, tags, layers).
- Use [SerializeField] private fields instead of public fields.
- Keep scripts small and single-purpose.
- Briefly explain any Unity-specific concept I might not know.
```

<div class="task" markdown="block">

Save your filled-in version somewhere handy, like a notes app or a `PROMPTS.md` file in your project. You'll use it constantly. 📌

</div>

<html>
  <details>
    <summary><strong>WHY MENTION THE INPUT SYSTEM?</strong></summary>
    Unity has two ways to read keyboard and mouse input: the older Input Manager (<code>Input.GetKey</code>) and the newer Input System package. Newer projects default to the Input System, but a lot of AI training data uses the old one. If you don't specify, you may get code that throws errors as soon as you press Play.
  </details>
</html>

---

## 🗺️ How to Use This Library

The site is organized around how a learning game actually gets made:

1. **Design for Learning:** align your learning objectives with your game mechanics *before* you build anything. Each page ends with a paired prompt for brainstorming, mapping, or critiquing your concept.
2. **Unity 2D Prompts:** build common learning-game patterns, like branching scenarios, feedback systems, and player data logging
3. **Worked Examples:** follow a full prompt sequence from empty project to playable prototype

Every prompt page follows the same layout, so you always know where to look:

<html>
  <div>
<dl>
  <dt>Goal</dt>
  <dd>What the prompt builds and when to use it</dd>
  <dt>The Prompt</dt>
  <dd>Copy-ready text, with brackets for the parts you customize</dd>
  <dt>What You'll Get Back</dt>
  <dd>What a good AI response looks like</dd>
  <dt>Editor Steps to Expect</dt>
  <dd>The Unity setup you'll need to do yourself</dd>
  <dt>Common Pitfalls</dt>
  <dd>What usually goes wrong, and how to fix it</dd>
  <dt>Variations</dt>
  <dd>Ways to adapt the prompt for different games</dd>
</dl>
  </div>
</html>

{:.highlight}
Found a prompt that worked well for you? Share it! This library is meant to grow with the class. 🌱
