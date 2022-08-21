# To-Do

## `0.0.0`

1. Local setup
   - Replace `project-name` with project name (don't forget to skip this line :wink:)
     - Run `yarn` afterwards to update lockfile
   - Commit scopes
     - Update [`.commitlintrc.ts`](.commitlintrc.ts)
   - Label management
     - Update [`.github/labels.yml`](.github/labels.yml)
   - Package details
     - Update [`package.json#author`](package.json#L17-L20)
     - Update [`package.json#description`](package.json#L3)
     - Update [`package.json#keywords`](package.json#L5)
     - Review [`package.json#publishConfig`](package.json#L21-L23)
   - Preliminary documentation
     - Review [contributing guide](CONTRIBUTING.md)
     - Update project description in [`README`](README.md)
     - Update [project license](LICENSE.md)
       - Sync [`package.json#license`](package.json#L8)
   - Release management
     - Check [`package.json#tagPrefix`](package.json#L140)
   - Review @dependabot configuration
     - [`.github/dependabot.yml`](.github/dependabot.yml)
   - Review Yarn configuration
     - [`.yarnrc.yml`](.yarnrc.yml)
       - Update [workflow](.github/workflows/) environments and permissions
   - `git launchwithinit gh:flex-development/<project-name>`
2. Repo Settings
   - [ ] General
     - [ ] Features
       - [ ] Issues
       - [ ] Projects
       - [ ] Discussions
     - [ ] Pull requests
       - [ ] Do **NOT** allow merge commits
       - [ ] Allow squash merging
         - [ ] Default to pull request title
       - [ ] Allow rebase merging
       - [ ] Always suggest updating pull request branches
       - [ ] Allow auto-merge
       - [ ] Do **NOT** automatically delete head branches
   - [ ] Code and automation
     - [ ] Branches
       - [ ] Add branch protection rule matching `main`
         - [ ] Protect matching branches
           - [ ] Require a pull request before merging
             - [ ] Require at least `1` approval
             - [ ] Dismiss stale pull request approvals
           - [ ] Require status checks to pass before merging
             - [ ] Require branches to be up to date before merging
               - [ ] GitGuardian Security Checks
               - [ ] ci
           - [ ] Require conversation resolution before merging
           - [ ] Require signed commits
           - [ ] Require linear history
     - [ ] Security
       - [ ] Secrets
         - [ ] Action secrets
         - [ ] Dependabot secrets
3. `git ac 'chore: complete repo setup' && git push`
