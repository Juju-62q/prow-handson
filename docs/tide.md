# Tide
* マージの自動化

# 機能

## 例
```
tide:
  merge_method:
    kubeflow/community: squash

  target_url: https://prow.k8s.io/tide.html

  queries:
  - repos:
    - kubeflow/community
    - kubeflow/examples
    labels:
    - lgtm
    - approved
    missingLabels:
    - do-not-merge
    - do-not-merge/hold
    - do-not-merge/work-in-progress
    - needs-ok-to-test
    - needs-rebase

  context_options:
    # Use branch protection options to define required and optional contexts
    from-branch-protection: true
    # Treat unknown contexts as optional
    skip-unknown-contexts: true
    orgs:
      org:
        required-contexts:
        - "check-required-for-all-repos"
        repos:
          repo:
            required-contexts:
             - "check-required-for-all-branches"
            branches:
              branch:
                from-branch-protection: false
                required-contexts:
                - "required_test"
                optional-contexts:
                - "optional_test"
```

## Tideの設定
