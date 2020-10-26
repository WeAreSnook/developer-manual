# Branches

## Use main as your base branch

As the Internet Engineering Task Force (IETF) outline, master-slave naming conventions are outdated and oppressive language.

When you create repositories from Snook's Github UI, the base branch will default to `main`. However when you you create a new git repo locally, git (usually) defaults to naming the main branch as `master`.

> Run `git config --global init.defaultBranch main` to always set your base git branch to main.

## How to work with branches

Branches are _yours_. You can do what you like to them – including [force pushing](https://git-scm.com/docs/git-push#git-push---force-with-leaseltrefnamegt) unless you've agreed with someone else that you won't.

This makes it easy to help your fellow developers by [rewriting](http://git-scm.com/book/en/Git-Tools-Rewriting-History) your commits regularly so that they make logical sense. You can use `git rebase --interactive` to do this.

Although it's sometimes hard to be disciplined, prefer smaller commits, which can be squashed together later. It's harder to break large commits up into smaller ones.

Smaller commits make git tools like `annotate` and `log` more useful. They also increase the chance that the commit can be useful on its own. This is frequently useful when you're working in parallel with another developer on a separate branch and you both need early access to the same work. It makes [cherry-picking](https://git-scm.com/docs/git-cherry-pick) much easier.

Pushes to main should be for absolute emergency [hotfixes](https://en.wikipedia.org/wiki/Hotfix) only, and with the agreement of one or more other members of the team.
