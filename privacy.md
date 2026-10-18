# Privacy Policy for the "Fitomi" App

**Last updated: October 18, 2026**

## 1. Controller

The controller responsible for data processing in connection with the "Fitomi" app (Android and iOS) is:

Marius Hartmann
Osnabrück, Germany
Email: bootandrun@gmail.com

This privacy policy explains which personal data is processed when you use the app, for what purpose, on what legal basis, and what rights you have.

## 2. Overview

Fitomi is an app for cookbooks, recipes, nutrition tracking (food diary), meal planning and shopping lists.

- **Without an account**, all data is stored exclusively locally on your device.
- **With an account**, your content is additionally stored in the cloud (Google Firebase) and synchronized across your devices. You can also share cookbooks and shopping lists with other users and share recipes via a link.

Fitomi uses **no** advertising, **no** analytics or tracking services and **no** crash reporting.

## 3. Using the app without an account

You can use the app without registering. In that case, recipes, cookbooks, diary entries, water intake, goals, meal planner, shopping lists and images are stored exclusively in a local database (SQLite) on your device. No data is transmitted to my servers or to cloud services, and there is no synchronization. If you uninstall the app, this data is lost.

Even without an account, the app uses the Open Food Facts interface when needed (see Section 8.3) and loads fonts from Google (see Section 8.4).

## 4. Account and sign-in

You can create an account to use cloud features. Sign-in is handled through Firebase Authentication (Google LLC) and is possible in the following ways:

- **Email and password:** We process your email address and password. The password is processed securely by Firebase Authentication; I have no access to your plain-text password. After registration, a confirmation email is sent. If you reset your password, an email may be sent to your address.
- **Sign in with Google:** You sign in with your Google account. Google transmits your email address, your display name and, if applicable, the URL of your profile picture to Firebase. Google's privacy policy applies to Google's processing of your data.
- **Sign in with Apple:** You sign in with "Sign in with Apple". Apple may transmit your name and email address (or, at your choice, an anonymized Apple relay address) to Firebase. Apple's privacy policy applies to Apple's processing of your data.

**Legal basis:** Art. 6(1)(b) GDPR (providing the account functions and cloud synchronization).

## 5. Cloud data (Google Firebase)

When you are signed in, the following data is stored in Firebase Firestore and Firebase Storage:

### 5.1 User profile

When you first sign in, a profile is created containing: user ID (UID), email address, username, display name, profile picture URL (if provided by Google/Apple), plan (Free/Pro, with expiry date if applicable), and creation and modification timestamps. Your initial username is automatically derived from the part of your email address before the "@"; you can change it at any time in your profile. The plan can only be changed on the server side.

### 5.2 Cookbooks, recipes and ingredients

Titles, descriptions, preparation steps, tags, categories, servings, preparation time, difficulty, ratings, ingredients (including quantities, barcodes and nutritional values), as well as the creator's ID and the IDs of the cookbook's members. All members of a shared cookbook can read and edit its content.

### 5.3 Cookbook and recipe images

Images you select for cookbooks or recipes are compressed on your device (JPEG, max. 1024 px, under 500 KB) and stored in **Firebase Storage**, so they are visible on your other devices and to members of shared cookbooks. Access is limited to members of the respective cookbook. Images that remain only on your device and the preset images bundled with the app are not uploaded. Without an account, no images are uploaded.

### 5.4 Food diary, water intake and goals

Diary entries (date, meal, foods or recipes with quantities and nutritional values), water intake (if water tracking is enabled) and your nutrition goals. This data can only be accessed by your own account.

> **Note:** This information may allow conclusions about your diet and possibly your health (health data within the meaning of Art. 9 GDPR). Entering it is voluntary. It is processed on the basis of your explicit consent (Art. 9(2)(a) in conjunction with Art. 6(1)(a) GDPR), which you give by voluntarily using these functions and signing in with cloud synchronization. You can withdraw your consent at any time with effect for the future by deleting the data or your account.

### 5.5 Shopping lists

List titles, items (name, quantity, unit, checked status, recipe name where applicable), owner and members of the list. All members of a shared list can read and edit it.

### 5.6 Sharing with other users

- **Invitation codes for cookbooks and shopping lists:** When you share, a code is generated that is valid for one hour. The code, title, owner ID and expiry time are stored. Anyone who redeems the code becomes a member. Members can see the content as well as each other's usernames. The owner can remove members; members can leave a cookbook or list.
- **Recipe share links:** When you share a recipe via a link, a copy of the recipe (title, description, category, tags, servings, time, difficulty, instructions, ingredients with nutritional values) is stored in the cloud together with the creator's name and creator ID. The link is valid for 48 hours; **anyone who knows the link can access the recipe during this period**. Therefore only share the link with people you want to show the recipe to. You can delete a share yourself at any time.

**Legal basis:** Art. 6(1)(b) GDPR (providing the functions you choose); for health data additionally Art. 9(2)(a) GDPR (see above).

## 6. Data on your device

- **Local database (SQLite):** All content is also stored locally so the app works offline and loads quickly. This includes the **meal planner**, which is stored only locally and is not synchronized to the cloud. The app also contains a built-in list of common meals with nutritional values (no personal data) as well as meals you have created yourself.
- **Settings (SharedPreferences):** Theme (light/dark), language, water tracking on/off, onboarding status, timestamps for notices (e.g. guest notice, in-app review) and a cached history of product searches (up to 7 days).
- **Images:** Images you select and cookbook/recipe images downloaded from the cloud are stored in the app's storage on your device.
- **Camera and photos:** The app only requests access to the camera (for scanning barcodes) and to your photos (for selecting images for recipes and cookbooks) when you use the respective function. You can revoke these permissions at any time in your system settings. The camera image of a barcode scan is analyzed on the device only; only the recognized barcode number is transmitted (see 8.3).
- **Keep screen awake:** In cooking mode, the app prevents the screen from turning off. No data is collected in the process.

