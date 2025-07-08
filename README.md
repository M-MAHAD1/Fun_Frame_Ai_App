🚀 Project Overview: Fun Frame AI

Fun Frame AI is an innovative Android application designed to add a touch of humor and creativity to your photos by generating funny and contextually relevant comments using Artificial Intelligence. It aims to provide users with an engaging and effortless way to enhance their image-sharing experience on social media and with friends.

Purpose and Vision:
The primary goal of Fun Frame AI is to leverage the power of generative AI to transform ordinary photos into sources of laughter and entertainment. In a world saturated with visual content, the app helps users make their images stand out with witty captions, fostering more engaging interactions and bringing smiles to faces.

Key Features by Screen:
1. Main Screen (MainFragment)
   
This is the initial interaction point where users prepare their input for AI processing.

![image alt](https://github.com/M-MAHAD1/Fun_Frame_Ai_App/blob/main/Screenshot%20(82).png)

Image Upload & Preview: Users can easily select an image from their device's gallery. A large image box provides a clear preview of the selected photo.

Language Selection: A spinner allows users to choose their preferred language for comment generation from a list of 20 commonly used languages (e.g., English, Spanish, Hindi, Arabic, Mandarin Chinese).

![image alt](https://github.com/M-MAHAD1/Fun_Frame_Ai_App/blob/main/Screenshot%20(93).png)

Comment Quantity Selection: Another spinner enables users to specify how many funny comments they want the AI to generate (options typically range from 5 to 20 comments).

Runtime Permissions Handling: The app gracefully requests necessary storage permissions (for gallery access) at runtime, ensuring a secure and user-friendly onboarding process.

Input Validation: Strict validation is in place to ensure that only image files are selected. If a user attempts to select a non-image file (like a video), the app provides an immediate toast message and prevents the invalid file from being processed, avoiding crashes.

Ad Integration (Banner Ad): A prominent banner ad is displayed above the "Upload Image" section, providing consistent visibility without obstructing core functionality.

Interstitial Ad Trigger: Upon clicking the "Generate" button, an interstitial (full-screen) ad is displayed, creating a natural break before navigating to the results.



2. Results Screen (ResultFragment)
   
This screen displays the AI-generated comments and offers various sharing options.

AI-Powered Comment Generation: After the user submits an image, the app integrates with the Google Gemini API to intelligently analyze the visual content and generate a batch of humorous comments.

Robust Error Handling & Patience: The application is built with robust error handling for network connectivity issues. It includes increased network timeouts (up to 30 seconds) to gracefully handle slow internet connections (like 2G/3G), preventing premature "timeout" errors or allowing more time for comments to be generated and received.

Individual Comment Sharing: Each generated comment in the list has a dedicated share icon next to it. Users can tap this icon to share that specific comment. When a single comment is shared, the original selected image is also included in the share intent, providing visual context.

![image alt](https://github.com/M-MAHAD1/Fun_Frame_Ai_App/blob/main/Screenshot%20(96).png)

Batch Sharing (Image + All Comments): A dedicated "Share" button allows users to share the original uploaded image along with all the generated comments in a single, convenient action.

![image alt](https://github.com/M-MAHAD1/Fun_Frame_Ai_App/blob/main/Screenshot%20(97).png)

Regenerate Comments: Users have the option to regenerate comments for the same image, providing more humorous options.

![image alt](https://github.com/M-MAHAD1/Fun_Frame_Ai_App/blob/main/Screenshot%20(95).png)

Technologies & Tools Used:
Languages: Kotlin, XML

Frameworks/Libraries:

Android SDK & AndroidX Libraries

Google Play Services (for AdMob integration)

OkHttp (for efficient HTTP requests to the Gemini API)

Gson (for JSON parsing of API responses)

Kotlin Coroutines (for asynchronous programming and managing long-running operations without blocking the UI)

AI/ML: Google Gemini API (for generative AI capabilities)

Integrated Development Environment (IDE): Android Studio

This project demonstrates a strong foundation in Android development, API integration, and a commitment to creating engaging and resilient mobile applications.
