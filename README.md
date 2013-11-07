You can use this repository as a maven repo in your gradle build. Example of working `build.gradle`:

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