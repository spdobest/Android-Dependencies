# Android-Dependencies
  
https://github.com/gokhanaliccii/TrendyGifs/blob/develop/app/build.gradle  

Add below line in project level gradle file  
  
allprojects {  
    repositories {  
        google()  
        jcenter()  
    }  
}  
  
## AndroidX Testing dependencies  
https://developer.android.com/jetpack/androidx/migrate/artifact-mappings  
// Core library
  androidTestImplementation 'androidx.test:core:1.0.0'  
  
  // AndroidJUnitRunner and JUnit Rules  
  androidTestImplementation 'androidx.test:runner:1.1.0'  
  androidTestImplementation 'androidx.test:rules:1.1.0'  
  
  // Assertions  
  androidTestImplementation 'androidx.test.ext:junit:1.0.0'  
  androidTestImplementation 'androidx.test.ext:truth:1.0.0'  
  androidTestImplementation 'com.google.truth:truth:0.42'  
  
  // Espresso dependencies  
  androidTestImplementation 'androidx.test.espresso:espresso-core:3.1.0'  
  androidTestImplementation 'androidx.test.espresso:espresso-contrib:3.1.0'  
  androidTestImplementation 'androidx.test.espresso:espresso-intents:3.1.0'  
  androidTestImplementation 'androidx.test.espresso:espresso-accessibility:3.1.0'  
  androidTestImplementation 'androidx.test.espresso:espresso-web:3.1.0'  
  androidTestImplementation 'androidx.test.espresso.idling:idling-concurrent:3.1.0'  
  
  // The following Espresso dependency can be either "implementation"  
  // or "androidTestImplementation", depending on whether you want the  
  // dependency to appear on your APK's compile classpath or the test APK  
  // classpath.  
  androidTestImplementation 'androidx.test.espresso:espresso-idling-resource:3.1.0'  
    
## Android JETPACK DEPENDENCIES  
https://developer.android.com/jetpack/androidx/releases/work **(WORK MANAGER)**  
https://developer.android.com/jetpack/androidx/releases/room **(ROOM)**  
https://developer.android.com/jetpack/androidx/releases/paging **(PAGING)**  
https://developer.android.com/jetpack/androidx/releases/navigation **( NAVIGATION )**  
https://developer.android.com/jetpack/androidx/releases/lifecycle **( LIFE CYCLE )**  
https://developer.android.com/jetpack/androidx/releases/concurrent  

 
 ## Glide
def glideVersion = "4.9.0"  
implementation "com.github.bumptech.glide:glide:$glideVersion"  
annotationProcessor "com.github.bumptech.glide:compiler:$glideVersion"  
  
## Architecture comp. navigation
def nav_version = "2.2.0-alpha01"
implementation "androidx.navigation:navigation-fragment:$nav_version"  
implementation "androidx.navigation:navigation-ui:$nav_version"  
implementation "androidx.navigation:navigation-runtime:$nav_version" 
  
## Room  
def room_version = "2.2.0-beta01" // alpha06 has bugs  
implementation "androidx.room:room-runtime:$room_version"  
implementation "androidx.room:room-rxjava2:$room_version"  
annotationProcessor "androidx.room:room-compiler:$room_version"  
  
## RX JAVA  
// RxAndroid  
def rxandroid_version = '2.1.1'  
implementation "io.reactivex.rxjava2:rxandroid:$rxandroid_version"  
// RxJava  
def rxjava_version = '2.1.1'  
implementation "io.reactivex.rxjava2:rxjava:$rxjava_version"  
  
// Rx-Retrofit Call Adapter  
def rxcalladapter_version = '2.5.0'  
implementation "com.squareup.retrofit2:adapter-rxjava2:$rxcalladapter_version" // Retrofit call adapter  
implementation 'com.jakewharton.rxbinding3:rxbinding:3.0.0'  

## DAGGER2  
// Dagger  
def dagger_version = "2.22"  
//    def dagger_version = "2.16" // version used by google samples  
  
// Dagger2 core  
implementation "com.google.dagger:dagger:$dagger_version"  
annotationProcessor "com.google.dagger:dagger-compiler:$dagger_version"  
  
