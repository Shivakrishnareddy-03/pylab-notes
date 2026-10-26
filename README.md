# pylab-notes

**Python notes with hand-worked examples, common mistakes, and exercises that go from easy to tricky. One small step at a time, from your first line of code to job-ready skills.**

Written by a Master's student in Data Analytics while learning Python. Every topic is explained the way I wish it had been explained to me: from first principles, with one small example worked by hand before any formula or syntax.

> Status: in progress. New topics are added as I finish them. Watch or star the repo to follow along.

---

## Who this is for

- **University students** taking an introductory Python or data-analytics course.
- **Self-learners** who want a clear path instead of random tutorials.
- **Job seekers** preparing for data analyst, data science or Python developer interviews.
- **Anyone switching from another language** (Excel, MATLAB, C, JavaScript...). Python's surprises are flagged in the notes, because that is where most mistakes happen.

No prior programming knowledge is required. If you already code, you will move faster, and you will see "Watch out" boxes wherever Python behaves differently from what you might expect.

---

## How every topic is built

Each topic follows the same five parts, so you always know where to look:

1. **The idea.** A plain-English explanation with a small example worked by hand first, then the same thing in code.
2. **Common mistakes.** The errors that actually happen (real ones, from real practice) and how to spot them.
3. **Quick recap.** Three questions from *earlier* topics, so nothing is forgotten as you move forward.
4. **Exercises, easy to tricky.** Warm-ups first, then problems that mix several ideas, then a few that are deliberately tricky.
5. **Solutions.** In a separate file. Try first, then check.

Everything is available as a Markdown page to read and a Jupyter notebook to run.

---

## Roadmap

Topics follow a beginner-to-advanced order. Order and names may shift as the material grows.

| # | Topic | What you will be able to do | Status |
|---|-------|-----------------------------|--------|
| 01 | **Basics:** calculator, data types, strings, `if`, loops, imports | Write small programs with decisions and repetition | In progress |
| 02 | **Lists, tuples, dictionaries, sets** and list comprehensions | Store and reshape collections of data | Planned |
| 03 | **Functions** and scope | Package code so it can be reused and tested | Planned |
| 04 | **Classes and objects** (OOP I) | Model real things as objects | Planned |
| 05 | **Object-oriented programming II** | Inheritance, structure, cleaner designs | Planned |
| 06 | **NumPy** | Fast numerical work on arrays | Planned |
| 07 | **pandas** | Load, clean, group and summarise tables of data | Planned |
| 08 | **Plotting** with matplotlib and seaborn | Turn data into clear charts | Planned |
| 09 | **Machine learning** with scikit-learn (and statsmodels) | Fit and evaluate a first model | Planned |
| 10 | **Capstone projects** | Portfolio-ready mini projects | Planned |

---

## Repository structure

```
pylab-notes/
|-- README.md
|-- LICENSE
|-- 01-basics/
|   |-- README.md          # the notes
|   |-- notebook.ipynb     # run the code yourself
|   |-- exercises.md       # easy -> tricky
|   `-- solutions.md       # try first!
|-- 02-lists-and-dicts/
|   `-- ...
|-- revision/
|   |-- after-01-02.md     # mixed questions from topics 01 and 02
|   `-- ...                # grows after every few topics
`-- cheatsheets/
    `-- python-gotchas.md  # quick list of the classic mistakes
```

The `revision/` folder is how this repo fights forgetting: after every couple of topics there is a mixed quiz that makes you use old ideas together with new ones.

---

## How to use this repo

1. Read a topic's `README.md` slowly. Do not skip the hand-worked example.
2. Open `notebook.ipynb` and run each cell. Change the numbers and see what breaks.
3. Do the exercises **before** looking at the solutions. Getting something wrong and fixing it is where most of the learning happens.
4. Do the matching `revision/` quiz before starting the next topic.

**Setup:** install [Anaconda](https://www.anaconda.com/download) (it already includes Python, Jupyter, NumPy, pandas, matplotlib, seaborn, scikit-learn and statsmodels), or run the notebooks in Google Colab with no installation.

---

## A taste: classic Python gotchas

| You might write | What Python actually does | What you wanted |
|---|---|---|
| `5^3` | gives `6` (`^` is a bit-level operation) | `5**3` gives `125` |
| `7/2` | gives `3.5` | `7//2` gives `3` (integer division) |
| `x = [5, 6, 7]`, then `x[1]` | gives `6`, the *second* item | `x[0]` is the first |
| `2 * [2, 3, 4]` | repeats the list: `[2, 3, 4, 2, 3, 4]` | `[2*v for v in [2, 3, 4]]` gives `[4, 6, 8]` |
| `int(2.9)` | gives `2` (drops decimals, no rounding) | `round(2.9)` gives `3` |
| `bool("False")` | gives `True` (any non-empty text is `True`) | compare text explicitly |

Notes like this are why every topic has a "common mistakes" section.

---

## Contributing

Spotted a mistake, an unclear sentence, or a better example? Please open an issue or a pull request. New exercise ideas (with solutions) are especially welcome.

---

## About

These notes are written in my own words as personal revision while studying Python. They are not official course material and are not affiliated with or endorsed by any university. They do not include any assessed work or answers to graded assignments.

Built by **[Your Name]**. Find me on [GitHub](https://github.com/your-username) and [LinkedIn](https://www.linkedin.com/in/your-profile).

## License

Released under the MIT License. See [LICENSE](LICENSE).

If these notes help you, give the repo a star. It helps others find it.
