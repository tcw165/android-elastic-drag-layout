Release Process
===

### Step 1

Update the `library_version` configuration in the `elastic-drag-layout/deploy.gradle` file.

### Step 2
Run the command

```
./gradlew clean build elastic-drag-layout:bintrayUpload
```