## 7. No analytics, no advertising

The app contains no analytics or tracking tools (e.g. Firebase Analytics, Crashlytics), no advertising networks and no push notifications. No profiling for advertising purposes takes place.

## 8. Services used and recipients

### 8.1 Google Firebase (Google LLC / Google Ireland Ltd.)

Used for authentication (Firebase Authentication), database (Cloud Firestore) and image storage (Firebase Storage). A data processing agreement under Art. 28 GDPR is in place with Google. Data may be transferred to the USA; the transfer is based on EU Standard Contractual Clauses or the EU-US Data Privacy Framework adequacy decision, where Google is certified. Data in transit is encrypted using TLS.

### 8.2 Google Sign-In and Sign in with Apple

When you use these sign-in methods, the respective provider (Google or Apple) processes your data as an independent controller under its own privacy policy.

### 8.3 Open Food Facts

For barcode scanning and product search, the app queries the public interface of Open Food Facts (Open Food Facts Association, France; servers in the EU). The scanned barcode or your search term, your IP address and the app identifier (user agent) are transmitted. These requests are made only when you actively scan or search. No account data is transmitted.

**Legal basis:** Art. 6(1)(b) GDPR (providing the function you chose), alternatively Art. 6(1)(f) GDPR.

### 8.4 Google Fonts

The app loads its fonts (Poppins, Playfair Display) from Google Fonts when needed. Your IP address is transmitted to Google in the process. This serves a consistent appearance of the app (legitimate interest, Art. 6(1)(f) GDPR). You can object to this (see Section 12).

### 8.5 In-app review (Google Play / Apple App Store)

After a few days of use, the app may ask you for a rating (at most twice, at least 90 days apart). The timing is determined solely locally on your device using counters (e.g. days since installation, number of recipes). The review itself is handled via the dialog of Google Play (Android) or Apple (iOS); the developer receives no personal data in the process.

### 8.6 App stores

When you download the app, Google Play or the Apple App Store collect their own data (e.g. account, time, device identifier). The platform operators are solely responsible for this.

## 9. Retention and deletion

- **Cloud data** (profile, cookbooks, recipes, ingredients, images, shopping lists, diary, water, goals) is stored until you delete it or delete your account.
- **Invitation codes** are valid for one hour; **recipe share links** for 48 hours. Expired entries can no longer be accessed. You can delete your own shares and invitations; at the latest, they are removed when you delete your account.
- **Local data** remains on your device until you delete it, sign out, delete your account or uninstall the app.
- **Account deletion in the app:** You can delete your account directly in the app under your profile. This deletes your diary, water and goal data, your user profile, your share links and invitations, and the associated images in the cloud, and finally your sign-in account in Firebase Authentication. Your local data on the device is subsequently removed as well. For cookbooks and shopping lists, the following applies: if other members remain, ownership is transferred to the member who has been part of it the longest, and the content remains available to those members; if there are no other members, the cookbook or list is deleted together with its recipes, ingredients and images. For cookbooks and lists where you are only a member, you leave them. If deletion requires a recent sign-in, please confirm by signing in again; deletion will then continue.
- Alternatively, you can request deletion by email at bootandrun@gmail.com.

There are no statutory retention obligations for the content stored in the app. For technical reasons, backups at Google may continue to exist for a limited period.

## 10. Data security

Transmission between the app and the cloud is encrypted (TLS). Access rules in Firestore and Storage limit access to your own data and to content in which you participate as a member or which you have explicitly shared. Local data is protected by your device's security mechanisms (e.g. lock screen, device encryption).

## 11. Children

The app is not intended for children under 16. If you are younger, please use the app only with the consent of your parents or legal guardians. I am not aware of knowingly processing data of children under 16. If you become aware of such a case, please contact me at the email address above.

## 12. Your rights

Within the scope of the law, you have the following rights:

- **Access** to the data stored about you (Art. 15 GDPR)
- **Rectification** of inaccurate data (Art. 16 GDPR); you can change your username and display name directly in your profile
- **Erasure** (Art. 17 GDPR), including directly in the app (see Section 9)
- **Restriction of processing** (Art. 18 GDPR)
- **Data portability** (Art. 20 GDPR)
- **Objection** to processing based on legitimate interests (Art. 21 GDPR), e.g. to the loading of Google Fonts
- **Withdrawal of consent** with effect for the future (Art. 7(3) GDPR)

To exercise your rights, an email to bootandrun@gmail.com is sufficient. I will usually respond within one month.

You also have the right to lodge a complaint with a data protection supervisory authority, e.g. the State Commissioner for Data Protection of Lower Saxony (Landesbeauftragte für den Datenschutz Niedersachsen) or the supervisory authority of your place of residence.

## 13. Overview of legal bases

| Processing | Legal basis |
|---|---|
| Account, sign-in, cloud synchronization, sharing | Art. 6(1)(b) GDPR |
| Food diary, water, goals (health data) | Art. 9(2)(a) in conjunction with Art. 6(1)(a) GDPR |
| Barcode scan and product search (Open Food Facts) | Art. 6(1)(b), alternatively (f) GDPR |
| Google Fonts | Art. 6(1)(f) GDPR |
| In-app review (local counters) | Art. 6(1)(f) GDPR |

## 14. Changes to this policy

I will update this privacy policy when the app or the legal situation changes. The current version is available at this address; the date above shows its effective date. In the case of material changes, I will notify you in an appropriate way (e.g. in the app).

## 15. Contact

Marius Hartmann
Osnabrück, Germany
Email: bootandrun@gmail.com
