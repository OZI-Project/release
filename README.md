# OZI Release

Build python package releases with OZI in GitHub actions.

## Inputs

* python-dist - dist version string e.g. security2, security1, bugfix, prerelease - required
* github-token - workflow-generated token - optional
* freethreaded - enable freethreaded python builds when applicable (Python >= 3.13) - optional
* wheel-sign-token - to sign wheel RECORD.jws - optional

Also expects an artifact named ``security2`` with a drafted release from [OZI Draft](https://github.com/marketplace/actions/ozi-draft).

## Outputs:

* hashes - release file hashes in base64

## Permissions

Use the following:

```yaml
    permissions:
      contents: write
      id-token: write
```
