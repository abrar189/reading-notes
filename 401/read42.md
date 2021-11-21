# Location

## Get the last known location

Use the fused location provider to retrieve the device's last known location. The fused location provider is one of the location APIs in Google Play services.

It manages the underlying location technology and provides a simple API so that you can specify requirements at a high level, like high accuracy or low power. It also optimizes the device's use of battery power.

**[Set up Google Play services]**

Your app's development project must include Google Play services. Download and install the Google Play services component via the SDK Manager and add the library to your project.

**[Specify app permissions]**

Apps whose features use location services must request location permissions, depending on the use cases of those features.

**[Create location services client]**

In your activity's `onCreate()` method, create an instance of the Fused Location Provider Client.

**[Get the last known location]**

You can use the fused location provider's `getLastLocation()` method to retrieve the device location. The precision of the location returned by this call is determined by the permission setting you put in your app manifest.

**[Choose the best location estimate]**

The **`FusedLocationProviderClient`** provides several methods to retrieve device location information:

- **getLastLocation()** gets a location estimate more quickly and minimizes battery usage that can be attributed to your app. However, the location information might be out of date, if no other clients have actively used location recently.

- **getCurrentLocation()** gets a fresher, more accurate location more consistently. However, this method can cause active location computation to occur on the device
