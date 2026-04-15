# "Data: What It Is, What It Can Tell Us, and What It Can't"
### 8th Grade Data Science — Interactive Reveal.js Presentation

---

## Slide 1 — Title Slide

---

## Section 1: Why Do We Need Data?

### Slide 2 — Opening Challenge
- "Raise your hand if you listen to music while studying"
- "Raise your hand if you think it helps"
- Almost every hand goes up
- "How do you know?"
- Take a few responses — then let them sit with the question
- Return to this at the end: "how would you actually design a study to answer this?"

### Slide 3 — The Problem with Gut Feelings
- We are bad intuitive statisticians
- The Birthday Problem: how many people do you need in a room for a 50% chance two share a birthday?
- Almost everyone guesses 180+. The answer is 23.
- Test it live with the class
- Our brains look for stories, not patterns

### Slide 4 — What Data Does for Us
- Replaces "I think" with "here's what we observed"
- Lets us compare, track change over time, and spot things invisible to the naked eye

### Slide 5 — Data Is Everywhere
- Everything measurable is potential data: temperature, test scores, heart rate, rainfall, likes on a post
- Interactive: ask students to name 5 things that were measured about them today

---

## Section 2: What Can Data Tell Us?

### Slide 6 — Two Jobs of Data
- Data has two big superpowers:
  - **Uncover hidden truths** — things happening right now that we can't see with our eyes
  - **Forecast** — predict what hasn't happened yet
- Both depend on the same raw material: careful observation

---

### Part A: Uncovering Hidden Truths

### Slide 7 — Things Too Big, Too Small, Too Slow, or Too Fast to See
- **Too big** — climate change, ocean currents, continental drift
- **Too small** — bacteria, air pollutants, blood chemistry
- **Too slow** — glacier retreat, species extinction, soil erosion
- **Too fast** — lightning, nerve signals, a car crash
- Data makes the invisible visible across all four dimensions of scale
- The data collection method has to match the speed of what you're studying

### Slide 8 — What Does a Dataset Actually Tell Us?
- When you collect data you get a pile of numbers — how do you summarize it?
- Two fundamental questions:
  - **Where is the middle?** — central tendency
  - **How spread out is it?** — variability

### Slide 9 — Central Tendency: Finding the Middle
- Mean, median, mode — three ways to describe "typical"
- They don't always agree — and that disagreement is informative
- Example: average income in a room changes dramatically when a billionaire walks in — median barely moves
- The choice of measure matters

### Slide 10 — Spread: How Much Does It Vary?
- Two datasets can have the same average but look completely different
- Example: daily temperature in San Diego vs. the Midwest — same annual average, wildly different spread
- Spread tells you how much you can trust the middle as a description
- High spread = the average is a weak summary

### Slide 11 — Putting It Together
- Any dataset needs both: where is the center, and how spread out is it?
- These are the two most basic tools of data description
- Everything else in data science builds on these two ideas

### Slide 12 — Correlation as a Clue
- When two things move together it suggests a connection worth investigating
- Example: ice cream sales and shark attacks both spike in summer
- But correlation is just a clue — not an answer

### Slide 13 — The Confounding Variable
- The real culprit: hot weather drives both
- This hidden third factor is called a confounding variable
- Interactive: can you spot the confounding variable? (2-3 quick examples)

### Slide 14 — From Clue to Cause
- How do we go from "these move together" to "this one causes that one"?
- We need to rule out confounders, test mechanisms, replicate findings
- Data starts the investigation — it rarely ends it alone

---

### Part B: Forecasting

### Slide 15 — Predicting What Hasn't Happened Yet
- If uncovering truth looks backward at patterns, forecasting looks forward
- Based on: historical patterns + current conditions + a model of how the system works

### Slide 16 — What Makes a Good Forecast
- A forecast doesn't need to know *why* — just *what tends to happen next*
- Example: you don't need to understand fluid dynamics to notice "when pressure drops fast, it usually rains"
- Patterns in historical data can be enough
- This is how a lot of modern machine learning works — find the pattern, skip the explanation
- A good forecast is: specific enough to be useful, honest about uncertainty, testable

### Slide 17 — Pattern vs. Mechanism
- Pure pattern-based forecasting: powerful but blind — you know *that* it works, not *why*
- The scientific method: uses data to test hypotheses about underlying mechanisms — slower but gives real understanding
- They're not opposites — the best science uses both
- Discussion question: *"Is a forecast that works but has no explanation still science?"*

### Slide 18 — Weather as the Ultimate Forecasting Lab
- Forecasts made and tested every single day
- Instant feedback loop — bad models get caught immediately
- Leads into Section 5

---

## Section 3: Can We Ever Prove Anything?

### Slide 19 — What Would "Proof" Even Mean?
- Ask students: "Can you prove the sun will rise tomorrow?"
- Intuitive answers, then dig in — this is harder than it sounds

### Slide 20 — The Black Swan Problem
- Centuries of Europeans assumed all swans were white — then they reached Australia
- One observation destroyed a universal claim
- No amount of confirming data proves something true forever

