README for ynot

### REST API endpoints for repository contents

Use the REST API to create, modify, and delete Base64 encoded content in a repository.

use **get /repos/{owner}/{repo}/contents/{path}** where

-   owner: fischerpj

-   repo: ynot

-   path: README.md

    =\> get /repos/**fischerpj**/**ynot**/contents/**README.md**

-   curl -L \\ -H "Accept: application/vnd.github+json" \\ -H "Authorization: Bearer \<YOUR-TOKEN\>" \\ -H "X-GitHub-Api-Version: 2022-11-28" \\ https://api.github.com/repos/OWNER/REPO/contents/PATH

-   curl -L \\ -H "Accept: application/vnd.github+json" \\ -H "Authorization: Bearer \<YOUR-TOKEN\>" \\ -H "X-GitHub-Api-Version: 2022-11-28" \\ https://api.github.com/repos/**fischerpj**/**ynot**/contents/README.md

-   JS // Octokit.js // https://github.com/octokit/core.js#readme const octokit = new Octokit({ auth: 'YOUR-TOKEN' })

    await octokit.request('GET /repos/{owner}/{repo}/contents/{path}', { owner: 'OWNER', repo: 'REPO', path: 'PATH', headers: { 'X-GitHub-Api-Version': '2022-11-28' } })

[ynot/README.md at main · fischerpj/ynot (github.com)](https://github.com/fischerpj/ynot/blob/main/README.md)

### ...or create a new repository on the command line

```         
echo "# ynot" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/fischerpj/ynot.git
git push -u origin main
```

### ...or push an existing repository from the command line

```         
git remote add origin https://github.com/fischerpj/ynot.git
git branch -M main
git push -u origin main
```
