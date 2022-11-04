# chat-app

A chat app for mobile devices using React Native. The app provides users with a chat interface and options to share images and their location.

## Key features:

- A page where users can enter their name and choose a background color for the chat screen before joining the chat.
- A page displaying the conversation, as well as an input field and submit button.
- The chat must provide users with two additional communication features: sending images and location data.
- Data gets stored online and offline.

## Technologies used:

JavaScript, React Native, GiftedChat, Firebase, Expo

## Setting up the development environment:

- Clone the repository: `git clone https://github.com/mats-js/chat-app.git`
- Install Expo CLI as a global npm package: `npm install -g expo-cli`
- Install all project dependencies: `npm install`
- Head over to https://expo.dev/, create an account and log in via terminal with `expo login`
- Follow expo CLI's instructions depending on your preferred simulator (XCode, Android Studio, Expo Go)
- Start the project: `npm start` or `expo start`
- In case Expo cannot detect the running project, try running it with `npx expo start --tunnel`

## Database configuration:

- Go to https://firebase.google.com/ and sign in with your existing or create a new Google account
- Go to Firebase console and click on "Create Project"
- Once on your project's dashboard, click on "Develop" on the left, then "Cloud Firestore", then "Create Database" and follow the instructions, selecting "Test Mode"
- Create a new collection named "messages"
- Under "Project Settings", scroll down and click the "Firestore for Web" button (</>)
- Choose a name for the chat app, then click "Register" and copy the configuration code to the cloned repository into components/Chat.js, replacing the following with your configuration code:
  apiKey: '...',
  authDomain: '...',
  projectId: '...',
  storageBucket: '...',
  messagingSenderId: '...',
  appId: '...',
- To be able to upload photos, go to "Storage" on the left, then the "Rules" tab, then exchange "allow read, write: if false;" for "allow read, write: if true;"

## Main dependencies:

- "@expo/react-native-action-sheet": "^3.14.0",
- "@expo/webpack-config": "^0.17.0",
- "@react-native-async-storage/async-storage": "^1.17.10",
- "@react-native-community/masked-view": "^0.1.11",
- "@react-native-community/netinfo": "9.3.0",
- "@react-navigation/native": "^6.0.13",
- "@react-navigation/stack": "^6.3.3",
- "expo": "^46.0.16",
- "expo-image-picker": "^13.3.1",
- "expo-location": "^14.3.0",
- "expo-permissions": "^13.2.0",
- "expo-status-bar": "~1.4.0",
- "firebase": "^8.10.1",
- "react": "18.0.0",
- "react-dom": "18.0.0",
- "react-native": "0.69.6",
- "react-native-gesture-handler": "~2.5.0",
- "react-native-gifted-chat": "^1.0.4",
- "react-native-maps": "0.31.1",
- "react-native-reanimated": "~2.9.1",
- "react-native-safe-area-context": "4.3.1",
- "react-native-screens": "~3.15.0",
- "react-native-web": "~0.18.7",
- "react-navigation": "^4.4.4"

![Screenshot 1](/img/Screenshot_1.png?raw=true)
![Screenshot 2](/img/Screenshot_2.png?raw=true)
