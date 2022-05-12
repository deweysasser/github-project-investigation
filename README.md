# github-project-investigation

Tools to investigate github projects

## fetch-prs -- fetch all open project PRs and summarize them

Example

```
./fetch-prs git@github.com:kubernetes/kubernetes.git
```

This will clone the given repo, examine all of the open PRs and arrange to fetch each locally, then 
create an index of all commits on each PR and leave them in the `manifests` directory.

It will then summarize the PRs and print the top contributors.

The resulting (bare) git repository will be left with a branch for each PR.