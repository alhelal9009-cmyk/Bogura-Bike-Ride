name: Build Android APK

on:
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout
        uses: actions/checkout@v4

      - name: Extract project ZIP
        run: |
          unzip -o BoguraBikeRide-BuildReady.zip
          cd BoguraBikeRide
          chmod +x gradlew

      - name: Build APK
        working-directory: BoguraBikeRide
        run: ./gradlew assembleDebug

      - name: Upload APK
        uses: actions/upload-artifact@v4
        with:
          name: BoguraBikeRide-APK
          path: BoguraBikeRide/app/build/outputs/apk/debug/*.apk
