You can run the following commands _in the order shown_ to clean your project, if the plugin is not running as expected:
* `./gradlew --stop` which stops the gradle daemon
* `rm -rf ~/.m2 ~/.gradle` (or just `rm -rf ~/.gradle/caches/`)
* `File -> Invalidate Caches / Restart...`. If you run the project afterwards, it should automatically download the dependencies and set up intellisense.
* `./gradlew clean`
* Click the gradle refresh button in the side panel to re-download the dependencies
