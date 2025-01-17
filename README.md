# Expo Android Build Failure: Resource Not Found

This repository demonstrates a bug in the Expo CLI Android build process where a 'resource not found' error occurs despite resources being present in the project. The build fails with an error message indicating that a required resource is missing, even though it's included in the project files. This problem arises from inconsistencies between the AndroidManifest.xml, build.gradle files, and project resources. Incorrect build variants, missing dependencies, or incorrect resource paths can cause this issue.

## Steps to Reproduce

1. Clone this repository.
2. Install the necessary dependencies (follow instructions in package.json).
3. Attempt to build an Android APK using `expo build:android`.
4. Observe the build failure with the 'resource not found' error message.

## Solution

This error typically requires careful examination of the AndroidManifest.xml file, build.gradle files, and resources to identify the inconsistency.  The provided solution file in this repo fixes a common cause of the problem which often is due to build variant inconsistencies. Thoroughly review the build configuration files to ensure they are properly set up and match the resources that are available in your project.