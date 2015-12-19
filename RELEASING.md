# Releasing

 1. Update the version in `build.gradle` to a non-SNAPSHOT version.
 2. Update the `CHANGELOG.md` for the impending release.
 3. Update the `README.md` with the new version.
 4. Update `library_betterimageview_strings.xml` with the new version.
 5. `git commit -am "Prepare for release X.Y.Z"` (where X.Y.Z is the new version)
 6. `./gradlew clean install bintrayUpload`
 7. `git tag -a X.Y.Z -m "Version X.Y.Z"` (where X.Y.Z is the new version)
 8. Update the version in `build.gradle` to the next SNAPSHOT version.
 9. `git commit -am "Prepare next development version"`
 10. `git push && git push --tags`