// Dagger Android  
implementation "com.google.dagger:dagger-android:$dagger_version"  
implementation "com.google.dagger:dagger-android-support:$dagger_version"  
annotationProcessor "com.google.dagger:dagger-android-processor:$dagger_version"  
  
## Retrofit   
implementation "com.squareup.retrofit2:retrofit:2.5.0"  
implementation "com.squareup.retrofit2:adapter-rxjava2:2.5.0"  
implementation "com.squareup.retrofit2:converter-gson:2.5.0"  
## OKHTTP  
implementation 'com.squareup.okhttp3:okhttp:4.0.1'  
implementation 'com.squareup.okhttp3:logging-interceptor:3.12.1'  



## ROUND IMAGEVIEW  
implementation 'de.hdodenhof:circleimageview:3.0.0'  
## KOTLIN  KTX
apply plugin: 'kotlin-android'  
  
apply plugin: 'kotlin-android-extensions'  
  
apply plugin: 'kotlin-kapt'    
  
**FIND THE KTX DEPENDENCEIS HERE  
https://developer.android.com/kotlin/ktx/extensions-list  

implementation "androidx.core:core-ktx:1.1.0"  
implementation "androidx.activity:activity-ktx:1.0.0"  
implementation "androidx.collection:collection-ktx:1.1.0"  


## COROUTINES  
// -- Coroutines
def coroutines_version = "1.2.1"
implementation "org.jetbrains.kotlinx:kotlinx-coroutines-core:$coroutines_version"
implementation "org.jetbrains.kotlinx:kotlinx-coroutines-android:$coroutines_version"

## FIREBASE
implementation 'com.google.firebase:firebase-core:16.0.3'  
implementation 'com.google.firebase:firebase-database:16.0.2'  
implementation 'com.google.firebase:firebase-storage:16.0.2'  
implementation 'com.google.firebase:firebase-auth:16.0.3'  
implementation 'com.google.firebase:firebase-storage:16.0.2'  
//16.0.2  
implementation 'com.google.android.gms:play-services-auth:16.0.0'  
  
## FCM SET UP   
https://firebase.google.com/docs/cloud-messaging/android/client  
implementation 'com.google.firebase:firebase-messaging:20.1.0'  

## Android Vision  
implementation 'com.google.android.gms:play-services-vision:15.0.0'  
  
## ANDROID DATA BINDING SET UP  
// enable data binding for app here  
android {  
    ...  
    dataBinding {  
        enabled = true  
    }  
}  
  
https://github.com/android/databinding-samples  
  
## Constraint layout  
implementation "androidx.constraintlayout:constraintlayout:2.0.0-beta4"  
  
## CARDVIEW AND ANDROID X
implementation 'androidx.appcompat:appcompat:1.0.0'  
implementation 'androidx.cardview:cardview:1.0.0'  
  
  
  
## object mapper
implementation 'com.fasterxml.jackson.core:jackson-databind:2.8.5'  
implementation 'com.fasterxml.jackson.core:jackson-core:2.8.5'  
implementation 'com.fasterxml.jackson.core:jackson-annotations:2.8.5'  
## gson  
implementation 'com.google.code.gson:gson:2.8.0'  
## Supernova Emoji  
implementation 'com.github.hani-momanii:SuperNova-Emoji:1.1'  
// implementation 'hani.momanii.supernova_emoji_library:supernova-emoji-library:0.0.2'  
  
## for emojji  
implementation 'com.rockerhieu.emojicon:library:1.3.3'  
   
 ## picaso  
implementation 'com.squareup.picasso:picasso:2.5.2'  

## CRASHLYTICS DEPENDENCIES  
buildscript {  
 repositories {  
   maven { url 'https://maven.fabric.io/public' }  
}  
  
dependencies {  
// These docs use an open ended version so that our plugin  
// can be updated quickly in response to Android tooling updates  
  
// We recommend changing it to the latest version from our changelog:  
// https://docs.fabric.io/android/changelog.html#fabric-gradle-plugin  
    classpath 'io.fabric.tools:gradle:1.+'  
  }  
}  
  
  
  

