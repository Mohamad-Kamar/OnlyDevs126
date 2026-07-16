# Speaker guide — end-game talk

These are talk beats, not a script to memorise. Keep the language direct and conversational. The audience should remember the habit—keep following the effect—and the final question, not five definitions.

## Slide 1 — Title

Let the title sit for a moment. Do not define systems thinking yet.

## Slide 2 — A one-line change. Three weeks later.

“A one-line change. You were sure: an afternoon, tops. It shipped three weeks later. You have been there.”

“Here is the strange part: the line was never the whole problem. Everything around the line was.”

Keep this calm. It is recognition, not a dramatic incident story.

## Slide 3 — A field we already partly know

“There is a whole field that studies why systems keep behaving a certain way, even when the people inside them are trying to improve them.”

Point out that systems thinking is commonly applied to ecology, economies, organisations, cities, management, and product design.

Then bring it home:

“Software engineers are not starting from zero. We already trace dependencies, watch queues, build feedback into tests and monitoring, and expect one change to affect another part of the system.”

“Formal systems thinking gives us useful names. More importantly, it teaches us to choose a wider boundary.”

## Slide 4 — Keep following the effect

“We usually stop tracing when we find the code path. Today, we keep going—from the code all the way to the people who live with what it changes.”

“Do not worry about collecting five new terms. Notice the move: each time, we keep following the effect.”

This is the promise: seeing sooner creates better questions. Do not promise a fix for every system in 25 minutes.

## Slides 5–7 — Code: feedback loops

### Name it

“A feedback loop happens when the result comes back and affects what happens next.”

### Recognise it

Flash the fork bomb and infinite re-render quickly. Do not turn either into a mini-lecture.

### Explain it

Build the retry loop in ordinary words: more failures lead to more retries; retries add load; more load creates more failures.

“One retry can be sensible. When every failed request creates another request, the recovery action adds load to the thing already struggling.”

Person plant:

“Someone wrote that retry. It was the right call—retrying a flaky call is good engineering. The loop is what turned a good call into a bad day.”

Only after the shape is clear, name it a **reinforcing feedback loop**.

Carry forward:

“What comes back and changes what happens next?”

Transition:

“In running code, a loop can happen in seconds. In delivery, the effects can take weeks, which makes them much easier to miss.”

## Slides 8–10 — Delivery: stocks, flows, and delays

### Name it

“A stock is something that piles up. A flow adds to it or removes from it. A delay is the wait before we see the result.”

Use simple examples: backlog, open pull requests, a test queue, and work that looks done but has not been tested end to end.

### Recognise it — show of hands

“Think about the software projects you have worked on. How often did they finish when you first expected them to?”

Ask in order: Always → Usually → Sometimes → Rarely → Never.

“Interesting. We are good engineers. We plan, estimate, track work, and learn from previous projects. So why is this still so hard?”

Do not blame planning, managers, or engineers. Let the question lead to the diagram.

### Explain it

Start with “work still to do” and “work looks complete.” Reveal “problems not found yet” as the hidden stock, then the delayed return as rework.

“A plan can show what we intend to finish. It cannot show work we do not yet know is coming back.”

Person plant:

“Someone marked that work done. They were not wrong—it looked done. The rework was hiding where no plan could show it.”

The MIT rework cycle is a model to investigate, not proof that one mechanism explains every late project.

Carry forward:

“Where does work keep piling up, and why do we only notice when we are already late?”

## Slide 11 — Video

