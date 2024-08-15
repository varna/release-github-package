# How to release a package in GitHub

1. Copy `.github/workflows/npm-publish-github-packages.yml`
2. Make sure that `package.json` is correct:

```json
{
  "name": "@username/repo-name",
  "repository": {
    "type": "git",
    "url": "https://github.com/username/repo-name.git"
  },
  "publishConfig": {
		"registry": "https://npm.pkg.github.com/"
	}
}
```
