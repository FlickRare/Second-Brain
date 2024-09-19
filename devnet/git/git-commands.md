# git commands
| Purpose                                                         | Command                    | Notes & Flags                                                 |
|-----------------------------------------------------------------|----------------------------|---------------------------------------------------------------|
| Display the state of the working dir and staging area           | git status                 |                                                               |
| Lists commits in reverse chronological order                    | git log                    | --all ensures all refs/ and HEAD are listed as well           |
| Add altered files to staging area ahead of commit               | git add                    | "git add ." adds all changed made within the dir              |
| Reset staging area                                              | git reset HEAD             |                                                               |
| Save changed from staging area to the repo                      | git commit                 | -m "$message" to bypass text edit for simpler commits         |
| Revert the repo to a previous version (version control!)        | git reset ($sha1)          | "$sha1" = the ID of specfic commit you want ot revert to      |
| Add your changes to a remote repo (github?)                     | git push                   |                                                               |
| Set the location of the remote repo for current instance of git | git remote add origin $url | "$url" = url of remote repository (click green "code" button) |
| Download a remote repository                                    | git clone $url             | $url = url of remote repository                               |