# Pre-Mortem-Claude-Skill

# 🔮 Pre-Mortem

### A Claude skill that imagines you already lost, then finds out why.

![Claude Skill](https://img.shields.io/badge/Claude-Skill-D97757?style=for-the-badge)
![Works on Free Plan](https://img.shields.io/badge/Works%20on-Free%20Plan-2ea44f?style=for-the-badge)
![License: MIT](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)

</div>

---

## 💡 The idea

Ask an AI "do I have a chance?" and you'll usually hear why you'll win. That's pleasant, but it hides the real problem: the true reasons for a loss usually only show up **after** the loss.

**Pre-Mortem brings that moment forward.** It assumes you already lost, then works backward to find the quiet problems you can't see from the inside.

> 🧠 Imagining an event as *already happened* helps people come up with more, and more specific, reasons than asking "what might go wrong?"

---

## 🎯 Who is it for?

Use it when you're making **one attempt** that **someone else will judge**, with a yes or no at the end:

| | Situation |
|---|---|
| 🏆 | Competitions and science fairs |
| 💼 | Job and freelance pitches |
| 💰 | Grants and funding requests |
| 🎤 | Exams and auditions |

### 🚫 It is *not* for
- Proofreading or routine draft feedback
- Choosing between options (which phone, which university)
- Everyday decisions
- Pure-luck situations

---

## ⚙️ How it works

**1. 🗣️ Discovery:** Claude asks you questions first. Who are the judges? What do they score on? How would you explain your idea in one sentence? It doesn't analyze anything until it has enough context.

**2. 💀 The pre-mortem:** Claude imagines you lost and gives you **up to 5 hidden reasons, ranked from most to least likely**. They're specific to your situation, not generic advice. It's blunt about your work, never about *you*.

**3. ✨ One honest line:** a single short line on what's genuinely working in your favor.

**4. 🛠️ Fixes, only if you want them:** Claude asks whether you'd like to work on fixes. They come after you say yes, so the failure analysis stays clear.

---

## 🧪 Example (fictional)

> **You:** I'm entering a startup idea competition with an app I built. Why might I lose?
>
> **Claude:** *(asks a few questions about the judges, scoring, and your one-sentence pitch)*
>
> **Claude:** Imagine you lost. The most likely reasons:
> 1. **Your pitch explains how it works, not why anyone needs it.** If the judges are business-minded, the technical part won't earn points.
> 2. **No proof that real users want it.** ...
> 3. ...
>
> **In your favor:** you have a working demo, which many entries won't.
>
> Want to start working on fixes?

*(This is a made-up example to show the format, not real output.)*

---

## 📥 Install

1. ⬇️ Download **`pre-mortem.skill`** from the [Releases](../../releases) page.
2. 🧩 In Claude, go to **Customize → Skills**.
3. ➕ Click **+**, choose **Create skill**, then **Upload a skill**.
4. 📂 Select the `pre-mortem.skill` file.
5. ✅ Make sure the skill is switched on, and that code execution is enabled in **Settings → Capabilities**.

Then start a chat and describe what you're entering. Works on the **free plan** too.

> Menu names can differ slightly between web and mobile.

---

## 📁 What's inside

```
pre-mortem/
├── SKILL.md                      # the main method
└── references/
    ├── competitions.md           # silent killers: competitions & science fairs
    ├── pitches.md                # silent killers: job & freelance pitches
    ├── grants.md                 # silent killers: grants & funding
    ├── prospective-hindsight.md  # the core method
    ├── curse-of-knowledge.md
    ├── outside-view.md
    ├── disconfirming-evidence.md
    └── planning-blind-spots.md
```

The checklists list **problems only, never fixes**. Claude opens only the notes that fit your situation.

---

## 🧠 The thinking tools behind it

| Tool | In plain words |
|---|---|
| 🔭 **Prospective hindsight** | Imagine it already failed, then ask what happened. |
| 🧱 **Curse of knowledge** | Experts forget what it's like not to know, so they explain things in ways the judges can't use. |
| 🌍 **Outside view** | Judge by how entries like yours usually fare, not just your own story. |
| 🔍 **Disconfirming evidence** | Look for what you *haven't* checked, not just facts that support you. |
| ⏳ **Planning blind spots** | People underestimate time and last-minute problems. |

---

## ⚠️ Please read: limits and warnings

- 📉 **It leans negative by design.** It will almost always find reasons you could lose, even when your chances are good. A list of weak spots does **not** mean you'll lose.
- 🎲 **The ranking is rough judgment, not real math.** It does not give percentages or exact odds.
- 🙈 **It can't know your judges unless you tell it.** The better your answers to its questions, the better the result. If you don't know the judges, it will state an assumption and continue.
- 🌐 **Language:** it replies in the language you write in, including Bangla.
- 🧪 **Early version.** It has had limited real-world testing. Feedback is welcome.

---

## 🤝 Feedback and contributing

Found a case where it gave generic or unhelpful reasons? Open an [issue](../../issues) and describe what happened. Ideas for new checklists (exams, auditions, and more) are welcome too.

---

## 📄 License

Released under the [MIT License](LICENSE). Add a `LICENSE` file when you create the repo (GitHub can generate one for you).

---

<div align="center">

Made by **Amir Asaadullah Chowdhury**

*If this helped you, consider giving the repo a ⭐*

</div>
