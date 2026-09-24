# DarkFactory

dark factory instructions for agentic software engineering. Brief and customized

------

## Before

* prepare a **vision.md** with the specs and requirements (is this spec-driven development?!)
* prepare a Git repo and clone it locally
* run your favorite harness (Codex, Claude Code, Pi ..)

## Prompt

```text
check `visions.md` and understand the goal. make a plan and implement everything described there. make decisions yourself and keep working until the whole vision is processed and we have a working product.

work directly on `main`. use git properly. atomic commits, conventional commit messages, semver. every commit bumps the patch version, major features bump the minor version. every commit must be green before commit and push. push continuously.

set up `localPipeline.sh` as early as possible, with all testing, linting, formatting, type/static checks, coverage, builds, and later e2e + docker checks. keep test coverage at least 95%. make github actions mirror the local pipeline and keep everything green.

write small reusable scripts for repetitive tasks. document all scripts properly.

first make the local version work, then dockerize it. add github actions for docker build and publish the image to ghcr.

use GPLv3. add the proper `LICENSE` file and copyright/license headers where appropriate.

update `README.md` with badges like in `cullendula` or `mylastfmplayer` under `~/repos` (or https://github.com/marcelpetrick/myLastFmPlayer). document setup, testing, pipeline, docker, and usage. include at least one real screenshot of the UI.

use unit, integration, and end-to-end tests where appropriate. do not skip requirements.

before finishing, run `/reviewBranch`, fix all issues, then run `/githubAbout`. do a final check against every item in `visions.md`, run the full local pipeline, make sure github actions are green, the docker image works, everything is pushed, and the working tree is clean.

only stop when you can really say the whole `visions.md` is done and the product works.
```

* press Enter, wait ..
