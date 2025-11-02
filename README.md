# TuneScope

This is a web-based audio analyzer that uses Firebase for authentication and analytics.

## How to Run

1.  **Set up a Firebase project:** If you don't have one already, create a new project on the [Firebase Console](https://console.firebase.google.com/).
2.  **Get your Firebase configuration:** In your Firebase project, go to the project settings and find your web app's configuration object. It will look similar to the `firebaseConfig` object in the `analyzer.html` file.
3.  **Replace the placeholder configuration:** Open the `analyzer.html` file and replace the placeholder `firebaseConfig` object with your actual Firebase project configuration.
4.  **Enable Firebase Authentication:** In the Firebase Console, go to the "Authentication" section and enable the sign-in methods you want to use (e.g., email/password, Google, etc.). The code redirects to `signup.html` which is not provided, so you might need to create that file or change the redirect to a login page.
5.  **Open the HTML file in a browser:** Once you've configured Firebase, you can open the `analyzer.html` file in your web browser.

## Dependencies

This project uses the following front-end libraries, which are loaded from a CDN:

*   [Firebase](https://firebase.google.com/docs/web/setup)

## Detailed Firebase Setup

### 1. Create a Firebase Project

1.  Go to the [Firebase Console](https://console.firebase.google.com/).
2.  Click on **"Add project"** and follow the on-screen instructions to create a new project. Give it a name (e.g., "TuneScope").

### 2. Register Your Web App

1.  Once your project is created, you'll be taken to the project dashboard.
2.  Click on the web icon (`</>`) to add a web app to your project.
3.  Give your app a nickname (e.g., "TuneScope Web").
4.  You don't need to set up Firebase Hosting at this stage.
5.  Click on **"Register app"**.

### 3. Get Your Firebase Configuration

1.  After registering your app, Firebase will provide you with a `firebaseConfig` object. This object contains the API keys and other information your app needs to connect to Firebase.
2.  Copy this object. You will need it in the next step.

### 4. Add the Firebase Configuration to Your HTML Files

1.  You will need to do this for all the HTML files in the project that use Firebase.
2.  Open the `analyzer.html` file (and other HTML files) in a text editor.
3.  Find the `<script>` section at the bottom of the file that contains the `firebaseConfig` object.
4.  Replace the placeholder `firebaseConfig` object with the one you copied from the Firebase console.

    ```javascript
    // TODO: Replace with your actual Firebase config object
    const firebaseConfig = {
      apiKey: "YOUR_API_KEY",
      authDomain: "YOUR_AUTH_DOMAIN",
      projectId: "YOUR_PROJECT_ID",
      storageBucket: "YOUR_STORAGE_BUCKET",
      messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
      appId: "YOUR_APP_ID",
      measurementId: "YOUR_MEASUREMENT_ID"
    };
    ```

### 5. Set Up Firebase Authentication

1.  In the Firebase Console, go to the **"Authentication"** section from the left-hand menu.
2.  Click on the **"Sign-in method"** tab.
3.  Enable the sign-in providers you want to use. For example, you can enable **"Email/Password"** and **"Google"**.
4.  The code in `analyzer.html` redirects to `signup.html` if the user is not authenticated. You will need to create a `signup.html` and a `login.html` page with the necessary Firebase authentication UI and logic.

### 6. Set Up Firebase Storage (Optional)

If you want to store the audio files in the cloud, you can use Firebase Storage.

1.  In the Firebase Console, go to the **"Storage"** section.
2.  Click on **"Get started"** and follow the on-screen instructions to set up Firebase Storage.
3.  You will need to add the Firebase Storage SDK to your HTML files and then use the Firebase Storage API to upload and download files.
