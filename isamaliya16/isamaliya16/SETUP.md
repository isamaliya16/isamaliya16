# Setup Guide (delete this file from the repo once you're done, or keep it, it's optional)

## Which files matter?

| File | Needed? | Purpose |
|---|---|---|
| `README.md` | **Required** | The profile page itself |
| `assets/banner.svg` | **Required** | Top and animated banner |
| `assets/profile-animation.svg` | Recommended | About-section illustration |
| `assets/section-divider.svg` | Recommended | Animated dividers |
| `assets/project-banners/*.svg` | Recommended | Project cards |
| `.github/workflows/update-profile.yml` | Optional | Daily contribution snake |
| `LICENSE` | Optional | MIT license |
| `SETUP.md` | Optional | This guide |

## Update your existing repo (isamaliya16/isamaliya16)

```bash
git clone https://github.com/isamaliya16/isamaliya16.git
cd isamaliya16
# copy the new files from this package over the old ones (keep the .git folder!)
git add .
git commit -m "Redesign profile README"
git push origin main
```
(If your default branch is `master`, use that instead of `main`. If you prefer no terminal: open the repo on github.com, click **Add file -> Upload files**, drag everything in, and commit.)

## Turn on the snake animation (one-time)

1. Repo -> **Settings -> Actions -> General -> Workflow permissions** -> choose **Read and write permissions** -> Save.
2. Repo -> **Actions** tab -> **Update profile animations** -> **Run workflow**.
3. Wait about a minute. An `output` branch appears and the snake shows in your README.

## Things to EDIT (search README.md for "EDIT")

1. **Projects:** change the seven repo names/links to your real repositories, update the descriptions, and add demo links (or delete the "Demo" part).
2. **Connect:** replace `YOUR-LINKEDIN-ID`, `YOUR-EMAIL`, `YOUR-KAGGLE-ID`.
3. **Certifications:** add real certificates with verification links.
4. **Technology Stack:** remove anything you are not comfortable discussing.
5. **Fun Facts:** make them truly yours.
6. **Project banners:** the titles live in the SVG files; if you rename a project, edit the text in `assets/project-banners/0X-*.svg`.

## Final checklist

- [ ] Repo is named exactly `isamaliya16`, is **Public**, and README.md is in the root
- [ ] Banner, divider and project images all display (no broken icons)
- [ ] Typing animation plays
- [ ] All 7 project links open real repositories (no 404)
- [ ] LinkedIn / email / Kaggle placeholders replaced
- [ ] Stat cards load (if not, wait a minute, and the fallback links in the README still work)
- [ ] Snake workflow ran successfully (green tick in Actions) and the snake is visible
- [ ] Opened your profile on a phone: layout is readable
- [ ] Checked the profile in both light and dark GitHub themes
- [ ] No private or sensitive information is shown

## Notes

- Animations inside the SVG files (SMIL/CSS) play on GitHub because the SVGs are loaded as images. Scripts do not run, and none are used.
- Stat widgets (github-readme-stats, streak-stats, activity-graph, trophies, view counter) are free third-party services and can be slow or rate-limited. The README stays readable if they fail.
- Profile views count starts from zero when first loaded.
