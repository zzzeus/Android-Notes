# Android-Notes
This is a note for Android development.

* Basic 
  * Intent
  * Activity
  * Fragments   
* Architecture Components
  * ViewModel
  * Room
  * View Binding   
  * WorkManager
  * LiveData
  * Kotlin coroutines
* User interface
* Permissions
* Navigation component

## Update Gradle files
```
// In app/build.gradle
dependencies {
    // WorkManager
    implementation "androidx.work:work-runtime-ktx:$versions.work"

    // Room components
    implementation "androidx.room:room-ktx:$rootProject.roomVersion"
    kapt "androidx.room:room-compiler:$rootProject.roomVersion"
    androidTestImplementation "androidx.room:room-testing:$rootProject.roomVersion"

    // Lifecycle components
    implementation "androidx.lifecycle:lifecycle-viewmodel-ktx:$rootProject.lifecycleVersion"
    implementation "androidx.lifecycle:lifecycle-livedata-ktx:$rootProject.lifecycleVersion"
    implementation "androidx.lifecycle:lifecycle-common-java8:$rootProject.lifecycleVersion"

    // Kotlin components
    implementation "org.jetbrains.kotlin:kotlin-stdlib-jdk7:$kotlin_version"
    api "org.jetbrains.kotlinx:kotlinx-coroutines-core:$rootProject.coroutines"
    api "org.jetbrains.kotlinx:kotlinx-coroutines-android:$rootProject.coroutines"
    
    implementation "androidx.appcompat:appcompat:$rootProject.appCompatVersion"
    implementation "androidx.activity:activity-ktx:$rootProject.activityVersion"

    // UI
    implementation "androidx.constraintlayout:constraintlayout:$rootProject.constraintLayoutVersion"
    implementation "com.google.android.material:material:$rootProject.materialVersion"
}

// In build.gradle
versions.work = "2.5.0"
```

## Basic

### Intent
```Kotlin
val intent:Intent = Intent(this,NewActivity::class.java)
startActivity(intent)
```

### Activity

### Fragments

## Architecture Component

### ViewModel
