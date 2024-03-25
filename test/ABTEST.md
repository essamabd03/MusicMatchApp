**A/B Test Name:** Album/Song Rating Prompt

**User Story Number:** US6: Prompt to Rate Album/Song

**Metric** (from the HEART grid): Task Success

- **Hypothesis:** By getting users to interact more inside of our application (rating albums/songs) we will likely see a notable success in user interaction, thus fulfilling our Task Success and possibly retention rates.
- **Problem:** Users do not consistently rate albums/songs after listening to them, leading to a lack of feedback and potential missed opportunities for improving recommendations and user satisfaction.
- **Impact:** By increasing the rate of user feedback through prompt mechanisms, we can gather more data to improve our recommendation algorithms, enhance user satisfaction, and potentially increase user engagement with the platform.
- **Experiment:** To test the hypothesis, we will implement a prompt mechanism to encourage users to rate albums or songs after listening. The experiment will be conducted using Firebase capabilities to track user interactions and measure the success metrics accurately.
- **Variations:** The variation we will test involves displaying a modal prompt at the end of a listening session, asking the user to rate the album or song they just listened to. The prompt will include a star rating system and an optional text input for additional feedback. 
___
**A/B Test Name:** Light vs. Dark mode

**User Story Number:** US7: Light vs. Dark Mode

**Metric** (from the HEART grid): User Engagement & User Retention

**Hypothesis:**
- Problem: Our app has a high drop off rate during nighttime usage, suggesting potential discomfort or reduced engagement due to the brightness of the interface.
- Impact: High bounce rates during nighttime usage could lead to decreased user satisfaction and retention, ultimately affecting our app's success and revenue.
- Hypothesis: Offering a dark mode option will reduce user discomfort during nighttime usage, leading to increased engagement and retention.

**Experiment:**
- Setup: For this A/B test, we will allocate 50% of our user base to the experimental group, where users will have access to the dark mode feature. The other 50% will serve as the control group, maintaining the existing light mode interface. We will utilize Firebase Remote Config to dynamically enable dark mode for the experimental group while keeping the control group on the regular light mode.

- Success Metric: User Engagement
  - Tracking: Monitor metrics such as session duration, number of sessions per user, and interactions within the app (e.g., clicks, scrolls) using Firebase Analytics.
- Secondary Metric: User Retention
  - Tracking: Track the percentage of users who return to the app within a specified timeframe (e.g., 7 days) using Firebase Analytics.

**Variations:**
- Variation 1: Dark Mode Implementation
  - Design Work: Implement a dark mode interface design that complements the app's existing UI/UX. Considerations include choosing appropriate contrast ratios, color schemes, and ensuring readability in low-light conditions.

- Variation 2: Control Group (Light Mode)
  - Design Work: Maintain the current light mode interface design without any changes. This variation serves as the control group against which we'll compare the experimental group's performance with dark mode enabled.

By testing these variations, we aim to validate our hypothesis that introducing a dark mode option will improve user engagement and retention, particularly during nighttime usage, ultimately enhancing the overall user experience of our app.

___
**A/B Test Name:** New App Features

**User Story Number:** US8: New App Features

**Metric** (from the HEART grid): User Rating

- **Hypothesis:** While our app has a decent amount of users, the engagement with the current features of the app are not as high as were initially thought. What this suggests is that there is a bottleneck when it comes to feature adoption. We believe that the features that are live now do not have the ability to keep the users engaged. To fix this issue, we think the best course of action is redesigning the features that are not being used by users daily and make it more user-friendly. With the use of user-rating, we can get an idea of what the current feature stands and then aim at achieving a higher score with the revamped feature. We believe that improving the user rating of the app's feature will lead to higher engagement and satisfaction.
- **Experiment:** For the experiment, instead of releasing the new features to all users, we will opt to send them out to just 50% of all users. The reason for a smaller release to a certain percentage of users is to get feedback before a wider release which will allow us to fine-tune the features. Also, we can monitor the performance to see how it responds and if there are any issues. For tracking, after a week of the new feature being out, it will ask the users to rate it 1 to 5, this being done through cloud functions in Google Firebase.
- **Variations:** The variation we will use is after a feature is launched and users have had access to it for about a week, they will have a message displayed on their screen asking them to rate the feature 1 to 5 of how much they like it.
___

**A/B Testing Proposal: Optimizing the Album Rating System**

**Objective**: To determine the most effective and user-friendly album rating system that enhances engagement and provides valuable feedback for personalized recommendations within the Music Match app.

**Hypothesis**: We believe that offering a more nuanced album rating system (Version B), with options beyond the traditional five-star scale (Version A), will lead to higher user engagement and more accurate music recommendations, ultimately improving user satisfaction.

**Test Description**:

- **Version A (Control)**: The traditional five-star rating system. Users can rate albums from 1 to 5 stars, with 5 being the highest. This system is widely understood and easy to use but may not capture the full spectrum of user sentiments towards an album.

- **Version B (Variant)**: A nuanced rating system with four options: "Love," "Like," "Dislike," and "Hate." This approach aims to simplify the decision-making process for users and capture a clearer sentiment towards the music, potentially providing more actionable data for personalizing music recommendations.

**Key Performance Indicators (KPIs)**:
1. **Engagement Rate**: Measured by the percentage of users who rate albums after this feature is introduced compared to those who did so before.
2. **Rating Volume**: The total number of ratings received per album in each version, indicating which system encourages more feedback.
3. **User Retention**: Changes in daily and monthly active users, as a more engaging rating system may enhance overall app stickiness.
4. **Feedback Quality**: Qualitative assessment of how well the ratings align with other indicators of preference, such as listening time and playlist additions.

**Implementation Details**:
- Randomly assign an equal number of new and existing users to either Version A or Version B upon app login or update.
- Ensure both groups have similar demographics and usage patterns to control for external variables.
- Run the test for a period of 4 weeks to collect a substantial amount of data across different user interactions.

**Expected Outcome**:
We anticipate that Version B will outperform Version A in terms of engagement rate and feedback quality, as it allows users to express their feelings about an album more directly and succinctly. This could lead to improved personalization of music recommendations and, consequently, higher overall satisfaction and retention rates.

By comparing the performance of these two versions, we aim to refine our album rating system to better meet our users' needs and enhance their experience on the Music Match app.
<!--- replace this text with your user story! (Be sure to delete this comment afterwards!) -->
