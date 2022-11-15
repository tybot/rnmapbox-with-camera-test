1. `npm install`
2. `npx eas build -p android` (using EAS Build)
   - configure EAS Build using prompts
   - build succeeds
3. `npx expo install expo-camera`
4. `npx eas build -p android`
   - build fails at `Run gradlew`:

```
[stderr] FAILURE: Build failed with an exception.
[stderr] * Where:
[stderr] Build file '/home/expo/workingdir/build/android/build.gradle' line: 40
[stderr] * What went wrong:
[stderr] A problem occurred evaluating root project 'mapbox-build-test'.
[stderr] > Could not find method maven() for arguments [build_a4pmw2504rhdm3lg68kv7pbd1$_run_closure1$_closure3@4911148e] on root project 'mapbox-build-test' of type org.gradle.api.Project.
```
