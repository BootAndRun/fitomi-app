# Privacy Policy

**Last updated: June 14, 2026**

---

## 1. Introduction

This Privacy Policy explains how your personal data is collected, used, and protected when you use the mobile application **Fitomi** ("the App"). The App is developed and provided by:

**Marius Hartmann**
Osnabrück, Germany
Contact: bootandrun@gmail.com

By creating an account and using the App, you acknowledge that you have read and understood this Privacy Policy. If you do not agree with this policy, please do not use the App.

---

## 2. Overview of Data We Process

Fitomi is a recipe management, nutrition tracking, and meal planning application. Because the App offers cloud sync, account creation, and collaborative features (shared cookbooks and shopping lists), some of your personal data is necessarily processed on our servers and by third-party services. We are committed to processing only the data that is strictly required to provide the App's functionality.

The following categories of data are processed:

- **Account data** – your email address, username, display name, and account settings
- **Nutritional diary data** – meals, food items, portions, calorie and macronutrient entries, water intake, and dietary goals
- **Recipes, cookbooks, and ingredients** – content you create or contribute to shared cookbooks
- **Shopping lists** – items you add, including shared lists with other users
- **Images** – photos of recipes or cookbooks stored locally on your device only
- **Device and network data** – IP address transmitted as part of standard network communication with third-party services

---

## 3. Account Creation and Authentication

To use the core features of Fitomi, you must create an account. We support two methods:

### 3.1 Passwordless Email Sign-In (Magic Link)

When you sign in with your email address, we send you a one-time sign-in link. Your email address is:
- Transmitted to and processed by **Firebase Authentication** (Google LLC) to send and verify the sign-in link
- Stored in your user profile in our Firestore database (see Section 4)
- Temporarily stored on your device in local app storage (SharedPreferences) solely to complete the sign-in process on the same device

**Legal basis:** Art. 6(1)(b) GDPR – processing is necessary for the performance of the contract (providing you with access to the App).

### 3.2 Google Sign-In

Alternatively, you can sign in using your existing Google account. In this case:
- You authenticate directly with Google. Google's own privacy policy applies to this process: https://policies.google.com/privacy
- Upon successful sign-in, we receive your email address, display name, and Google profile photo URL from Google
- These are stored in your user profile in our Firestore database

**Legal basis:** Art. 6(1)(b) GDPR – processing is necessary for the performance of the contract.

---

## 4. Data Stored in Our Cloud Database (Firebase Firestore)

Fitomi uses **Google Firebase Cloud Firestore** as its cloud database. The following data is stored there and associated with your account:

### 4.1 User Profile

When you register, a user profile document is created containing:
- Unique user ID (UID) assigned by Firebase Authentication
- Email address
- Username and display name (editable by you)
- Profile visibility setting (public/private, relevant for a planned community feature)
- Account plan (Free or Pro) and plan expiry date – set server-side only
- Account creation date and last update timestamp

### 4.2 Recipes, Cookbooks, and Ingredients

Any recipes, cookbooks, and ingredients you create are stored in Firestore. This includes:
- Titles, descriptions, tags, nutritional values, step-by-step instructions, and ingredient lists
- The user ID of the creator and the list of cookbook member IDs
- Timestamps for creation and updates

When you share a cookbook via invite code, all members of that cookbook can read and edit its content. When you share an individual recipe via a public share link, the recipe content is publicly readable by anyone who has the link.

### 4.3 Food Diary and Nutritional Tracking

The diary feature allows you to track your daily food intake and water consumption. The following data is stored per user:
- Diary entries per date, including meal categories (e.g., breakfast, lunch, dinner, snacks)
- Individual food items per meal with name, quantity, and nutritional values (calories, protein, fat, carbohydrates, and other nutrients)
- Daily water intake entries
- Dietary goals you have set (e.g., target calories, protein, fat, carbohydrates)

This data is **strictly private**: it is only accessible to you. No other user, including other cookbook members, can see your diary or goals.

> **Note on health data:** Nutritional tracking data (food intake, calorie and macronutrient records) may constitute data relating to your health under Art. 9 GDPR. We process this data exclusively on the basis of your explicit and voluntary use of the diary feature as the core service you signed up for. The legal basis is Art. 6(1)(b) GDPR in conjunction with Art. 9(2)(a) GDPR (your explicit consent, expressed through active and voluntary use of the feature). You may delete all diary data at any time by deleting your account.

### 4.4 Shopping Lists

Shopping list content (item names, quantities, checked status) and list membership are stored in Firestore. When a shopping list is shared via invite code, all members can read and edit it. Membership management follows the same access control model as shared cookbooks.

### 4.5 Invitation Codes and Recipe Share Links

