# PA Study Bank — 240 Questions

Mobile-first SOA Exam PA question bank. Works on phone, tablet, or desktop. Progress saves automatically in your browser.

## Deploy to GitHub Pages (free, 5 minutes)

1. Go to github.com → New repository → name it `pa-study-bank`
2. Upload both files: **index.html** and **questions.js**
3. Go to **Settings → Pages → Source → Deploy from branch → main / root → Save**
4. Visit: `https://YOUR-USERNAME.github.io/pa-study-bank/`
5. On your phone: tap **Share → Add to Home Screen** — works like an installed app

## What's included

- **240 questions** covering all 13 Exam PA topics from the Coaching Actuaries manual
- **4 study modes**: All Questions, Weak Areas, Not Yet Seen, Timed Mode (3 min/question)
- **Topic drill**: Tap any topic on the home screen to practice it alone
- **Difficulty filter**: Easy / Medium / Hard via the settings button
- **Progress tracking**: Mastered count, accuracy, per-topic stats — saved in your browser
- **Daily streak** counter to keep you consistent
- **Answer review**: Full explanations + learning objectives after each quiz

## Topics covered (questions per topic)

| Topic | Questions |
|---|---|
| Data Fundamentals | 25 |
| Sampling | 15 |
| EDA | 20 |
| Data Transformation | 15 |
| Statistical Learning | 10 |
| Multiple Linear Regression | 30 |
| Regularization | 15 |
| GLM | 25 |
| Decision Trees | 20 |
| Ensemble Methods | 15 |
| PCA | 13 |
| Clustering | 15 |
| Business Context | 22 |

## Adding more questions

Open **questions.js** and add new objects inside the `QUESTIONS` array following this exact format:

```javascript
{
  id: 241,                           // unique number, increment from last
  topic: "GLM",                      // must exactly match a topic name above
  diff: "Medium",                    // "Easy", "Medium", or "Hard"
  lo: "Describe what this tests",    // learning objective (one sentence)
  q: "The full question text here?", // the question
  opts: [                            // exactly 4 options
    "Option A",
    "Option B", 
    "Option C",
    "Option D"
  ],
  ans: 1,                            // 0-indexed correct answer (0=A, 1=B, 2=C, 3=D)
  exp: "Explanation of why the correct answer is right, referencing the concept."
},
```

## Reset progress

Open browser console and type: `resetAll()`
