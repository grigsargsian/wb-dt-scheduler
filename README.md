# WB DT scheduler

This public repository contains only the GitHub Actions timers for the private **WB by Grigor** site.

- `wb-dt-check.yml` requests a short-lived GitHub OIDC token and calls the public relay about every five minutes.
- `scheduler-keepalive.yml` records harmless monthly repository activity so GitHub does not disable the public-repository schedule after 60 inactive days.
- No WB API key, Sites bypass token, DT secret, order data, or product data is stored here.

The relay accepts tokens only from this repository's immutable GitHub identity, the `main` branch, and the exact scheduler workflow.
