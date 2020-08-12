Official HC fork of Docker's official images repository.

Initial setup:

1. Clone this repository with `git clone git@github.com:docker-library/official-images.git`
2. Rename the remote origin to `upstream` with `git remote rename origin upstream`
3. Add the HashiCorp fork of `docker-library/official-images` as the new origin 
with `git remote add origin https://github.com/hashicorp/docker-official-images`
4. `git checkout master` and `git pul`l to base your changes off the upstream master and avoid conflicts.
5. Create a new project named branch such as `git checkout -b consul-1.8.3`

When making a new PR:

1. From the project-specific branch, `git remote update` and `git rebase upstream/master`
2. Commit your changes and push the branch to the HashiCorp repo with `git push origin {BRANCH}`
3. Open a pull request against `https://github.com/docker-library/official-images` to update 
the official image from the new branch in our fork.
