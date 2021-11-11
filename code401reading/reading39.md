# Location
[Notes taken from this site](https://developer.android.com/training/location/retrieve-current)

## Set up Google Play Servcies
- add to build.gradle:
```Java
apply plugin: 'com.android.application'

...

dependencies {
    implementation 'com.google.android.gms:play-services-location:18.0.0'
}
```
## Specify App Permissions
> - Apps whose features use location services must request location permissions, depending on the use cases of those features.

## Create location services client
- Create an instance of `FusedLocationProviderClient` in the `onCreate()` method:
```Java
private FusedLocationProviderClient fusedLocationClient;

// ..

@Override
protected void onCreate(Bundle savedInstanceState) {
    // ...

    fusedLocationClient = LocationServices.getFusedLocationProviderClient(this);
}
```
## Get the last known location of the device
- Example:
```Java
fusedLocationClient.getLastLocation()
        .addOnSuccessListener(this, new OnSuccessListener<Location>() {
            @Override
            public void onSuccess(Location location) {
                // Got last known location. In some rare situations this can be null.
                if (location != null) {
                    // Logic to handle location object
                }
            }
        });
```
## Choose the best location estimate
The `FusedLocationProviderClient` provides several methods to retrieve device location information. Choose from one of the following, depending on your app's use case:

> - `getLastLocation()` gets a location estimate more quickly and minimizes battery usage that can be attributed to your app. However, the location information might be out of date, if no other clients have actively used location recently.
> - `getCurrentLocation()` gets a fresher, more accurate location more consistently. However, this method can cause active location computation to occur on the device.
>
>   This is the recommended way to get a fresh location, whenever possible, and is safer than alternatives like starting and managing location updates yourself using requestLocationUpdates(). If your app calls requestLocationUpdates(), your app can sometimes consume large amounts of power if location isn't available, or if the request isn't stopped correctly after obtaining a fresh location.

[Back to HOME](../README.md)