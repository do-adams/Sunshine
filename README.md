#Sunshine
Weather data for Android and Android Wear. 

![Sunshine Preview Img](Sunshine Watch Faces Preview.png?raw=true)

Sunshine is a weather app for the Android platform designed to highlight multiple concepts of application development that I covered during the Udacity Android Developer Nanodegree program. Most notably, its feature set of Android Wear functionality is precisely what makes this app an interesting project. Besides fetching timely weather information and notifications in the background, Sunshine comes with a unique watch face that users can enjoy on both round and square Android Wear devices in order to keep them informed of the daily weather well ahead of time. 

The concepts that led me to developing the watch face portion of the app during late August 2016 are covered in Udacity's [Android Wear Development](https://www.udacity.com/course/android-wear-development--ud875A) course. When focusing on this part of the Android platform, I made sure that I:
- Built and designed an attractive custom Android Wear watch face.
- Implemented Android's Data Layer API to transfer data between the handheld and Wear devices.
- Programmatically drew UI elements on the Android Wear watchface that aligned properly across different screen shapes.
- Made efficient UI design tradeoffs between interactive and ambient modes on the Wear device.

#Getting Started

Before you begin with Sunshine you will first need a few things: 
- An [Open Weather Map API](http://openweathermap.org/api) key in your local or global gradle.properties file.
- A [Google Places API](https://developers.google.com/places/android-api/signup) key in your local or global gradle.properties file along with a `google-services.json` configuration file in your `/app` dir.

See the Gradle app-level build file for more information as to how to embed these keys in the properties file. 

Make sure you set the `IS_WEAR_DEBUG_MODE` flag to `false` in the `SunshineSyncAdapter.class` (located in the `sync` package) file if you're not testing or debugging the Android Wear functionality of the application.

If you're using an emulator for the Wear device, make sure to [forward](https://developer.android.com/training/wearables/apps/creating.html#SetupEmulator) the AVD's communication port to your handheld.
