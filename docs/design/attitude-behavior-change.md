---
layout: notes
title: "Designing for Attitude & Behavior Change"
parent: "Design for Learning"
nav_order: 5
---

# Designing for Attitude & Behavior Change
{: .no_toc }

Some learning games aren't trying to teach a skill. They're trying to shift how players *think or act*: reducing bias, encouraging healthy habits, building empathy. This page covers Kaufman, Flanagan, and Seidman's **Embedded Design** model, which shows why games that announce their message often fail, and what to do instead.

## Table of Contents
{: .no_toc .text-delta }

{: .fs-2 }
- TOC
{:toc}

---

## 🛡️ Why Being Direct Backfires

Most persuasive games present their message in a direct, matter-of-fact way, assuming players will take it in and carry it into real life. Drawing on social psychology, the authors argue this is "ill-advised at best and potentially harmful at worst," especially when the message is uncomfortable or goes against what the player already believes.

Two psychological barriers get in the way:

<html>
  <div>
<dl>
  <dt>Psychological reactance</dt>
  <dd>When people sense someone is trying to change their attitudes or behavior, they feel their freedom is threatened, and their defenses go up. Surprisingly, this happens <strong>even when the person already agrees with the message.</strong></dd>
  <dt>The bias blind spot</dt>
  <dd>People accept that bias exists, but deny or downplay their own. Especially relevant for games about stereotypes and prejudice.</dd>
</dl>
  </div>
</html>

There's a cost to fun, too. The authors point out that sensing a persuasive agenda works against being immersed in a game world at all. <span class="highlighter">A game that preaches is both less persuasive and less enjoyable.</span>

---

## 🧩 The Embedded Design Model

The model's core idea: persuasive games work better when the message is <span class="highlighter">woven into the game's content, mechanics, or context of play</span>, rather than being the focal point. The authors present three strategies:

<html>
  <div>
<dl>
  <dt>🔀 Intermixing</dt>
  <dd>Balance "on-message" content with "off-message" content, so the message feels less overt and less threatening.</dd>
  <dt>🎭 Obfuscating</dt>
  <dd>Use genres and framing that point players' expectations away from the game's persuasive goal.</dd>
  <dt>🧟 Distancing</dt>
  <dd>Use fiction, metaphor, and "what if?" scenarios to put psychological distance between the player's own identity and the game's message.</dd>
</dl>
  </div>
</html>

{:.highlight}
The authors' examples are all tabletop games from the Tiltfactor lab at Dartmouth, but they say the principles apply to digital games too. In fact, digital games give designers even more control over things like when information is revealed and how characters are shown.

---

## 🔀 Intermixing

### *Awkward Moment*

*Awkward Moment* is a party game for pre-teens and young teens that aims to reduce gender stereotypes in STEM. Each round, one player draws a "Moment" card describing an awkward situation, and the others play "Reaction" cards in response. Some Moments involve gender bias in STEM. Others are just awkward, like *"You sit on ketchup."*

The key design question was the **ratio** of on-topic to off-topic cards. In the authors' experiments:

- Youth who played an **intermixed** version (about 45% bias-related Moments) showed significantly more perspective-taking afterward than those who played an **overloaded** version (75% bias-related).
- An intermixed version tripled how likely players were to associate women with science after one session.
- Adults who played an overloaded workplace version felt more negative, reported feeling "fed up," and ended up *less* concerned about bias than people who didn't play at all.

### *The Luminists*

In this strategy game, players recruit real-life STEM role models. The goal was to give girls positive female role models in STEM. A version with **equal numbers** of male and female scientists worked better than one where 6 of the 8 were women: girls who played the balanced version felt more connected to the characters and showed higher STEM aspirations and self-efficacy.

<div class="imp" markdown="block">

Intermixing is counterintuitive. Players see *less* of the message, but they're more likely to accept it instead of defending against it.

> **WAIT, ISN'T THAT BOLTED ON?** The [Aligning Objectives]({% link docs/design/aligning-objectives.md %}) and [LM-GM Mapping]({% link docs/design/lm-gm-mapping.md %}) pages warn against content the game could do without. That advice is for teaching a **skill or concept**, where the learning should be the core of play. For **attitude change**, off-message content does a job of its own: it keeps the player's defenses down. The on-message parts should still be built into play, not tacked on.

> **NOTE:** For a vibe-coded game, intermixing often comes down to your content files. If your scenarios, questions, or dialogue live in a ScriptableObject or JSON file, you can tune the on-message ratio without touching code.

</div>

---

## 🎭 Obfuscating

The authors describe three ways to obscure a game's persuasive intent:

