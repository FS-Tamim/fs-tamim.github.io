# fs-tamim.github.io

Personal academic website of **Fahim Shakil Tamim**, Lecturer in CSE at IUBAT.
Live at https://fs-tamim.github.io/ - built with Jekyll (AcademicPages theme).

## Where to edit

| Page | Edit this file |
|---|---|
| Home | about/index.md (intro, links, news) |
| Research | research/index.md (interests, papers) |
| Teaching | teach/index.md (semesters, courses) |
| Education & Experience | education/index.md |
| Achievements & Skills | achievements/index.md |

- Each folder's _style.html holds that page's colors and spacing.
- Navbar, sidebar and page titles: assets/css/site-theme.css
- Menu links: _data/navigation.yml
- Name, photo, sidebar links: _config.yml (restart the server after editing)

## Run locally

    bundle install
    bundle exec jekyll serve --config _config.yml,_config.dev.yml

Then open http://localhost:4000

## Publish

    git add -A
    git commit -m "Update site"
    git push
