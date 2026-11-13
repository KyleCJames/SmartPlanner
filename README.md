# SmartPlanner — Android Task Planner

An Android Kotlin scheduling and task-management project with login/registration screens and remote data integration.

## Features visible in the source
- User registration and sign-in using Firebase Authentication
- Home screen with a week selector and task list
- Create, display, complete and remove tasks
- Retrofit integration with a configurable remote task/events API
- Firebase Cloud Functions backend example for authenticated event endpoints

## Tech stack
Kotlin, Android SDK, Firebase Authentication, Retrofit, Moshi, OkHttp, LiveData/ViewModel, JavaScript, Firebase Functions, Firestore.

## Local configuration
This public-ready source package excludes the original `app/google-services.json`, which belongs to your Firebase project. To run the application, connect your own Firebase Android application and download its `google-services.json` to `app/`. The Firebase project settings and API access rules must be configured separately.

The sample Retrofit base URL is in `app/src/main/java/com/example/smartplanner/data/remote/ApiClient.kt`; review and replace it with an endpoint you control if needed. Do not store private service credentials in the repository.

## Running locally
Open this project in Android Studio, configure Firebase as above, sync Gradle, and run on an emulator/device. The Firebase Functions sample in `functions/` requires separate Firebase project setup and deployment.

## Notes
This is a learning/portfolio project. Some task data uses local fallback/sample values, and not every function has been verified end to end. Do not treat this as a production-ready app.
