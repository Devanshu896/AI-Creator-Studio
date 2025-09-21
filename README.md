# AI-Creator-Studio

LIVE LINK :  https://devanshu896.github.io/AI-Creator-Studio/

![App Screenshot](https://github.com/Devanshu896/AI-Creator-Studio/blob/main/AI%20Creator%20Studio%20SS.png)


## AI Creator Studio

This project is a dynamic web application that serves as an **AI Creator Studio**, offering users a hub for generating and analyzing content using artificial intelligence. The application provides three core functionalities: text generation, image generation, and image analysis. It features a responsive and modern user interface built with a utility-first CSS framework.

***

### Key Features

* **Multi-functional AI Platform**: Users can switch between three distinct modes:
    * **Text Generation**: Create written content like stories, poems, and articles from a text prompt.
    * **Image Generation**: Generate images based on a user-provided text prompt.
    * **Image Analysis**: Upload an image and ask the AI to describe its contents or answer specific questions about it.
* **Prompt Management**: Includes a "Surprise Me" button that populates the input with a random, pre-defined prompt to inspire the user.
* **Generation History**: The application saves a history of all generated content (text and images) and displays it on the page.
* **Responsive Design**: The interface is designed to be fully responsive and works well on both desktop and mobile devices.
* **User Authentication**: The application uses Firebase to handle anonymous user authentication, ensuring each user has a unique ID and their history is maintained across sessions.
* **State Management**: The UI dynamically updates based on the application's state, such as showing a loading spinner during generation and disabling buttons to prevent multiple submissions.
* **Clipboard Integration**: A "Copy" button is available for text-based results, allowing users to easily copy the generated content to their clipboard with a single click.
* **Confirmation Modal**: A modal window is used to confirm sensitive actions, such as clearing the generation history.
* **Toast Notifications**: Provides user feedback with non-intrusive toast pop-ups for actions like copying text.

***

### Technologies Used

### Frontend
* **HTML5**: Provides the semantic structure of the web page.
* **CSS3**: Custom CSS is used for specific styles like modal overlays, toast animations, and font settings.
* **Tailwind CSS**: A utility-first CSS framework used for rapid UI development. It handles the modern, dark theme and responsive layout.
* **JavaScript (ES Modules)**: Powers the application's interactive features and logic. It manages UI state, handles user events, and communicates with the backend APIs.
* **Inter Font**: A clean, modern sans-serif font is imported to be used throughout the application.

### Backend & API Integration
* **Google Gemini API**: This is the core AI technology powering the text and image generation/analysis features. The application makes direct calls to the Gemini API endpoints for different content types.
* **Firebase**: Used for two key backend functions:
    * **Firebase Authentication**: Manages anonymous user sessions to provide a persistent `userId` for each user.
    * **Cloud Firestore**: A NoSQL cloud database used to store and retrieve the user's generation history. The history is stored under a collection specific to the authenticated user's ID.
