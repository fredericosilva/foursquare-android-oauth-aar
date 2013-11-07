foursquare-android-oauth-aar
============================

Foursquare native authentication library built with gradle in aar format for usage with android gradle build system.

Inspired by [facebook-api-android-aar](https://github.com/mente/facebook-api-android-aar)

```groovy
buildscript {
    repositories {
        mavenCentral()
    }

    dependencies {
        classpath 'com.android.tools.build:gradle:+'
    }
}

repositories {
    mavenCentral()
    maven {
        url 'http://fredericosilva.github.io/foursquare-android-oauth-aar'
    }
}

apply plugin: 'android'
dependencies {
    compile 'com.foursquare:foursquare-android-nativeoauth-lib:1.0.0@aar'
}

android {
  //android build setup
}
```