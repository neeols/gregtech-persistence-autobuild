# GregTech Persistence Autobuild

This repository automatically checks the latest commits of:

https://github.com/Quantum-Studios-MC/GregTech-Persistence

If a new commit is found, it:

- clones the repository
- builds the mod jar with Gradle
- creates a GitHub release
- updates the stored built commit in `latest_commit`

## Files

- `.github/workflows/build.yml` — GitHub Actions workflow
- `latest_commit` — stores the last built upstream commit hash