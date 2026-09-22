---
title: Instructions & Systems
date: 2026-09-14
week: 1
tags:
  - instructions
  - systems
  - journal
publish: true
---

> [!important] Complete this week's exercises and reflections yourself
> Lesson 01 is a **Human-only** session: do not use generative AI to invent rules, write or debug the p5.js exercise, or write your process notes. This page is only a structure for documenting your own work.

- [Lesson 01: Instructions & Systems](https://digitalideation.github.io/gencg_h2601/lessons/lesson01_intro/)
- [Journal guidelines](https://github.com/digitalideation/gencg_h2601/blob/refactor_2026/lessons/extra/journal.md)

## Evidence checklist

Keep evidence of the process, not only the successful result.

- [x] Original drawing or idea
- [x] First instruction set
- [x] First execution by another person
- [x] Moments of confusion or ambiguity
- [x] Revised instructions
- [ ] Second execution
- [ ] Small rule system
- [ ] Sketch or diagram of the system
- [ ] p5.js translation

<!-- Add images to ./sketches/ and embed them like this:
![[./sketches/your-file-name.jpg]]
-->

## 1. Exploration & Experimentation

### Human → Human

**Original idea**

>![[WhatsApp Image 2026-09-15 at 17.41.17.jpeg|230]]

**First instruction set**

1. You will need an A4 plain paper, orientated vertically, and a black felt tip.
2. In the middle of the page draw a 1cm x 1cm (approx.) square, fill it in.
3. From the bottom right corner of the square, draw a straight line to the right, approx 4cm. Then stop and continue the line upwards, approx. 10cm. 
4. Stop and continue the line to the left, make a circle that goes through the line.
5. From the left corner of the square, make the first 2 lines you did but mirror them. When you have done the 2nd line (10cm going downwards), draw a 10cm line to the right, then draw a line to the bottom approx. 10cm.
6. Draw a circle with aa radius of 2mc at 2cm of the last line you drew, it has to overlap the line.

**First execution** (by Vishy Pravin)
![[WhatsApp Image 2026-09-21 at 22.10.08.jpeg|252]]


**Where did interpretation differ?**

- Interpretation of approximative size/length differs
- "draw a straight line to the right" appears to no be clear enough - line was drawn diagonally, down. 
- part 5) is also unclear, as I did not explain in which axis it should be mirrored.

**Revised instructions**

2. In the middle of the page draw a 1cm x 1cm (approx.) square, fill it in.
3. From the bottom right corner of the square, draw a straight line to the right, approx. 4cm. Then stop and continue the line upwards, approx. 10cm. 
4. Stop and continue the line to the left, make a circle that goes through the line.
5. From the left corner of the square, make the first 2 lines you did but mirror them. When you have done the 2nd line (10cm going downwards), draw a short line to the right, approx. 2cm, then draw a line to the bottom approx. 10cm
6. Draw a circle with a radius of 2cm at the end of the last line you drew, it has to overlap the line.

**Second execution**

<!-- Embed or link the second result. What changed? -->
(not done)
### Small rule system

- **Starting condition:** draw a square in the centre of the page.
- **Action:** 
- **Relationship:**  the line connects to the previous shape's point to the next shape's point
- **Variation:** 
- **Constraint:**
- **Stopping rule:** 

<!-- Add a sketch or diagram of the system. -->

### Human → Computer

What did a human understand automatically that the computer needed you to specify?

-
-

```js
// function setup() {

  createCanvas(windowWidth, windowHeight);

}

  

function draw() {

  background(230);

  rectMode(CENTER);

  

  // quare properties

  let centerX = width / 2;

  let centerY = height / 2;

  let size = 25;

  // bottom right corner

  let cornerX = centerX + (size / 2); // Move right

  let cornerY = centerY + (size / 2); // Move down

  // draw the black square

  rectMode(CENTER);

  fill(0);

  noStroke();

  rect(centerX, centerY, size, size);

  // draw a line starting from the bottom-right corner

  stroke(0);

  strokeWeight(2);

  line(cornerX, cornerY, 350, 350); // Ends at (350, 350)

  

}
```

**Parameters tested**

| Parameter | Values tried | What changed |
| --------- | ------------ | ------------ |
|           |              |              |
|           |              |              |

**Technical challenges or failed attempts**

-
-

## 2. Influences & References

Choose at least one work, artist, or idea from the lesson or your own research.

- **Artist / work:**
- **Link or citation:**
- **What I noticed:**
- **How it connects to my experiment:**

Possible starting points from the lesson include Sol LeWitt, Conditional Design, George Brecht, Alison Knowles, and Yoko Ono.

## 3. Algorithmic Thinking

**What stays fixed?**

-

**What can vary?**

-

**Describe the system in plain language or pseudocode**

```text
START

ADD YOUR RULES HERE

STOP WHEN ...
```

**How do the rules produce the visual result?**

<!-- Explain the relationship between your instructions and the outcome. -->

## 4. Critical Reflection

- One thing my executor interpreted differently was...
- One rule I changed was...
- One ambiguity I decided to keep was...
- One thing I had to make explicit for the computer was...
- What worked or surprised me?
- What did not work, and why?
- What would I explore next?

## Next steps

- [ ] Save all drawings and outputs
- [ ] Check that images and links work
- [ ] Choose one question to carry into Week 2
