# Meteor Autobuild Template

This template builds off of https://github.com/MeteorDevelopment/meteor-addon-template, adding the following:
- Branches for Minecraft versions `1.21.4`, `1.21.3`, `1.21.1`, and `1.20.4`.
- GitHub workflows to automatically build release jars for each version in repository releases on commit.
- GitHub workflow to attempt to automatically backport by rebasing all previous versions onto the default branch (run manually).
    - If merge conflicts are present in `src/main/*`, the rebase is aborted
    - If merge conflicts are present in any other file (e.g. `gradle.properties`), the original branch's version is accepted.

## License

This template is available under the CC0 license. Feel free to use it for your own projects.
