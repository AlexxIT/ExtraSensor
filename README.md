# Extra Sensor for Garmin

This Garmin Connect IQ DataField lets you add additional sensors to your workouts.

By default, Garmin watches record only one sensor of each type, for example, heart rate or distance. And that's enough for many users. But if you want to compare the readings from several sensors, this DataField is exactly what you need.

The number of external sensors you can connect is limited only by the capabilities of your Garmin devices. On modern models, this is up to 9 ANT sensors and 3 BLE sensors.

Currently supported:

- ANT+ and BLE Heart Rate Monitor

Tested devices:

- Garmin fēnix® 3 (ANT+)
- Garmin fēnix® 8 (ANT+ and BLE)
- Garmin HRM-Pro Plus (ANT+ and BLE)
- Garmin HRM 600 (ANT+ and BLE)
- COROS Hear Rate Monitor (BLE)
- Mio Link Heart Rate wrist band (ANT+ and BLE)

## Important

If your sensor has already been added to your Garmin device, you need to disconnect or remove it. Watch Settings > Connectivity > Sensor > Off. Simultaneous operation of sensors with the watch and this DataField is not supported.

Any sensor that you connect directly to the watch will be considered the primary sensor. It will be used to calculate your fitness level. The sensors connected to this DataField will be for informational purposes only.

## Settings

The settings can be changed in the Garmin Connect IQ mobile app.

**Type** - only ANT sensors for older devices, and both ANT and BLE for modern devices (check **Generic Bluetooth Low Energy Channel** feature [here](https://developer.garmin.com/connect-iq/compatible-devices/)).

**ANT ID / BLE NUM** - leave this field blank to enable automatic sensor discovery. After the sensor is detected for the first time, this field will be filled with the sensor's ID. For ANT devices, this will be the device's ANT ID. For BLE devices, this will be an automatically generated ID starting with 1 (due to security policy restrictions); it is stored in the app's memory and does not change over time. You can enter any text in this field after the space. Supported formats:

- `12345 HRM 600` - ANT+ sensor ID with custom name
- `1 COROS HR` - BLE sensor ID with custom name
- `aa:bb:cc:dd:ee:ff` - BLE sensor MAC

**Data Screen** - how to display sensor values on a Garmin device screen during a workout.

**Record Chart FIT** - save the chart to your workout. You'll be able to view it in the Garmin Connect mobile app or web interface.

## TIPS

If your sensor supports both ANT and BLE, you can connect it directly to the watch using one protocol and to this DataField using the other protocol.

If you have a **Garmin HRM 600** strap, you can pair it with your watch via secure BLE to enable the **Step Speed Loss** metric, then switch the sensor to open connection mode (three LED flashes) and connect it to this DataField via the ANT+ protocol.

You can use the **Broadcast Heart Rate** feature to receive data from additional Garmin watches and compare their metrics.