Open the linked [Uncle Bob video](https://www.youtube.com/watch?v=RlNpMz6X9lc) from the attribution card.

Do not add a spoken summary, transcript, extracted lesson, or interpretation. Let the video play and continue.

Transition:

“Now imagine we make one flow much faster: creating code. Does the whole delivery system become faster with it?”

## Slides 12–14 — AI interlude: moving the bottleneck

### Frame the interlude

“AI is not another boundary outside Delivery. It is a force that can speed up parts across the system.”

“Making one step faster helps until another step becomes the limit. That limiting step is the bottleneck.”

Keep the claim local: teams and workflows differ.

### Recognise it — show of hands

Ask:

1. “Who uses AI while coding?”
2. “Who feels writing code became faster?”
3. “Who feels reviewing, understanding, testing, and shipping became equally faster?”

Pause and let the pattern in the room be visible.

### Explain it

Walk through Create → Understand and review → Test and integrate → Run and maintain. Widen only the first flow.

“Code creation is one flow, not the whole outcome. If later steps do not improve too, the constraint moves and work waits somewhere new.”

Person plant:

“Someone accepted that AI-generated pull request. Faster was the whole point. The waiting did not vanish—it moved to the reviewer.”

Carry forward:

“What became faster, and what became the new bottleneck?”

Transition:

“Even if we make the whole path faster, we still have another question: did the software help anyone?”

## Slides 15–17 — Product: balancing feedback

### Name the bookend

“Code showed us a loop that amplifies. Product gives us a loop that can steer.”

“A balancing loop compares what is happening with what we want, then acts to close the gap.”

### Recognise it — silent reflection

“Think of a feature your team shipped successfully. It worked. It was released. The ticket was closed. How did you know it actually helped anyone?”

Pause. No hands.

Person plant:

“Someone closed that ticket. It shipped, it worked, the ticket was green. Nobody was told whether it helped a single user.”

### Explain it

Show the open path: Build → Ship → Close ticket. Then show the return path: user response → next decision → next change.

Use the provisional wording:

“Shipping tells us what we did. The user’s response tells us what changed. When that response shapes what we do next, that is a feedback loop.”

One leverage demonstration:

“The move is not to add another dashboard. Wire one useful signal back to a decision that somebody can actually make.”

Carry forward:

“What changed for the user—and how will that change what we do next?”

Transition:

“Code does not decide to retry. Work does not decide it is done. AI does not decide a pull request is ready. People make those choices inside the structure around them.”

## Slides 18–20 — People: the destination

### Collect the people already in the talk

“Every system today already had a person in it—the one who wrote the retry, the one who marked the work done, the one who accepted the pull request, and the one who closed the ticket.”

“Each made a sensible choice. That is why we end here.”

“Structure shapes behaviour” is not a new stop. It is the generalisation of the choices the audience has already seen.

### Recognise it — private reflection

“Think of the person everyone calls when something breaks. What happens when they are not there?”

Do not ask anyone to identify the person or confess a team problem aloud.

### Explain it

Walk through the hero loop: one person understands the system → they rescue the incident → immediate relief → deeper improvement waits → dependence grows.

“The engineer did something valuable. Thank them. But if the same person must save the system every time, the rescue is also telling us something about the system.”

“The retry cost seconds. Hidden rework cost weeks. An open product loop can cost users. A hero system can cost someone their Saturday.”

Do not diagnose burnout from one example. The warning sign is repeated dependence on the same people’s time and attention.

## Slide 21 — Close

Let the completed journey sit behind one question:

> **What is the system teaching people to do?**

Do not recap the five definitions or the five carry-forward questions.

Final spoken line:

> **“Start with the code. Follow what it changes. End with the people.”**

Then stop.

## Rehearsal guardrails

- The video takes 1:50. If time is tight, trim AI explanation before trimming People.
- Keep the Code and Delivery definitions short.
- Let the show-of-hands and reflection pauses breathe, but do not discuss answers in the room.
- Treat every causal diagram as a model to test, not a diagnosis proven by a slide.
- Keep the person plants to one sentence each.

## Q&A prompts and careful answers

- **“Isn’t this just root-cause analysis?”** It is complementary. Systems thinking pays explicit attention to boundaries, accumulations, feedback, delays, goals, and behaviour over time.
- **“Does every problem need a causal-loop diagram?”** No. Use the smallest model that helps. A simple bug often deserves a direct fix.
- **“Can developers change organisational conditions?”** Not all alone. They can make the pattern visible, ask a sharper question, change local defaults, and bring evidence to whoever owns the wider rule.
- **“Is the AI section saying AI slows teams down?”** No. It asks which parts changed speed and where the limiting step is now. The answer is local.
