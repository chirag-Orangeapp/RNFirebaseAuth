# React Native Firebase Authentication

Firebase Authentication with React Native

This is a demo project with use of React Native to Authenticate Firebase User with different methods provided by Firebase.

This project was built using [React Native Firebase](https://rnfirebase.io/).

## How to use

1. To run the project
  
  ```
  npm install
  ```
  
  ```
  npx pod-install
  ```
  
2. Create a Firebase project 
  
  [Firebase](https://console.firebase.google.com/)

3. Add config object from Firebase Webapp in to /src/app/services/firebase/firebase-config.ts
  
  ```
  var config = {
  apiKey: '',
  authDomain: '',
  databaseURL: '',
  projectId: '',
  storageBucket: '',
  messagingSenderId: ''
};

## Email and Password authentication with firebase

1. Enable email and password authentication on Firebase.

## Facebook authentication with firebase

1. Create facebook app using facebook devloper account.

2. Add android and ios platform on facebook app.

3. Enable facebook authentication and set facebook app id and secrate key on Firebase.

## Google authentication with firebase

1. Create Android and ios platform from firebase project setting. 

2. Download google-service.json and googleService-info.plist file and add both file project root folder.

3. Enable google authentication on Firebase.

## Phone number authentication with firebase

1. Enable phone number authentication on Firebase.

## Apple authentication with firebase

1. Enable phone number authentication on Firebase.

## Setup Guides

1. For setup on ios follow [ios guide](src/IosGuide.md)

2. For setup on android follow [android guide](src/AndroidGuide.md)

## To do

- [x] Add Authentication with Email and Password
- [x] Add Authentication with Facebook
- [x] Add Authentication with Google
- [x] Add Authentication with Phone number
- [x] Add Authentication with Apple
- [ ] Add Authentication with Twitter