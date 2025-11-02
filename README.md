# TuneScope 🎶

TuneScope is a web-based audio analysis tool that helps musicians identify musical scales and notes from an audio file. It provides real-time analysis of audio and suggests matching scales, making it a great tool for music students, producers, and enthusiasts.

## Features ✨

*   **Audio Analysis:** Analyze audio files to detect notes and frequencies.
*   **Real-Time Note Detection:** See the notes being played in real-time.
*   **Scale Suggestions:** Get suggestions for musical scales that match the detected notes.
*   **Firebase Integration:** User authentication and data storage powered by Firebase.

## Getting Started 🚀

To get a local copy up and running, follow these simple steps.

### Prerequisites

*   A modern web browser (Chrome, Firefox, Safari, etc.)
*   A Firebase account (you can create one for free [here](https://firebase.google.com/)).

### Installation

1.  **Clone the repo:**

    ```sh
    git clone https://github.com/your_username/TuneScope.git
    ```

2.  **Set up Firebase:**

    *   Create a new project in the [Firebase Console](https://console.firebase.google.com/).
    *   Add a new web app to your project.
    *   Copy the `firebaseConfig` object.
    *   In each HTML file, replace the placeholder `firebaseConfig` object with your own.
    *   Enable **Email/Password** and **Google** sign-in methods in the **Authentication** section of the Firebase Console.

3.  **Open the `index.html` file in your browser and you are ready to go!**

## Dependencies 📦

*   [Firebase](https://firebase.google.com/docs/web/setup)

## Contributing 🤝

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request