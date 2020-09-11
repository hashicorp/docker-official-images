Official HC fork of Docker's official images repository.

Initial setup:

1. Clone this repository with `git clone git@github.com:hashicorp/docker-official-images.git`
2. Add the [official Docker repository](https://github.com/docker-library/official-images) this is forked from as a new `upstream` remote with `git remote add upstream https://github.com/docker-library/official-images`

When making a new PR:

1. Run `git remote update`, then `git checkout upstream/master` to base your changes off the upstream master to avoid conflicts.
2. Create a new release-specific branch such as `git checkout -b consul-1.8.3`
3. Commit your changes and push the branch to the HashiCorp repo with `git push origin ${BRANCH}`
4. Open a pull request against `https://github.com/docker-library/official-images` to update the official image from the new branch in our fork. (Clicking the `New Pull Request` button for your branch on https://github.com/hashicorp/docker-official-images/branches will set the upstream Docker repository as base by default.) 
