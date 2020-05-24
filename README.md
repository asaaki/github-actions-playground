# github-actions-playground

Playing with GitHub Actions

## Generate a short SHA env var for usage in jobs/steps

Since `::set-env` doesn't seem to work reliably across steps,
let alone jobs, we need to use a tiny trick:
Let's use a dedicated job for a more globally usable variable.

Take a look at [ci.yml](./.github/workflows/ci.yml)
