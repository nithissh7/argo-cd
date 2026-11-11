# ZDH-010 Proof of Concept

This file was created by an attacker who:
1. Submitted a PR with a crafted git user.name containing $(cmd)
2. A maintainer merged the PR and added a cherry-pick label
3. The cherry-pick workflow expanded $(cmd) in an unquoted heredoc
4. The attacker captured the workflow token (GH_TOKEN)
5. Used the token to push this file to the repository

This demonstrates full repository write access from a commit message injection.
