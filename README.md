# Personal Website - Raunit Kohli

A fun little portfolio website built with the assistance of ChatGPT Agent Mode (Oct 2025) and Github Copilot (Claude Sonnet 4 - Oct 2025, Claude Opus 4.6 - April 2026).

## Running Locally

```bash
bundle install
bundle exec jekyll serve
```

Then open [http://localhost:4000](http://localhost:4000) in your browser.

## Updating the Resume

The resume and CV are built from LaTeX source files. To update:

1. Edit `assets/rk_resume.tex` (1-page industry resume) or `assets/rk_cv.tex` (multi-page academic CV)
2. Compile the PDFs:
   ```bash
   cd assets
   pdflatex rk_resume.tex
   pdflatex rk_cv.tex
   ```
3. Clean up build artifacts (optional):
   ```bash
   rm -f rk_resume.aux rk_resume.log rk_resume.out rk_cv.aux rk_cv.log rk_cv.out
   ```
4. Commit and push:
   ```bash
   cd ..
   git add assets/rk_resume.tex assets/rk_resume.pdf assets/rk_cv.tex assets/rk_cv.pdf
   git commit -m "Update resume"
   git push
   ```

**Content provenance:** See `assets/content_provenance.md` for a line-by-line audit of every bullet on the resume/CV with source citations.

**Requires:** A LaTeX distribution — install via `brew install --cask basictex` on macOS.