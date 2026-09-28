# Lesson Planner

Plan gradual-release lessons (I Do → We Do → You Do) for any grade, K–12, and grade student work against an answer key with Claude.

Live site: https://bebopoutlawstar-cloud.github.io/lesson-planner/

## Plans

- One plan per week, with a tab for each school day
- Grade picker (K–12) and subject color themes: Math, ELA / Reading, Science, Social Studies
- Fields: Essential Question, standards, I Can statements, vocabulary, materials, Scaffolding & ELL supports, Anticipatory Set, I Do, We Do, You Do, practice problems, Wrap Up
- Start a line with `Kagan:` in We Do or You Do and it is highlighted
- Assessment or special days show in orange
- **Excel** export (one column per day) and **printable PDF** export (one page flow per day)
- **Copy to next week** duplicates a plan and moves every date forward 7 days
- **Draft empty fields with Claude** (needs an API key) fills in a day from its lesson and unit

## Grade work

1. Type the answer key, or upload photos or a PDF of it. Add point values like `(2 pts)`.
2. Add photos or scans of student papers. Each file can be one student, or all the files can be one student's pages.
3. Click **Grade**. The app marks every question, totals the score and writes short feedback.
4. Check the results. Click any mark to change it, edit the feedback, and download a scores CSV.

Answers the app can't read are marked **Unclear** so you can check them yourself.

## Standards data

- Tag each answer-key line with its standard in brackets: `3) 1.56 (2 pts) [5.NBT.B.7]`. Or fill in **Standard for untagged questions** when a whole quiz covers one standard.
- After grading, each assignment shows every standard as **Met**, **Approaching** or **Not yet**, with the students in each group, and a **Standards CSV** download.
- The **Data** page combines every graded assignment into a student × standard grid, a list of standards to reteach as a class, and reteach groups for each standard. Filter by subject and grade, and download it as a CSV.
- Cutoffs default to Met ≥ 80% and Approaching ≥ 60%; change them in Settings. Answers marked Unclear are left out until you mark them.
- Students are matched by name across assignments, so type names the same way each time.

### Two ways to grade (choose in Settings)

- **Free text reader (default):** runs in your browser with [Tesseract.js](https://github.com/naptha/tesseract.js). No key, no cost, and photos never leave your computer. Best for typed worksheets or neat print with answers numbered like `1) 16.25`, one per line. It understands equivalent numbers (1/2 = 0.5), multiple-choice letters, and small spelling slips, but not messy handwriting, long written answers, or partial credit.
- **Claude (optional):** reads handwriting, gives partial credit and writes feedback. Needs your own API key.

## Claude API key (optional)

Claude grading and drafting use your own key from Anthropic:

1. Sign in at [console.anthropic.com](https://console.anthropic.com), add credit under Billing, and create a key under API Keys.
2. In the app, open **Settings**, paste the key, click **Save key**, then **Test key**.

The key is saved only in your browser and sent only to Anthropic's API. Anthropic bills your account for each paper graded. Don't save your key on a shared computer.

## Privacy

Plans, assignments and scores are saved in your browser (localStorage). There is no account or server. With the free reader, student photos stay on your computer. With Claude grading, photos are sent to Anthropic and are not stored by this site. Use first names or student numbers.

## Run it or deploy it

Open `index.html` in a browser. To host it, push the folder to GitHub and turn on **Settings → Pages → Deploy from a branch → main / (root)**.

## Files

| File | What it is |
| --- | --- |
| `index.html` | The whole app: HTML, CSS and JavaScript |
| `sample.json` | Sample plan for the "Try a sample plan" button |

## Credits

Made by Cole Eggly, based on his Lesson Planner Claude skill. Built with help from Claude.
