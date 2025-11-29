## Test Results 

Run Android UI tests:
```bash
./gradlew :app:connectedDebugAndroidTest
```

Pull allure results from the emulator/device:
```bash
adb -s emulator-5554 pull /sdcard/Documents/allure-results .
```

Generate and open allure report: 
```bash
allure serve allure-results/
```

Remove allure results from the emulator/device:

```bash
adb -s emulator-5554 shell rm -rf /sdcard/Documents/allure-results
```