1. **Pick a genre that doesn't signal persuasion.** *Awkward Moment* was intentionally designed as a fast, silly party game. *Buffalo: The Name Dropping Game* looks like a trivia game: players race to name a real or fictional person who fits random pairs like "charismatic techie" or "Iranian poet." It's actually based on research showing that exposure to counter-stereotypical examples reduces stereotyping. Players rarely guessed the real goal.
2. **Use neutral framing language.** Telling players *Awkward Moment* was about "awkward social **stereotypes**" made it less fun and less effective than describing it as being about "awkward social **situations**." Framing *Buffalo* as about "pop culture stereotypes" instead of "pop culture knowledge" erased its effect on prejudice.
3. **Delay revealing the sensitive part.** In *Monarch*, players compete as princesses for a throne. Boys who learned their character's gender a few rounds in (after getting attached to the character) identified with their princesses more, and rejected gender stereotypes more afterward, than boys told up front.

---

## 🧟 Distancing

Distancing creates a safe buffer between the player's real identity and a sensitive topic. A game that's immersive already does some of this. The authors add two specific techniques:

<html>
  <div>
<dl>
  <dt>Hypotheticality</dt>
  <dd>Present "what if?" scenarios instead of mirroring players' real experiences. <em>Awkward Moment</em> describes situations happening to an unnamed "you," so no real player's embarrassing moment is in the spotlight.</dd>
  <dt>Fictionalizing</dt>
  <dd>Represent real issues through fantasy or metaphor. <em>POX: Save the People</em> is about vaccination and disease spread. Its <em>ZOMBIEPOX</em> version uses the same rules with a zombie plague. Both shifted attitudes toward vaccination equally, but players of the zombie version were more immersed and showed <strong>more</strong> empathy for real people with infectious diseases.</dd>
</dl>
  </div>
</html>

{:.highlight}
This connects to **Fantasy** in LeBlanc's 8 kinds of fun (see [Aligning Objectives]({% link docs/design/aligning-objectives.md %})). A fantasy layer isn't just decoration: it can make a hard topic safe enough to engage with.

---

## 🛠️ Putting It Into Practice

| Strategy | Design levers | Example from the paper |
|:--|:--|:--|
| **Intermixing** | Ratio of on-topic to off-topic content; balance among characters | *Awkward Moment* (about 45% on-topic), *The Luminists* (50/50 role models) |
| **Obfuscating** | Genre, title and description wording, delayed reveals | *Buffalo* as a trivia game; "situations" instead of "stereotypes"; *Monarch* |
| **Distancing** | Hypothetical scenarios, fantasy or metaphor in place of realism | *Awkward Moment*'s second-person "you"; *ZOMBIEPOX* |

<div class="warn" markdown="block">

**Think through the ethics before you hide your goal.** Obfuscating means not telling players what a game is trying to do to them. If you're testing your game with real students or running a study, talk to your instructor and your IRB about consent, and plan a **debrief** where players learn the game's purpose after they play. Stealth should help the message land, not leave players feeling tricked.

</div>

<div class="task" markdown="block">

**Embedding check.**
- [ ] Is less than all of my content "on-message"?
- [ ] Does the genre set expectations of fun, not of a lesson?
- [ ] Do my title, description, and opening screen avoid announcing the persuasive goal?
- [ ] Are sensitive elements revealed after players are invested, not before?
- [ ] Does fiction, metaphor, or a hypothetical frame give players some distance from the topic?
- [ ] Do I have a plan to debrief players afterward?

</div>

---

## ✏️ Paired Prompt

### Embed your message

```
I'm designing a game that aims to shift players' attitudes or behavior.
Target attitude or behavior: [what should change]
Players: [audience]
Current concept: [1-2 paragraphs, or "none yet"]

Using the Embedded Design model (Kaufman, Flanagan, & Seidman, 2015),
suggest ways to build this goal into the game without announcing it:
1. Intermixing: what off-message content could balance the on-message
   content, and roughly what ratio should I start with?
2. Obfuscating: what genre and framing language would set expectations
   of fun rather than a lesson? Is there an element I should reveal
   later instead of up front?
3. Distancing: how could fiction, metaphor, or hypothetical scenarios
   create a safe distance from the topic?
Then point out any part of my current concept that would likely
trigger reactance because it's too direct or preachy.
Finally, suggest a short debrief activity for after play.
```

<div class="warn" markdown="block">

**Watch for preachy output.** AI assistants love to end persuasive games with a moral, a summary screen, or a character who explains the lesson. That's exactly the overt messaging the model warns against. If you see it, push back: *"Cut anything that states the message directly. Let the player experience it through play."*

</div>

---

## 📚 Sources

- Kaufman, G., Flanagan, M., & Seidman, M. (2015). Creating stealth game interventions for attitude and behavior change: An "embedded design" model. *Proceedings of DiGRA 2015: Diversity of Play: Games – Cultures – Identities.*
