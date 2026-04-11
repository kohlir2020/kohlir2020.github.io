# Personal Website - Raunit Kohli

A fun little portfolio website built with the assistance of ChatGPT Agent Mode (Oct 2025) and Github Copilot (Claude Sonnet 4 - Oct 2025, Claude Opus 4.6 - April 2026).

## Running Locally

```bash
bundle install
bundle exec jekyll serve
```

Then open [http://localhost:4000](http://localhost:4000) in your browser.

## Updating the Resume

The resume is built from a LaTeX source file at `assets/rk_resume.tex`. To update it:

1. Edit `assets/rk_resume.tex`
2. Compile the PDF:
   ```bash
   cd assets
   pdflatex rk_resume.tex
   ```
3. Clean up build artifacts (optional):
   ```bash
   rm -f rk_resume.aux rk_resume.log rk_resume.out
   ```
4. Commit and push both files:
   ```bash
   cd ..
   git add assets/rk_resume.tex assets/rk_resume.pdf
   git commit -m "Update resume"
   git push
   ```

**Requires:** A LaTeX distribution — install via `brew install --cask basictex` on macOS.