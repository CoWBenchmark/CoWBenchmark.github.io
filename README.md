# CoWBenchmark.github.io
Circle of Willis Benchmarking Event 2023

Powered by Jekyll with the [al-folio](https://github.com/alshedivat/al-folio) theme.

* Modified from https://github.com/XR4biomed
* Images by unsplash (Photo by <a href="https://unsplash.com/@kocheva?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Polina Kocheva</a> on <a href="https://unsplash.com/photos/oazfJJL9N1A?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Unsplash</a>
  )

## Local build and test

```bash
bundle install
bundle exec jekyll serve
```

`bundle install` has error for `An error occurred while installing mini_racer (0.6.3)`

possible workaround:
- Installing Node.Js (`node -v # v19.7.0`)
- Commented out `gem 'mini_racer'`

see github issue [libv8-node error](https://github.com/alshedivat/al-folio/issues/691)

## Update Content

Pages relevant for the content update (basically all in `_pages` dir):
- `_pages/*.md`
- `_config.yml`
- `_news/`
- later if needs to include publications, `_bibliography/papers.bib`

## GitHub Pages Deploy

If you encounter `Liquid Exception: Liquid syntax error`, that is likely due to the deploy branch not set to `gh-pages` on github
> "Finally, in the Settings of your repository, in the Pages section, set the branch to gh-pages (NOT to master). For more details, see Configuring a publishing source for your GitHub Pages site."

## References

https://www.youtube.com/watch?v=g6AJ9qPPoyc