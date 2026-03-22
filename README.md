Notes:
- Root required. For non-rooted users, please use VPhonegaga.
- This tool only removes pairip from dex. If there is still pairip in the libs, you need to replace or patch the lib manually
  
See: replace lib tutorial.
Before trying this, I recommend downloading an older version of the app and checking its native libs. Sometimes, older versions still use the same libs without pairip and you can replace the current ones with those. You can also check other apps that use the same libs without pairip.

If you can’t find any, you can follow this video to identify which lib is being used, and build a simple app that includes the same dependency to get a clean version of the lib without pairip.

Fortunately, in most cases, the lib that contains pairip is not from the app developer’s own code, but from a third-party dependency, so you can rebuild the lib yourself without pairip.

Requirements:
Java 17 or later

Usage:
java -jar Pairip.jar -i example.apks

For translation:
java -jar Pairip.jar -i example_merged.apk -t pairip.json
