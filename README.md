# Release Test Repository

A simple test repository for GitHub Actions automated release workflows.

## What it does

This repository automatically creates GitHub releases with version files when you push a new tag. It's designed to test automated release pipelines before implementing them in production.

## How it works

1. Push a tag starting with `v` (like `v1.0.0`)
2. GitHub Actions automatically triggers
3. Creates a release with the tag name
4. Generates a `version.txt` file with build information
5. Uploads the file as a release asset

## Usage

To create a new release:

```bash
git tag v1.0.0
git push origin v1.0.0
```

This will automatically create a "Release v1.0.0" with a downloadable version file.