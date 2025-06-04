# OZI Release

Build python package releases with OZI in GitHub actions.

## Inputs

* python-dist - dist version string e.g. security1, security2, bugfix, prerelease - required
* github-token - workflow-generated token - optional
* freethreaded - enable freethreaded python builds when applicable (Python >= 3.13) - optional
* wheel-sign-token - to sign wheel RECORD.jws - optional

## Outputs:

* hashes - release file hashes in base64

## Permissions

Use the following:

```yaml
    permissions:
      contents: write
      id-token: write
```
