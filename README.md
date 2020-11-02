# Google Authentication Using Firebase and Expo

## Get Started

### Open https://console.cloud.google.com/  to create OAuth Client Id for your Google SignIn

### Click One Add Credentials


![one](https://user-images.githubusercontent.com/60876387/97795657-8af02780-1c2e-11eb-9fff-c9894ecd6082.PNG)


### Then Click on OAuth Client Id


![two](https://user-images.githubusercontent.com/60876387/97795611-68f6a500-1c2e-11eb-9965-b82c1adc0848.PNG)


### Then Select Android:


![three](https://user-images.githubusercontent.com/60876387/97795608-672ce180-1c2e-11eb-9b37-a48f15b081b1.PNG)


### Add Package name and SHA-1 Key

Add your package name as `host.exp.exponent` as per the expo documentations
then add SHA-1 Key you will get key from this:

`keytool -list -v -keystore <path to .android\debub.keystore> -alias androiddebugkey -storepass android -keypass android`

### Now create a project in Firebase

Open https://firebase.google.com/ to create a project

After that click on Web

![ten](https://user-images.githubusercontent.com/60876387/97795747-00a8c300-1c30-11eb-8be3-bfcafa42f65a.PNG)

Copy the firebaseConfig code and paste it in `config.js` file in the Project

Click on Authentication and Enable Google Sigin and fill your email

![seven](https://user-images.githubusercontent.com/60876387/97795654-86c40a00-1c2e-11eb-9b5b-73ca8dd426dd.jpg)

Then copy the Oauth Client Id Key and paste it over the Web SDK Configurations

![five](https://user-images.githubusercontent.com/60876387/97795627-7449d080-1c2e-11eb-9d00-06d20eab135a.jpg)

![eight](https://user-images.githubusercontent.com/60876387/97795612-68f6a500-1c2e-11eb-9121-195644a63f22.jpg)

And Copy the OAuth Client Id and Paste it in https://github.com/lmas3009/Google-Auth-Using-React-Expo/blob/master/Components/Screens/LoginScreen.js in `androidClientId`

For Google SignIn you need to install `expo install expo-google-app-auth`
