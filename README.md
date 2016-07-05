Official HC fork of Docker's official images repository.

Initial setup:

1. Clone this repository as `origin`
2. Add `https://github.com/docker-library/official-images` as `upstream`
3. Create a project-specific branch, e.g. `consul` or `vault`

When making a new PR:

1. From the project-specific branch, `git remote update` and `git rebase upstream/master`
2. Commit your changes and push to the project-specific branch in `upstream`
3. Send a PR to the official Docker repository
