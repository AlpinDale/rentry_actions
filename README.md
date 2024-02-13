## Github actions for Rentry

This repository contains a template for automatically creating and/or managing [rentry](https://rentry.co) pages through GitHub.

### Usage

Fork this repository, then add a [GitHub Secret](https://docs.github.com/en/actions/security-guides/using-secrets-in-github-actions) titled `RENTRY_PASSWORD`. This will be the password used to edit and create new rentries. Make sure you don't share this with anyone.

Then create a new `.md` file in the `src` directory, and add the following header:

```
---
some_url
---
```

Then follow it with your markdown content. The URL specified there must be unique, as it'll be the URL for the created rentry. e.g., the example above would create a new page under `https://rentry.co/some_url`.

### Why
Rentry doesn't have issues or pull requests, this should help with that I think.