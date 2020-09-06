# Linking

###### Linking gives you a general interface to interact with both incoming and outgoing app links.

> For example when you wile open this web site 
```
https://www.e-paper.link
``` 
OR
```
https://www.e-paper.link/tag/3
``` 

###### The App will open for the first link the app will open the WalkthroughScreen Screen

###### For the second link the app will open the SinglProduct Screen

> To Configure this in your App you need To have an Web site hosted With an domaine Name that use HTTPS

#### IOS Config

Go to ios folder and open findme.xcworkspace

![Xcode config](https://res.cloudinary.com/testcloudperfom-shop/image/upload/v1599359688/Capture_d_e%CC%81cran_2020-09-06_a%CC%80_03.30.22_rq5qma.jpg)

and replace the domaine here by your domaine name

#### Android Config

Go to android/app/src/main/AndroidManifest.xml

Replace
```
<data android:scheme="https" android:host="www.e-paper.link" />
```
###### By your domaine name


#### Web Config

In your website you need to add a file apple-app-site-association
the file need to be accessible via https://www.YOUR_DOMAINE_NAME.com/apple-app-site-association
and place this code
```
{
  "webcredentials": {
    "apps": [
      "YOUR_TEAM_ID.org.elliote.findme"
    ]
  },
  "applinks": {
    "apps": [],
    "details": [
      {
        "appID": "YOUR_TEAM_ID.org.elliote.findme",
        "paths": [
          "/*"
        ],
        "appIDs": [
          "YOUR_TEAM_ID.org.elliote.findme"
        ],
        "components": [
          {
            "/": "*",
            "comment": "All url"
          }
        ]
      }
    ]
  }
}
```
###### This config is for ios

###### For Android refere To https://developer.android.com/training/app-links/verify-site-associations?authuser=1


#### Finally go to src/static/data.js
Replace
> BASE_URL by https://www.YOUR_DOMAINE_NAME.com/tag/
> STRING_URL by YOUR_DOMAINE_NAME.com/tag/

[site]: http://e-paper.link/