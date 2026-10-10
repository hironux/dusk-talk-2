# Dusk Talk 2

Development line after the hackathon submission. The submitted version, **Dusk Talk**
(https://github.com/hironux/dusk-talk), is kept as it was and is not changed here.

Storage keys are prefixed `dusktalk2_` so both apps can live on the same GitHub Pages domain without sharing data.

## What is different from Dusk Talk

- **Reading the feeling**: weighted word lists, negation ("not tired"), strength ("very" / "a bit"), contrast ("tired, but relieved"), two feelings at once, topics (work, family, ...). Japanese and English.
- **The sky**: always a full-screen dusk gradient. Feelings tint it; a second feeling is blended into every color stop (all palettes are dusk-family, so a mix never turns gray). The sun/moon grows with intensity.
- **Conversation**: stages (listen, go deeper, toward tomorrow); question types never repeat within 3 turns; tappable choices; a gentle way out when the answer is "I don't know"; callbacks to what you said earlier.
- **Listening first** (reflective listening / OARS in spirit): a small recap once a night ("if I gently sum it up so far..."); some turns only receive what was said and ask nothing (after a long heavy message, and every third turn); the positive question ("a moment of relief?") is held back on heavy nights and early turns; the 0-10 question at most once a night; the "step for tomorrow" can be skipped ("Not now").
- **Today's line**: a one-line card built from your own words, the arc of the night, and the topics. Copy button.
- **Care**: gentle message with crisis lines for heavy words; no cheerful summary on such nights.
- **Next day**: the "step for tomorrow" is shown at the start of the next night.

## What this is not

Not medical care or counseling, and it promises no results. The on-screen notice says so and points to people and professional lines when the heaviness lasts.

## Not yet

No AI yet. Replies come from `planReply()` in `index.html`. The AI hookup goes into `getReply()` (see the comment there);
it needs a server-side endpoint so the API key is never in the page.
