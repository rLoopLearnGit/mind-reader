# One time setup #
1. Setup global configuration and email
    1. Add username <code>git config --global user.name "John Doe"</code>
    1. Add email <code>git config --global user.email johndoe@example.com</code>
2. Setup github username and password, see [ Caching your github password in git ]( https://help.github.com/articles/caching-your-github-password-in-git/ )


# Developing a feature #
1. Fork the development branch, use the web interface
2. Clone the forked repository <code>git clone *link_to_your_forked_repo*</code>
3. Add the upstream repository <code>git remote add upstream *link_to_rLoop_repo*</code>
4. Add a development branch <code>git checkout -b development</code>
5. Update the development branch <code>git pull upstream development</code>
6. Create a feature branch <code>git checkout -b *feature_name*</code>
7. Add the feature
8. Ready changes for commit
    1. View the changed files <code>git status</code>
    2. View the changes to a file <code>git diff *filename*</code>
    3. Stage file for commit <code>git add *filename*</code>
    4. View lines staged for commit <code>git diff --cached</code>
9. Commit changes <code>git commit -m "*commit message*"</code>, See writing good commit messages
10. Push feature branch to rLoop repository <code>git push upstream *feature_name*</code>
11. Create a pull request
    1. Add assignees @lochlon, @david
    2. Add a commit message
    - [x] Complies with code_standards <!-- FIXME: add link --!>
    - [x] Doesn't introduce new bugs
    - [x] Fixes *some_issue*
    - [x] Other items
12. Once pull request has been accepted, update development branch <code>git pull --rebase upstream development</code>
13. Get the new development branch <code>git checkout development</code>
14. Update development branch <code>git pull upstream development</code>
15. Update development branch <ocde>git pull upstream development</code>
