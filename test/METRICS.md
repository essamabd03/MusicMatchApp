Download rate: Use Firebase Analytics to monitor the app installation events and count the number of new downloads.
Sign-up conversion rate: Capture the rate at which new downloads lead to new sign-ups by tracking authentication events with Firebase Authentication.
Number of users trying the live discovery feature within the first week of app installation: Use a combination of Firestore to store feature usage flags and Firebase Analytics to track the timeframe of usage post-installation.
.Task Success: 
Success rate of album rating task: Track the completion of album rating tasks through Firestore event logging, identifying successful submissions and failures.
Average time to add an album to a playlist: Time-stamp the start and completion of adding an album using Firebase Analytics, then calculate the average duration.
Error rate during task completion: Implement error tracking in the app's code that reports to Firebase Crashlytics, enabling us to monitor and reduce the error rate.
