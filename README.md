# Set up Agent Reach with Claude Code

<div dir="rtl">

دليل سريع لتركّب [Agent Reach](https://github.com/Panniantong/agent-reach) وتعطي الـAI تبعك عيون على الإنترنت:
يحضرلك فيديوهات يوتيوب (عن طريق الترجمة)، يدوّر على Reddit و GitHub، ويقرا صفحات الويب. بياخد حوالي 5 دقايق.

**شو بدّك قبل ما تبلّش:**

- Claude Code، أو أي AI agent بيقدر يشغّل أوامر بالـterminal (Codex، Cursor…).
- Agent Reach مجاني و open source (رخصة MIT). بس اشتراك الـAI تبعك بيضلّ متل ما هو.

</div>

*A quick guide to installing [Agent Reach](https://github.com/Panniantong/agent-reach), which gives your AI agent eyes on the
internet: YouTube transcripts, Reddit and GitHub search, and web pages. It takes about 5 minutes. You need Claude Code
or another agent that can run terminal commands. Agent Reach is free and MIT-licensed; your agent's own plan still
applies. English is under the Arabic in each step.*

> Checked on Windows 11 with Claude Code on 11 November 2026, for Agent Reach 1.6.1. If a step fails, the
> [official install guide](https://github.com/Panniantong/agent-reach/blob/main/docs/install.md) has the latest steps.

---

## 1. Install it with one message

<div dir="rtl">

افتح Claude Code وابعتلو هالجملة بالحرف:

</div>

Open Claude Code and send it this, exactly:

```text
Install Agent Reach for me: https://raw.githubusercontent.com/Panniantong/Agent-Reach/main/docs/install.md
```

<div dir="rtl">

هو بيكمّل لحالو: بيركّب `uv`، بعدين Agent Reach، وبيشغّل `agent-reach setup`. بالآخر لازم يقلّك إنو
GitHub و YouTube والويب جاهزين. إذا سألك يسمحلو يشغّل أوامر، قول نعم.

</div>

It installs `uv`, then Agent Reach, then runs `agent-reach setup`. At the end it should report GitHub, YouTube and the
web as ready. If it asks permission to run commands, say yes.

## 2. The one tip that saves you an hour: ask for English subtitles

<div dir="rtl">

Agent Reach بيطلب ترجمة يوتيوب **بالصيني** أول شي. يوتيوب بيحظر هالطلب، وAgent Reach بيوقّف يوتيوب
**ساعة كاملة**. فدايماً قول بالـprompt: **English subtitles** أو `--lang en,en-orig`.

</div>

By default Agent Reach asks YouTube for **Chinese** subtitles first. YouTube rate-limits that, and Agent Reach then
pauses its YouTube channel for **an hour**. Always say **English subtitles**, or `--lang en,en-orig`.

## 3. Try it

<div dir="rtl">

جرّب هول بـClaude Code:

</div>

Try these in Claude Code:

```text
Use Agent Reach: read the English subtitles (--lang en,en-orig) of this video [link] and summarise it for me.
```

```text
Use Agent Reach: search YouTube for "[your topic]" and rank the videos by views.
```

<div dir="rtl">

مثال حقيقي: فيديو freeCodeCamp عن System Design، ساعتين و5 دقايق، طلع منو 20,861 كلمة بـ4.2 ثواني.

</div>

A real run: freeCodeCamp's 2:05:22 System Design course came back as 20,861 words in 4.2 seconds.

## 4. Sites that need a login

<div dir="rtl">

- **بلا login:** يوتيوب (بحث وترجمة)، GitHub، الويب، والبحث على Reddit.
- **بدها login:** قراءة كومنتات Reddit، X، Instagram، Facebook، ووظايف LinkedIn.
- Agent Reach بيفتح نافذة Chrome خاصة فيه، وانت بتعمل login بإيدك. **استعمل حساب تاني، مش حسابك الأساسي**:
  المواقع بتحظر الحسابات اللي بتستعمل أدوات أوتوماتيك.

</div>

- **No login:** YouTube search and subtitles, GitHub, the web, Reddit search.
- **Login needed:** Reddit comments, X, Instagram, Facebook, LinkedIn jobs.
- Agent Reach opens its own Chrome window and you log in yourself. **Use a second account, not your main one**:
  platforms restrict accounts used for automated access.

## 5. Watch out for scams

<div dir="rtl">

- الـpackage اللي اسمها `agent-reach` على PyPI **مش** هالمشروع. ركّب بس من رابط GitHub فوق.
- ما في token ولا عملة crypto لـAgent Reach. أي حدا بيطلب منك تربط wallet هو نصّاب.

</div>

- The PyPI package named `agent-reach` is **not** this project. Install only from the GitHub link above.
- Agent Reach has no token or coin. Anyone asking you to connect a wallet is a scam.

## 6. If you get stuck

<div dir="rtl">

- قول للـAI: "check Agent Reach status".
- إذا قلّك YouTube "rate limited": استنّى ساعة، وتأكد إنك طالب English subtitles.

</div>

- Ask your agent: "check Agent Reach status".
- YouTube says "rate limited": wait an hour, and make sure you asked for English subtitles.

---

<div dir="rtl">

من [@alihaidar.dev](https://www.instagram.com/alihaidar.dev/). خبرني شو عم تخلّي الـAI تبعك يحضر 👀

</div>

By [@alihaidar.dev](https://www.instagram.com/alihaidar.dev/). Not affiliated with Agent Reach or its author.
