framework for building agentic apps in JavaScript, Go, Dart, and Python, built and used in production by Google
genxnext-android/
├── build.gradle
├── settings.gradle
├── gradle.properties
├── keystore/
│   └── myProject_keyAndCertBundle_2.jks
└── app/
    ├── build.gradle
    ├── proguard-rules.pro
    └── src/
        └── main/
            ├── AndroidManifest.xml
            └── res/
                ├── values/
                │   └── strings.xml
                └── mipmap-hdpi/
                └──ic_launcher.png
Google Play & Firebase App Bundle Deployment Guide
​Artifact: app/build/outputs/bundle/release/app-release.aab
Package Name: online.genxnext.app
Target Platform: Google Play Console & Firebase App Distribution
​1. Local Pre-Flight Verification
​Before uploading, verify the integrity, signature, and metadata of your generated bundle.
​Step 1.1: Verify Keystore Signature
​Ensure the .aab is signed with the expected release key and not a debug certificate:# online.genxnext.app


 
