# MOCKUP API

We added to the Api an mockup Api <Strong>Use it only On DEV</Strong> the recepured data from this Mockup can be found on the file <Strong> static/data.js </strong>

### Description of Server Data

- ###### HomeData Describe All stores

- ###### Products Describe All Products

- ###### HomeAds Describe All Ads showen on the app

- ###### Tags Describe All tag linked to products


### Description of The mockup api that can be found on app.js

 - ###### The rout Get /pharma
 return all stores from Homedata that also take parametre query to make pagination , we limeted pagination for 3 pages for showCase prupose

 - ###### The rout Get /pharma/:id
 return detail of the store that matche the id ;

 - ###### The rout Get /pharma/openpharma/:date
 return all List of Stores opened at the moment of the request was make

 - ###### The rout Get /pub/homePage
 return all List of Ads recupered from HomeAds

 - ###### Get /pharma/:id/produits
 return all List of products from the id of store passed as parametre , the returnd data cam from HomeData

 - ###### Get /produit/:id/withrelated
 return all detail of product that match the id and show related product from the same store

 - ###### Get /pub/topandbottom
 return type bottom and top of Ads recupered from HomeAds

 - ###### Get /pub/bottom
 return type bottom  of Ads recupered from HomeAds

 - ###### Get /user/:token
 Check if the token matche a user token

 - ###### Post /user/login
 SignIn a user

 - ###### Put /user/connected/changerecieve
 Change the status if the user allow or not receiving newsletter

 - ###### Put /user/connected/changePassword
 Change password of user

 - ###### Put /user/connected/user
 Change information of user

 - ###### Get /tag/:id/withrelated
 get Product detail and related products from the scaned tag

 - ###### Get /tag/:id
get Product detail from the scaned tag