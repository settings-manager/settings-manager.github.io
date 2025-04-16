# Configuration

## Repository

### description

Short description of the repository.

Example:
```yaml
repository:
  description: Repository description goes here
```

### homepage

URL with more information about the repository.

Example:
```yaml
repository:
  homepage: https://example.com
```

### private

Either `true` to make the repository private or `false` to make it public.

Example:
```yaml
repository:
  private: false
```

### security\_and\_analysis

Specify which security and analysis features to enable or disable for the
repository.

Example:
```yaml
repository:
  security_and_analysis:
    advanced_security:
      status: enabled
    code_security:
      status: enabled
    secret_scanning:
      status: enabled
    secret_scanning_push_protection:
      status: disabled
    secret_scanning_ai_detection: 
      status: disabled
    secret_scanning_non_provider_patterns:
      status: disabled
```

### has\_issues

Either `true` to enable issues for this repository or `false` to disable them.

Example:
```yaml
repository:
  has_issues: false
```

### has\_projects

Either `true` to enable projects for this repository or `false` to disable
them.

Example:
```yaml
repository:
  has_projects: false
```

### has\_wiki

Either `true` to enable the wiki for this repository or `false` to disable
it.

Example:
```yaml
repository:
  has_wiki: false
```

### is\_template

Either true to make this repo available as a template repository or false to
prevent it.

Example:
```yaml
repository:
  is_template: true
```

### default\_branch

Updates the default branch for this repository.

Example:
```yaml
repository:
  default_branch: develop
```

### allow\_squash\_merge

Either `true` to allow squash-merging pull requests, or `false` to prevent
squash-merging.

Example:
```yaml
repository:
  allow_squash_merge: true
```

### allow\_merge\_commit

Either `true` to allow merging pull requests with a merge commit, or `false` to
prevent merging pull requests with merge commits.

Example:
```yaml
repository:
  allow_merge_commit: false
```

### allow\_rebase\_merge

Either `true` to allow rebase-merging pull requests, or `false` to prevent
rebase-merging.

Example:
```yaml
repository:
  allow_rebase_merge: false
```

### allow\_auto\_merge

Either `true` to allow auto-merge on pull requests, or `false` to disallow
auto-merge.

Example:
```yaml
repository:
  allow_auto_merge: true
```

### delete\_branch\_on\_merge

Either `true` to allow automatically deleting head branches when pull requests
are merged, or `false` to prevent automatic deletion.

Example:
```yaml
repository:
  delete_branch_on_merge: true
```

### allow\_update\_branch

Either `true` to always allow a pull request head branch that is behind its
base branch to be updated even if it is not required to be up to date before
merging, or `false` otherwise.

Example:
```yaml
repository:
  allow_update_branch: true
```

### squash\_merge\_commit\_title

Required when using squash\_merge\_commit\_message.

The default value for a squash merge commit title:

- **PR_TITLE**: default to the pull request's title.
- **COMMIT_OR_PR_TITLE**: default to the commit's title (if only one commit) or the pull request's title (when more than one commit).

```yaml
repository:
  squash_merge_commit_title: PR_TITLE
```

### squash\_merge\_commit\_message

The default value for a squash merge commit message:

- **PR_BODY**: default to the pull request's body.
- **COMMIT_MESSAGES**: default to the branch's commit messages.
- **BLANK**: default to a blank commit message.

```yaml
repository:
  squash_merge_commit_message: PR_BODY
```

### merge\_commit\_title

Required when using merge\_commit\_message.

The default value for a merge commit title.

- **PR_TITLE**: default to the pull request's title.
- **MERGE_MESSAGE**: default to the classic title for a merge message (e.g., Merge pull request #123 from branch-name).

```yaml
repository:
  merge_commit_title: PR_TITLE
```

### merge\_commit\_message

The default value for a merge commit message.

- **PR_TITLE**: default to the pull request's title.
- **PR_BODY**: default to the pull request's body.
- **BLANK**: default to a blank commit message.

```yaml
repository:
  merge_commit_message: PR_BODY
```

### archived

Whether to archive this repository. `false` will unarchive a previously
archived repository.

```yaml
repository:
  archived: true
```

### allow\_forking

Either `true` to allow private forks, or `false` to prevent private forks.

```yaml
repository:
  allow_forking: false
```

### web\_commit\_signoff\_required

Either `true` to require contributors to sign off on web-based commits, or
`false` to not require contributors to sign off on web-based commits.

```yaml
repository:
  web_commit_signoff_required: true
```