### Slide 21 — Popper & Falsifiability
- Science doesn't prove things true — it fails to prove them false
- A claim is scientific only if it *could* be proven wrong
- Good science makes claims that could be wrong — and invites the test

### Slide 22 — What Data Can Do
- Data can support or undermine a claim
- More data = more confidence, never absolute certainty
- This is not a weakness — it's honesty

### Slide 23 — Uncertainty Is Not Ignorance
- Distinguish: "we don't know" vs. "we know the range of likely outcomes"
- Uncertainty, quantified, is still knowledge
- Weather preview: "70% chance of rain" is precise, honest, and useful

### Slide 24 — The Problem of Bad Data
- Garbage in, garbage out
- Biased samples, missing data, measurement error
- Interactive: what's wrong with this survey? (show a flawed example)

---

## Section 4: How Intuition Fails Us — Four Fallacies

### Slide 25 — Our Brains Are Pattern Machines
- Evolution built us to find patterns fast — it kept us alive
- But fast pattern-finding in a data-rich world leads us badly astray
- Four classic ways our intuition breaks down

### Slide 26 — Fallacy 1: The Group Average Fallacy
- Average male grip strength is higher than average female grip strength
- But the distributions overlap enormously
- Many women are stronger than many men
- Knowing someone's group tells you surprisingly little about that individual
- Visual: two overlapping bell curves — the overlap is the lesson
- **The fix:** always look at spread, not just the average

### Slide 27 — Fallacy 2: Survivorship Bias
- WWII planes returned with bullet holes in the wings — engineers wanted to reinforce the wings
- Abraham Wald said: reinforce the engines — planes hit there didn't come back
- We only see the data that survived — the missing data is often the most important
- Modern version: "all these successful entrepreneurs dropped out of college!"
- **The fix:** always ask what data you're NOT seeing

### Slide 28 — Fallacy 3: The Texas Sharpshooter
- Shoot at a barn, then draw the target around the bullet holes
- If you look at enough data you will always find a pattern — even in pure noise
- This is how horoscopes, conspiracy theories, and bad science work
- **The fix:** decide what you're looking for before you look

### Slide 29 — Fallacy 4: The Gambler's Fallacy
- A coin lands heads 10 times in a row — tails feels "due"
- But the coin has no memory — each flip is still 50/50
- Past independent events don't change future probabilities
- Weather connection: just because it hasn't rained in two weeks doesn't mean rain is due — the atmosphere doesn't owe you anything
- **The fix:** ask whether events are truly independent before assuming streaks mean anything

### Slide 30 — The Capstone: Why Intuition Fails
- Gambler's Fallacy and Monty Hall are mirror image errors:
  - **Gambler's Fallacy** — seeing dependence where there is none (the coin is independent but we treat it as connected)
  - **Monty Hall** — seeing independence where there is dependence (the host's door reveal changes everything but we ignore it)
- We connect things that are separate and separate things that are connected
- Our intuition gets dependence exactly backwards — in predictable, systematic ways
- This is not a personal failure — it's how human brains are wired
- It is precisely why we need data, math, and statistical thinking to check our gut

---

## Section 5: Meteorological Forecasting — A Case Study

### Slide 31 — Why Weather Is Perfect for This
- We can't run experiments on the atmosphere
- But we have enormous amounts of observational data
- Forecasts are tested every single day — instant feedback loop
- Every fallacy we just covered shows up in how people misread weather

### Slide 32 — How Weather Data Is Collected
- Stations, satellites, balloons, ocean buoys, radar
- Millions of data points per hour
- The data collection method has to match the speed of the atmosphere
- Central tendency and spread apply here too — what is a "normal" temperature, and how much does it vary?

### Slide 33 — From Data to Forecast
- Physics equations + historical patterns + today's observations
- Ensemble modeling: run the forecast 50 times with slight variations, look at the spread
- The spread of the ensemble *is* the uncertainty

### Slide 34 — Reading Uncertainty Like a Scientist
- "70% chance of rain" — interactive poll on what students think it means
- Reveal: out of 100 days that looked like today, it rained on 70
- Probability is not certainty — and that's honest science
- Cone of uncertainty for hurricanes — same idea, higher stakes

### Slide 35 — How Forecasts Have Gotten Better
- 1960s 1-day forecast = today's 4-day forecast in accuracy
- What improved: more data, better models, more computing power
- Show a simple accuracy-over-time chart

### Slide 36 — What Forecasts Still Can't Do
- Chaos theory — small differences compound over time
- 10-day forecasts are still fuzzy, 30-day nearly impossible
- This isn't failure — it's the honest limit of the data

---

## Slide 37 — Bringing It All Together
- Data describes, compares, finds trends, and predicts
- Central tendency and spread are the foundation of every summary
- Data never *proves* — it builds confidence
- Pattern-based forecasting and mechanism-based science work best together
- Our intuition fails in predictable ways — data is how we correct it
- The best scientists are comfortable saying "probably" and "we're not sure yet"
- Weather forecasting is data science working in public, getting tested every single day

## Slide 38 — Closing Discussion
- Return to the opener: "So — does music help you study? How would you actually find out?"
- "Name something you believe — what data would change your mind?"
- Open Q&A
