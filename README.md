# About

A Personalized cookiecutter template based on [Cookiecutter Django](https://github.com/cookiecutter/cookiecutter-django)

# Features

1. Provides and option to unbundle Traefik
2. Fix issues related to unnamed docker volumes in the upstream template
3. Fix issue related to missing DATABASE_URL
4. Provide a staging environment to mock the production build on local machine
5. Reordered defaults to my liking

## Usage

Let's pretend you want to create a Django project called "redditclone". Rather than using `startproject`
and then editing the results to include your name, email, and various configuration issues that always get forgotten until the worst possible moment, get [cookiecutter](https://github.com/cookiecutter/cookiecutter) to do all the work.

First, get Cookiecutter. Trust me, it's awesome:

    uv tool install "cookiecutter>=1.7.0"

Now run it against this repo:

    uvx cookiecutter https://github.com/plktagrawal/cookiecutter-django-ninja.git

You'll be prompted for some values. Provide them, then a Django project will be created for you.

## Updating the main branch:

The `upstream` branch is the fork of [Cookiecutter Django](https://github.com/cookiecutter/cookiecutter-django)

The `main` branch contains my commits to the upstream code.

To update the main branch to the latest changes in upstream:

1. Update the `upstream` branch by pulling changes from [Cookiecutter Django](https://github.com/cookiecutter/cookiecutter-django)

2. Switch to `main` branch

3. Rebase `main` branch

```sh
git rebase myupstream
```

4. Push changes to github
