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
4. Set repository's Secrets in Settings (see [docs](https://docs.github.com/en/actions/reference/encrypted-secrets#creating-encrypted-secrets-for-a-repository))
- `SH_USER`: Username of sourcehut
- `SH_TOKEN`: Generated PAT
5. Modified gmi docs and director(ies) in `./pub/gmi/`
6. CI works by pushing your commits to repo or running [manually](https://docs.github.com/en/actions/managing-workflow-runs/manually-running-a-workflow#running-a-workflow)
7. Deployed!

## Badges

```markdown
󠀭󠀭[![Deploy](https://github.com/{name}/{repo}/actions/workflows/deploy.yml/badge.svg)](https://github.com/{name}/{repo}/actions/workflows/deploy.yml)
[![Website](https://img.shields.io/website?label=HTTPS&url=https%3A%2F%2F{name}.srht.site)](https://{name}.srht.site)
```
