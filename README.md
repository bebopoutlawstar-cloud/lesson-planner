# Eggly Lesson Planner

A gradual-release lesson planner for Legacy Traditional School, 5th grade. Plan a run of school days (I Do → We Do → You Do), see each day as a printable page as you type, and download the week as an Excel workbook or a printable PDF.

## Features

- One plan per week, one tab per school day
- Subject color themes: Math, ELA / Reading, Science, Social Studies
- Fields: Essential Question, NVACS standards, I Can statements, vocabulary, materials, Scaffolding & ELL supports, Anticipatory Set, I Do, We Do, You Do, practice problems, Wrap Up
- Start a line with `Kagan:` in We Do or You Do and it is highlighted (red in Excel, orange in the PDF)
- Mark assessment or special days, which show in orange
- **Excel** export: one column per day, landscape, header row and label column repeat when printed
- **Printable PDF** export: one page flow per day
- "Copy to next week" duplicates a plan with every date moved forward 7 days
- Plans save automatically in your browser (localStorage), so there is no account or server

## Run it

Open `index.html` in a browser, or visit the GitHub Pages site.
The Excel and PDF builders (ExcelJS and jsPDF) load from cdnjs, so exports need an internet connection.

## Deploy to GitHub Pages

1. Push this folder to a GitHub repo.
2. In the repo, go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, pick `main` and `/ (root)`, then click **Save**.
4. After a minute the site is live at `https://<your-username>.github.io/<repo-name>/`.

## Files

| File | What it is |
| --- | --- |
| `index.html` | The whole app: HTML, CSS and JavaScript |
| `sample.json` | Sample plan used by the "Try a sample plan" button (enVision Math Grade 5, Lessons 2-4 and 2-5) |

## Credits

Made by Cole Eggly, based on his Lesson Planner Claude skill. Built with help from Claude.
