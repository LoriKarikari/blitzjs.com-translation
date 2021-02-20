# blitzjs.com Translation

This repo contains resources and scripts to enable translations of https://blitzjs.com.

## Contributing to translations

Check www.isreacttranslatedyet.com to see if your language already has a translation effort in progress. Click on "Track Progress" on the language you want to contribute to in order to receive further instructions.

## Starting a new translation

If you would like to be the maintainer of a new translation, submit a PR adding a new file `{lang-code}.json`
to the `langs` folder with the following information:

* Language name (in English please)
* [Language code](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes)
* List of maintainers

For example:

```json
{
  "name": "Spanish",
  "code": "es",
  "maintainers": ["juanm04", "ntgussoni"]
}
```

In the PR comment, please describe your experiences with translation (e.g. links to previous work). We prefer more than one maintainer on each repo, so if you're by yourself, we'll leave the PR open for others to join in. If you are a group, please have at least one person other than the PR opener comment, to make sure all people listed actually want to be part of the translation!

Also, please read the [Maintainer Responsibilities](/maintainer-guide.md#maintainer-responsibilities) and make sure that you are comfortable with the responsibilities listed.

Once the PR is accepted, the bot will:

* Create a new repository for you at `blitz-js/{lang-code}.blitzjs.com`
* Add/invite all maintainers listed to the repository
* Create an issue from [PROGRESS.template.md](/PROGRESS.template.md) in the new repository to track your translation progress

You may want to [pin](https://help.github.com/articles/pinning-an-issue-to-your-repository/) the generated issue to make it easier to find.

See [Maintainer Tips](/maintainer-guide.md/#tips) for additional advice on how to manage your repository.

Happy translating!

## Adding a maintainer

If you are currently a maintainer of a translation and want to add another member, send a pull request to this repo updating `langs/{lang-code}.json`, where `{lang-code}` is the language code of the repo you want to be a maintainer of.

If you are interested in becoming a maintainer for a translation, please ask one of the current maintainers if they would like to add you. While different maintainers can have different requirements, usually they look for people who have already contributed to the translation already, either by translating or reviewing.

## Before publishing

1. Review your translations and make sure that the pages listed in "Core Pages" are fully translated. Run the site yourself locally to make sure there are no bugs or missing translations.
2. ask {TBD} to add {lang-code}.blitzjs.com as a subdomain.
3. submit a PR to [blitz-js/blitzjs.com](https://github.com/blitz-js/blitzjs.com) adding the language in the dropdown and the welcome message.
4. Celebrate! 🎉🌐

## Acknowledgements

This repo, and the bot that makes all this possible, is based off of and iterated upon [reactjs.org-translation](https://github.com/reactjs.org/reactjs.org-translation).
