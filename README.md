# Go Fork Yourself

### How to copy a local repo and make a new GitHub repo from it.

* Copy the local repo. Note that you should probably rename the directory while copying it, and that you should be moving it from wherever it was into the correct term/week directory!

    ```bash
    cp -r [path to local directory] [path to new directory]
    ```

    Note that the name of the directory doesn't matter to git, which doesn't care if you name your directory "Bruce Wayne" but the repo name is "Batman". Git doesn't know anything _at all_ about the filesystem beyond what's in the folder it's in!

* Create the GitHub repo, making sure NOT to check "create a README" this time. Name it whatever you want!

* Change the `remote`, which is how git knows where to upload to. Use the url from your address bar on GitHub, or from the directions GitHub gives you when you create a no-README repo, or just... know it's _always_ going to be https://github.com/[your username]/[your repo name].

    ```bash
    git remote set-url origin [your github url]
    ```

* Now you can make changes however you want, adding and committing just like always, but when you need to push up, *for the first time only*, you'll need to tell it where to push to, like so:

    ```bash
    git push -u origin master
    ```
---
And you're done!
