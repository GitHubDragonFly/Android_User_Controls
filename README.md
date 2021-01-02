# AndroidUserControls
A few relatively simple looking and somewhat customizable Android user controls.

All controls have been included in the "Gauge" screen of the [PhoneTest](https://github.com/GitHubDragonFly/PhoneTest) project, with minimum requirement of Android 4.1 (API level 16) while targeting Android 11 (API level 30).

# Functionality
- AngleIndicator
  - a control to indicate rotational position/angle, measured counterclockwise from the zero/home position.
  - zero/home position could be selected as either of East (0), North (90), West (180) or South (270).
  - designed to show -360 to 360 values and will reduce all other values to this range (use the CurrentValue() method to get the actual value).
  - could potentially be used as a weather vane since it can show the Direction suffix.
  - possibly use either Arc or Pie to sweep the angle for better visual appearance, see the screenshot.
  - it has publicly accessible methods: CurrentValue() for reading and setCurrentValue(newFloatValue) for writing.
- RoundGauge
  - a gauge control that could be used for miscelaneous measurements.
  - min/max values can be set individually.
  - it has publicly accessible methods: getGaugeCurrentValue() for reading and setGaugeCurrentValue(newFloatValue) for writing.
- LEDLight
  - a control that can be turned ON/OFF and Blink (which is of a higher order but will restore the last ON/OFF state once the blinking stops).
  - it has publicly accessible methods: isLED_ON() and isLED_Blink() for reading and setLED_ON(newBooleanValue) and setLED_Blink(newBooleanValue) for writing.

Screenshot is included in each control's folder.

# Install

All it should take is to:

- Add the control's java file to your app's src/main/java/com.e.whatever folder (copy-paste).
- Add the control's xml file to your app's src/main/res/values folder (copy-paste).
- Save it all, Sync with Gradle, Build/Rebuild Project, open one of your activity layout files and look for the new control under "Project".

# Licensing
These are all licensed under MIT License.

# Trademarks
Any and all trademarks, either directly on indirectly mentioned in any control, belong to their respective owners.
