# Getting started

####  1) Install Packages

- **First:** Unzip downloaded file from Code Canyon
- **Second:** Unzip Findme folder in the downloaded file that hav been unzeepid in the first step
- **Third:** Open the folder you can use https://code.visualstudio.com/

<img src="https://res.cloudinary.com/testcloudperfom-shop/image/upload/v1599352530/Capture_d_e%CC%81cran_2020-09-06_a%CC%80_01.34.37_fppmay.png" width="400" height="600">

Open terminal and Run
```
yarn
``` 

Open the ios folder and run 
```
Pod install
``` 


####  2) Run the app

- **Run Android:** Run
```
react-native run-android
``` 

- **Run Ios:** To run ios app go to ios folder and open the findme.xcworkspace generated from the commade Pod Install



> If you face probleme whit firebase Go to Configure Firebase


### 3) On Release on android

> you need to change google map API_KEY from https://console.developers.google.com/apis/library/maps-android-backend.googleapis.com

after Get and API KEY replace it in
```
    <meta-data android:name="com.google.android.geo.API_KEY" android:value="YOUR_API_KEY" />
```
