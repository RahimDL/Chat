Fixed package conflict for GitHub Actions APK build.
Use the included .github/workflows/build-apk.yml.
It builds apps/super_up_app with Flutter 3.35.1 and uploads debug APK artifact.
Main fix: v_chat_room_page meta downgraded from ^1.17.0 to ^1.16.0 and app dependency_overrides includes meta ^1.16.0.
Old android/local.properties and key.properties were removed because they contain local Mac paths/signing data and break cloud builds.
