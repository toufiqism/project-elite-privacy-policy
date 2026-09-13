# Privacy Policy — Project Elite

**Last updated:** 13 September 2026
**App:** Project Elite (Android)
**Developer:** Toufiq Akbar
**Contact:** toufiqakbar@gmail.com

This policy explains what data Project Elite collects, why, where it goes, and the choices you have. Project Elite is a personal self-improvement app for planning your day and tracking study, focus, fitness, habits, reflection, and Islamic practice.

---

## 1. Data we collect

### 1.1 Your account
You need an account to use Project Elite. You can sign in with Google or with an email address and password. Accounts are managed by Firebase Authentication (Google). We store:

- Firebase user ID (UID)
- Email address
- Display name and, if you use Google sign-in, your Google profile photo URL

Passwords are handled by Firebase Authentication. We never see or store your password. Password-reset emails are sent by Firebase.

### 1.2 Stored on your device
Your tracking data is stored in the app's private storage on your phone:

- Profile: display name, age, gender, goals, title rank
- Study sessions, subjects, focus sessions
- Daily planner time blocks, nightly debriefs, weekly reviews and commitments
- Voice journal entries, saved as **text transcripts only**
- Habit definitions, daily completions, streak freezes
- Fitness data: workouts, weight log, daily step counts
- Body metrics read from Health Connect (see §1.5)
- Prayer logs, missed-prayer (Qada') records, Qibla settings, Tasbih counts
- Discipline score, Seasons (goal arcs), game results
- App settings and preferences

### 1.3 Cloud backup (when you choose to back up)
When you tap **Upload** in the backup section of Settings, the data in §1.2 is copied to a private backup in Cloud Firestore (Google), stored under your user ID. When you sign in on a new device, the backup is restored. **Health Connect data is never included in the backup.** Security rules let only you read or write your own backup. We do not sell or share it.

### 1.4 Social features (optional)
Project Elite has two optional social features. Both work only with people who join using a six-character invite code you share with them.

- **The Circle** (small private leaderboards of up to 8 people): other members see your display name, your weekly consistency percentage, and your streak length.
- **Accountability partner** (one person): your partner sees your display name, your daily score, and whether you met your targets for the areas *you choose to share* (study, fitness, habits, prayer). Partners can send each other short text messages ("nudges", up to 180 characters).

This data is stored in Cloud Firestore. Only members of that circle or partnership can read it. **Leaving a circle** deletes your standing and removes your name from it. **Ending a partnership**, which either person can do at any time, deletes the partnership, its shared daily results, and its nudges.

### 1.5 Health Connect data
If you allow it, Project Elite **reads** the following from Health Connect to show them on the Body metrics screen:

- Weight
- Sleep
- Steps
- Active calories burned
- Hydration
- Resting heart rate

How we handle this data:

- **Read-only.** The app never writes, changes, or deletes anything in Health Connect.
- **Kept on your device.** It is displayed in the app and cached locally. It is never uploaded to our servers, never included in cloud backup, and never shared with other users or third parties.
- **Not used for advertising**, profiling, credit or insurance decisions, or sold to anyone. It is not used to train AI models.
- **Not a medical service.** Body metrics are for personal tracking only.
- You can revoke access at any time in Health Connect settings. Revoking stops all further reads.

Project Elite's use of information received from Health Connect follows the [Health Connect Permissions policy](https://support.google.com/googleplay/android-developer/answer/12991134), including its Limited Use requirements.

### 1.6 Voice journal and microphone
The voice journal lets you dictate entries. When you tap the microphone, your speech is converted to text by your **device's speech-recognition service**. That service is provided by your phone's system, usually Google, and may process audio on its own servers under its own privacy policy.

- Project Elite **never records, stores, or uploads audio.** It receives text only.
- The resulting transcript is saved as a journal entry (§1.2) and is included in your cloud backup when you upload one (§1.3).
- The microphone is used only while you are actively dictating.

### 1.7 Crash reports
Release versions of the app send crash reports to **Firebase Crashlytics** (Google) so we can fix bugs. A crash report contains:

- the error and stack trace
- device model, Android version, and app version
- a Firebase installation ID

It does not contain your tracking data, journal, or health data. Crashlytics keeps crash reports for 90 days.

### 1.8 Device permissions

| Permission | Why |
| --- | --- |
| Location (`ACCESS_COARSE_LOCATION`, `ACCESS_FINE_LOCATION`) | Calculate prayer times and Qibla direction. Coordinates are sent only to the AlAdhan prayer-times API (§2). |
| Physical activity (`ACTIVITY_RECOGNITION`) | Count steps using your phone's step sensor. Counting happens on the device. |
| Microphone (`RECORD_AUDIO`) | Voice journal dictation (§1.6). |
| Health Connect (read weight, sleep, steps, active calories, hydration, resting heart rate) | Body metrics screen (§1.5). |
| Notifications (`POST_NOTIFICATIONS`) | Local reminders for prayer times, habits, study, and walking. We do not send push notifications from a server. |
| Exact alarms (`SCHEDULE_EXACT_ALARM`) | Fire prayer reminders at the exact calculated time. |
| Run at startup (`RECEIVE_BOOT_COMPLETED`) | Reschedule reminders after your phone restarts. |
| Ignore battery optimisations (`REQUEST_IGNORE_BATTERY_OPTIMIZATIONS`) | Optional. Stops some phone battery savers from blocking prayer reminders. |
| Internet, network state, vibration, wake lock | Sign-in, backup, social features, API lookups; reminder vibration and timing. |

---

## 2. Third-party services

The app uses these services. Each has its own privacy policy.

| Service | What is sent | Why |
| --- | --- | --- |
| Firebase Authentication (Google) | Email, Google credential or password | Sign-in and account management |
| Cloud Firestore (Google) | Backup data (§1.3); social data (§1.4) | Cloud backup and social features |
| Firebase Crashlytics (Google) | Crash reports (§1.7) | Fixing crashes |
| Device speech recognition (usually Google) | Your speech while dictating | Converting speech to text (§1.6) |
| AlAdhan API (`api.aladhan.com`) | Latitude, longitude, date | Prayer-time calculation |
| ExerciseDB via RapidAPI | Exercise search keywords | Exercise database lookup |
| YouTube (opens in your browser) | Exercise name as a search query | "How to perform" exercise videos |

- Google / Firebase: https://firebase.google.com/support/privacy and https://policies.google.com/privacy
- AlAdhan: https://aladhan.com/privacy
- RapidAPI: https://rapidapi.com/privacy

---

## 3. What we do NOT do

- We do not show ads or use advertising IDs.
- We do not use analytics or tracking SDKs, and we do not track you across other apps or websites.
- We do not sell, rent, or trade your personal data.
- We do not record or store audio.
- We do not upload Health Connect data.
- We do not access your contacts, SMS, call logs, camera, photos, or files.

---

## 4. Sharing and disclosure

Your data leaves your device only in the ways described above:
- the Google services that run sign-in, backup, social features, and crash reports
- the API calls in §2
- the social data you choose to share with circle members or your partner (§1.4)

We may disclose data if required by law (for example, a court order) or to protect against fraud or abuse.

---

## 5. Retention and deletion

- **Data on your device:** kept until you delete your account or uninstall the app. Uninstalling removes everything stored locally.
- **Cloud backup:** kept while your account exists.
- **Social data:** kept while you are in a circle or partnership. It is deleted when you leave the circle or end the partnership (§1.4).
- **Crash reports:** kept by Firebase Crashlytics for 90 days.
- **Delete your account:** Settings → Delete account. This permanently deletes your cloud backup and your sign-in account, and clears your tracking data from the device. It cannot be undone.
  - **Before deleting your account, leave any circles and end any partnership** (from The Circle and Accountability screens), so your name, scores, and nudges are removed from those shared spaces.
- **Deletion by email:** email **toufiqakbar@gmail.com** from your account's email address to ask us to delete your account and all associated data, including any remaining social data. We will complete the request within 30 days.

---

## 6. Security

- All network traffic uses HTTPS/TLS.
- Firestore security rules restrict your backup to your own account, and restrict circle and partnership data to their members.
- Data on your device is kept in the app's private storage, protected by Android's app sandbox and your device's encryption.

No system is perfectly secure. Protect your account with a strong password, and turn on 2-Step Verification for your Google account.

---

## 7. Children

Project Elite is not directed to children under 13, and we do not knowingly collect data from children under 13. If you believe a child has provided us data, contact us and we will delete it.

---

## 8. International users

Data handled by Google services may be processed on servers outside your country, including in the United States.

---

## 9. Changes to this policy

We may update this policy. When we do, the "Last updated" date at the top will change. Significant changes will also be mentioned in the app's release notes.

---

## 10. Contact

Questions, deletion requests, or data inquiries:
**toufiqakbar@gmail.com**
