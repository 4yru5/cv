# cv

My CV in LaTeX. GitHub Actions rebuilds the PDF and the web version automatically
(layout based on [zeyu2001/cv](https://github.com/zeyu2001/cv)).

- **Download the PDF:** https://github.com/4yru5/cv/raw/main/cv.pdf
- **Web version:** https://4yru5.github.io/cv/

## How to edit

1. Open [`cv.tex`](cv.tex) on github.com and click the **pencil icon** (Edit this file).
2. Change the text inside the `{ }` braces. Leave the `\commands` alone.
3. Click **Commit changes…** and then **Commit changes** again.
4. About a minute later, the **Build CV PDF** workflow (see the **Actions** tab) commits
   an updated `cv.pdf` and refreshes the web version. Download it from the link above.

## Things to remember

- Write `&` as `\&` and `%` as `\%`. Otherwise LaTeX treats them as commands and the build fails.
- Write `--` for a dash, as in `Sep. 2023 -- Sep. 2024`.
- A new bullet point is a copy of an existing `\resumeItem{...}` line.
- If a build fails (red ✗ in the Actions tab), open the run to see the error,
  fix `cv.tex` and commit again. The previous `cv.pdf` stays in place until a build succeeds.