When you generate an invite code for a cookbook or shopping list, a document containing the code, your user ID, and the associated resource ID is stored in Firestore. Codes are deleted automatically once redeemed. Recipe share links are stored as publicly readable documents; list access is prevented to avoid code enumeration.

**Legal basis for all Firestore data:** Art. 6(1)(b) GDPR – processing is necessary for the performance of the contract (providing the App's core features such as cloud sync, collaboration, and cross-device access).

---

## 5. Data Stored Locally on Your Device

### 5.1 Images (Photos)

If you add photos to your recipes or cookbooks, images are stored **exclusively on your device** in the App's local document directory. Images are **never uploaded to any server** and are not accessible to us. You can delete images by removing them within the App or by uninstalling the App.

### 5.2 App Settings

Preferences such as your dark/light mode choice and water tracking settings are saved in your device's local app storage (SharedPreferences). This data never leaves your device.

### 5.3 Common Meals Database

The App includes a built-in local database (SQLite via Drift) of common pre-defined food items (e.g., generic meals like "doner kebab") that can be added to your diary for quick nutritional logging. This database is bundled with the App and no personal data is stored in it.

---

## 6. Camera and Photo Library Access

The App may request access to your device's camera and photo library in two contexts:

- **Barcode scanning:** To scan product barcodes for ingredient or food item lookup
- **Image selection:** To add photos to recipes or cookbooks

Both are entirely optional and only triggered by your explicit action. Camera and gallery access can be revoked at any time in your device's system settings.

**Legal basis:** Art. 6(1)(b) GDPR – processing is necessary to provide the requested feature.

---

## 7. Third-Party Services

### 7.1 Firebase (Google LLC)

Fitomi uses the following Firebase services provided by **Google LLC, 1600 Amphitheatre Parkway, Mountain View, CA 94043, USA**:

- **Firebase Authentication** – user login and session management
- **Cloud Firestore** – cloud database for all user-generated content described in Section 4

Google processes data on our behalf as a data processor under a Data Processing Agreement (Art. 28 GDPR). Data is transferred to the United States under the EU Standard Contractual Clauses (SCCs) adopted by the European Commission.

Google's privacy policy: https://policies.google.com/privacy
Firebase data processing information: https://firebase.google.com/support/privacy

### 7.2 Google Sign-In (Google LLC)

If you choose to sign in with Google, Google LLC processes your authentication data. This service is subject to Google's own privacy policy (linked above). The data transfer to the US is covered by Standard Contractual Clauses.

### 7.3 Open Food Facts API

The App integrates the **Open Food Facts API** (https://world.openfoodfacts.org), operated by the Open Food Maker Association (non-profit, France), to retrieve nutritional information when you scan a product barcode or search for a food item.

- This API is contacted **only when you actively trigger a barcode scan or food search** — never in the background or at startup
- The request technically includes your **IP address** as part of standard network communication
- No other personal data is transmitted by the App to this service

Open Food Facts is operated in the EU and subject to its own privacy policy: https://world.openfoodfacts.org/privacy

**Legal basis:** Art. 6(1)(b) GDPR – necessary to provide the requested product lookup feature.

### 7.4 Google Fonts

The App uses the `google_fonts` library, which may load font files from Google's font servers (https://fonts.google.com) at runtime. This causes your device's **IP address** to be transmitted to Google LLC servers in the US. Font files are cached locally after the first load.

**Legal basis:** Art. 6(1)(f) GDPR – legitimate interest in providing a consistent and visually accessible user interface. You may contact us if you wish to object to this processing.

> We are evaluating migrating to locally bundled fonts to eliminate this transfer entirely in a future update.

### 7.5 In-App Review (Google Play)

The App uses the **Google Play In-App Review API** to prompt you to rate the App in the Play Store after extended use. This prompt is triggered automatically after a set number of days. Any review you submit is processed directly by Google LLC and governed by Google's privacy policy. We do not receive any personal data through this mechanism.

### 7.6 App Stores (Google Play / Apple App Store)

When you download or use the App, **Google LLC** (Google Play Store) and/or **Apple Inc.** (Apple App Store) may independently collect data such as download statistics, crash reports, and device diagnostics under their own privacy policies. We have no access to personally identifiable information collected by these platforms.

- Google Play: https://policies.google.com/privacy
- Apple App Store: https://www.apple.com/legal/privacy

---

## 8. No Analytics, No Crash Reporting, No Advertising

Fitomi does **not** use any analytics SDKs, crash reporting services, or tracking tools. The developer does not collect usage data, behavioral data, or diagnostic data through the App. The App contains no advertisements and no advertising SDKs. No data is shared with advertising networks.

---

## 9. Legal Bases for Data Processing (GDPR Summary)

| Processing Activity | Legal Basis |
|---|---|
| Account creation & authentication | Art. 6(1)(b) – contract performance |
| Cloud sync of recipes, cookbooks, diary | Art. 6(1)(b) – contract performance |
| Nutritional diary and health-related data | Art. 6(1)(b) + Art. 9(2)(a) – explicit consent via voluntary use |
| Collaborative features (shared cookbooks, lists) | Art. 6(1)(b) – contract performance |
| Open Food Facts API (IP address) | Art. 6(1)(b) – contract performance |
| Google Fonts (IP address) | Art. 6(1)(f) – legitimate interest |
| In-App Review prompt | Art. 6(1)(f) – legitimate interest |

---

## 10. International Data Transfers

Your data is processed by Firebase (Google LLC) on servers that may be located outside the European Economic Area (EEA), including in the United States. These transfers are safeguarded by the **EU Standard Contractual Clauses (SCCs)** approved by the European Commission under Art. 46(2)(c) GDPR.

Similarly, the use of Google Sign-In and Google Fonts involves data transfers to the US, covered by the same legal mechanism.

The Open Food Facts API is operated by a non-profit organization in France and data is processed within the EU/EEA.

---

## 11. Data Retention

| Data | Retention Period |
|---|---|
| User profile (Firestore) | Until account deletion is requested |
| Diary entries, goals, water tracking | Until account deletion is requested |
| Recipes, cookbooks, ingredients | Until deleted by you or until account deletion |
| Shopping lists | Until deleted by you or until account deletion |
| Invite codes | Deleted immediately after redemption or by creator |
| Recipe share links | Until deleted by you or account deletion |
| Email in local storage (sign-in flow) | Deleted automatically after successful sign-in |
| Locally stored images | Until removed by you or App is uninstalled |
| App settings (SharedPreferences) | Until App is uninstalled |

When you request account deletion, all data associated with your account in Firestore will be permanently deleted. Data you have contributed to shared cookbooks or shopping lists may persist for other members, but will be disassociated from your identity.

---

## 12. Your Rights Under the GDPR

As a resident of the European Union, you have the following rights regarding your personal data:

- **Right of access (Art. 15 GDPR):** You may request information about the personal data we process about you.
- **Right to rectification (Art. 16 GDPR):** You may correct inaccurate data directly in the App (e.g., username, display name) or by contacting us.
- **Right to erasure (Art. 17 GDPR):** You may request deletion of your account and all associated data. Account deletion can be initiated in the App or by contacting us.
- **Right to restriction of processing (Art. 18 GDPR):** Under certain conditions, you may request that we restrict the processing of your data.
- **Right to data portability (Art. 20 GDPR):** You may request a copy of your personal data in a structured, commonly used, and machine-readable format by contacting us.
- **Right to object (Art. 21 GDPR):** Where processing is based on legitimate interests (Art. 6(1)(f) GDPR), you have the right to object. This applies in particular to the Google Fonts processing described in Section 7.4.
- **Right to withdraw consent (Art. 7(3) GDPR):** Where processing is based on your consent (e.g., use of the diary feature), you may withdraw consent at any time by deleting the relevant data or your account. Withdrawal does not affect the lawfulness of processing before withdrawal.

To exercise any of these rights, please contact: **marius-hartmann98@web.de**

We will respond to your request within one month as required by Art. 12(3) GDPR.

You also have the right to lodge a complaint with a supervisory authority. The competent authority for residents of Germany is:

**Die Bundesbeauftragte für den Datenschutz und die Informationsfreiheit (BfDI)**
https://www.bfdi.bund.de

---

## 13. Data Security

All data stored in Firestore is protected by Firebase security rules that strictly enforce that users can only access their own data or data they have been explicitly granted access to (e.g., shared cookbook members). Communication between the App and Firebase is encrypted in transit using TLS. Locally stored data (images, settings) is protected by your device's built-in security mechanisms (e.g., device encryption, passcode/biometric protection). We do not have access to your device or locally stored data.

---

## 14. Children's Privacy

Fitomi is not directed at children under the age of 16 (or the minimum digital consent age applicable in your EU member state). We do not knowingly collect personal data from children. If you believe a child has created an account or provided personal data through the App, please contact us at marius-hartmann98@web.de so we can take appropriate action.

---

## 15. Changes to This Privacy Policy

We reserve the right to update this Privacy Policy as the App evolves. Any material changes will be communicated by updating the "Last updated" date at the top of this document. For significant changes, we will provide an in-app notice. Continued use of the App after such changes constitutes your acknowledgment of the updated policy.

---

## 16. Contact

If you have any questions, concerns, or requests regarding this Privacy Policy or your personal data, please contact:

**Marius Hartmann**
Osnabrück, Germany
Email: marius-hartmann98@web.de

---

*This Privacy Policy was prepared in accordance with the requirements of the EU General Data Protection Regulation (GDPR), the German Federal Data Protection Act (BDSG), and the developer guidelines of Google Play and the Apple App Store.*
