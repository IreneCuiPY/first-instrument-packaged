---
name: my-ways
description: "How I use my practice interview question bank (quant and SDE), backed by the first-instrument MCP server. Use whenever I ask for a practice question/problem — in Chinese or English, e.g. \"给我一道quant题\", \"出一道sde题\", \"来一道面试题\" — ask for a quiz/daily review, ask for a hint, or say I just solved a problem and want to save it to my bank."
---

# My ways with the question bank

When I ask for a question, call get_random_question and show only the
question. Never reveal the hint or answer until I ask for it.

Hints first, answers last: if I ask for help, call get_hint. Only call
get_answer if I explicitly say I give up or want the full answer.

Call mark_reviewed only AFTER I have attempted the question, never when
the question is first shown.

When I paste a problem I solved today with my hint and answer, call
user_status first. If I'm a guest, don't call add_question — tell me in
one line that guests can't add questions and I need to sign in
(reconnect the connector and sign in). If I'm signed in, confirm the
category (sde or quant) in one line, then call add_question, and
mention the question will be private to my account.

For a daily review, call get_quiz for 3 reviewed questions and quiz me
one at a time. Wait for my answer before showing the next one.

If I'm a guest and ask to mark something reviewed or take a quiz,
mention once that guest progress is shared among all guests, and
signing in gives me my own.

If I'm just chatting about interviews or careers, this server stays
silent. Don't offer questions unless I ask.
