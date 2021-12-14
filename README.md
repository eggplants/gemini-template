# gemini-template

[See my sample repo](https://github.com/eggplants/gemini)

## WHAT?

- Publish [Gemtext](https://gemini.circumlunar.space/docs/gemtext.gmi) to sourcehut automatically:
  - `gemini://${USERNAME}.srht.site`
  - `https://${USERNAME}.srht.site`

## Step

1. [Fork me](https://github.com/eggplants/gemini/fork)
2. [Register sourcehut](https://meta.sr.ht/register)
3. [Generate OAuth2.0 Personal Token](https://meta.sr.ht/oauth2/personal-token)
4. Set generated PAT `PH_TOKEN` of repository's Secrets in Settings (see [docs](https://docs.github.com/en/actions/reference/encrypted-secrets#creating-encrypted-secrets-for-a-repository))
5. Modified gmi docs and director(ies) in `./pub/gmi/`
6. Change [USERNAME](https://github.com/eggplants/gemini/blob/bff21010c6b49f9e7b50b50a94cd86316261a88d/.github/workflows/deploy.yml#L37) into yours
7. CI works by pushing your commits to repo or running [manually](https://docs.github.com/en/actions/managing-workflow-runs/manually-running-a-workflow#running-a-workflow)
8. Deployed!

## Badges

```markdown
󠀭󠀭[![Deploy](https://github.com/{name}/{repo}/actions/workflows/deploy.yml/badge.svg)](https://github.com/{name}/{repo}/actions/workflows/deploy.yml)
[![Website](https://img.shields.io/website?label=HTTPS&url=https%3A%2F%2F{name}.srht.site)](https://{name}.srht.site)
```
