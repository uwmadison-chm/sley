# Reference repositories

This directory holds clones of *other people's* repositories that we consult while designing Sley -- specs, related tools, prior art. Nothing here is ours, so nothing here is committed: `.gitignore` excludes everything in `reference/` except this README.

To consult a repo, clone it here and add a line to the table below so the next person (or the next agent) can re-create the same working set.

## Repos

| Directory | Upstream | Why we care |
| --- | --- | --- |
| `tidyverse-style` | https://github.com/tidyverse/style.git | The tidyverse style guide. Source of truth for R naming, formatting, and file organization conventions. |
| `r-pkgs` | https://github.com/hadley/r-pkgs.git | *R Packages* (Wickham & Bryan). Package structure, testing, documentation, and release practice. |
| `r-for-data-science` | https://github.com/hadley/r4ds.git | *R for Data Science* (Wickham, Çetinkaya-Rundel & Grolemund). Tidy data principles and the data-wrangling idioms researchers will already know. |

## Re-creating this directory

Shallow clones are fine -- we read these, we don't develop in them.

```sh
cd reference
git clone --depth 1 https://github.com/tidyverse/style.git tidyverse-style
git clone --depth 1 https://github.com/hadley/r-pkgs.git r-pkgs
git clone --depth 1 https://github.com/hadley/r4ds.git r-for-data-science
```

## Notes

- Keep clones read-only in practice. If you need to experiment in one, fork it and work elsewhere.
- Because these are ignored, `git add -A` will not accidentally record them as bare gitlinks (submodule stubs).
- If a reference repo becomes a real dependency rather than reading material, it belongs in the project's dependency configuration, not here.
