# Privacy Information for WallCam

This document describes how the WallCam iOS app handles user data. Use this as the source of truth when filling out the App Store Connect "App Privacy" and "Privacy Manifest" sections.

> NOTE: Please review and update all TODO sections so that this document accurately reflects the real behavior of the app.

---

## 1. Overview

WallCam is an iOS application that allows users to [TODO: short functional description of the app, e.g. "capture photos and create wallpapers"].

We designed WallCam with privacy in mind:

- We collect only the minimum data necessary to provide core features.
- We do not sell user data to third parties.
- We do not use data for cross‑app tracking unless explicitly stated below.

---

## 2. Data Types Collected

### 2.1 Contact Info
- Email address: **[YES/NO – TODO]**
- Name / nickname: **[YES/NO – TODO]**
- Phone number: **[YES/NO – TODO]**

**Purpose(s):**
- Account creation & authentication: **[YES/NO – TODO]**
- Customer support: **[YES/NO – TODO]**
- Marketing communications: **[YES/NO – TODO]**

### 2.2 Location
- Precise location (GPS): **[YES/NO – TODO]**
- Approximate location: **[YES/NO – TODO]**

**Purpose(s):**
- Feature functionality (e.g., location‑based content): **[YES/NO – TODO]**
- Analytics: **[YES/NO – TODO]**
- Advertising: **[YES/NO – TODO]**

### 2.3 Photos, Videos, Camera & Microphone
- Photos from Photo Library: **[YES/NO – TODO]**
- Live camera feed: **[YES/NO – typically YES for camera apps – TODO]**
- Microphone audio: **[YES/NO – TODO]**

**Handling:**
- Camera access is used to [TODO: e.g. "capture photos and videos inside the app"].
- Photos/videos stay on the device unless the user explicitly shares or backs them up.
- We do **not** access media in the background.

### 2.4 Identifiers
- Device ID (e.g., Identifier for Vendor – IDFV): **[YES/NO – usually YES – TODO]**
- Advertising Identifier (IDFA): **[YES/NO – TODO]**
- User ID / Account ID: **[YES/NO – TODO]**

**Purpose(s):**
- Analytics: **[YES/NO – TODO]**
- Crash reporting & diagnostics: **[YES/NO – TODO]**
- Personalised advertising: **[YES/NO – TODO]**

### 2.5 Usage Data
- App interaction (screens, taps, session duration): **[YES/NO – TODO]**
- Crash logs: **[YES/NO – TODO]**
- Performance data (startup time, memory, etc.): **[YES/NO – TODO]**

**Purpose(s):**
- Improve app stability and performance
- Understand feature usage patterns

### 2.6 Other Data
- In‑app purchases / subscription status: **[YES/NO – TODO]**
- Push notification token: **[YES/NO – TODO]**
- Any other data type: **[Describe or set to NONE – TODO]**

---

## 3. Tracking & Third‑Party Partners

### 3.1 App Tracking Transparency (ATT)

If the app uses the IDFA or tracks users across apps/websites owned by other companies, you **must** request tracking permission using Apples AppTrackingTransparency framework.

- We request tracking permission via ATT: **[YES/NO – TODO]**
- We track users across apps & websites owned by other companies: **[YES/NO – TODO]**

### 3.2 Third‑Party SDKs and Services

List all SDKs that collect or process data (analytics, ads, crash reporting, etc.). Example:

- **Firebase Analytics** – collects usage data and identifiers for analytics and performance.
- **Firebase Crashlytics** – collects crash logs and basic device information to improve stability.
- **[AD NETWORK NAME]** – collects identifiers and usage data for advertising (if applicable).

For each SDK, specify:
- What data is collected (from section 2)
- Purpose (analytics, ads, crash reporting, etc.)
- Whether the SDK uses data for tracking and/or cross‑app advertising

> TODO: Replace examples above with the actual SDKs used in WallCam or explicitly state that no third‑party analytics/ads SDKs are used.

---

## 4. Data Usage, Sharing, and Retention

### 4.1 Data Usage

We use collected data for the following purposes:

- To provide and improve the core functionality of WallCam.
- To diagnose crashes and technical issues.
- To understand how the app is used and prioritize new features.
- [Optional] To show personalised or non‑personalised advertisements. **[YES/NO – TODO]**

### 4.2 Data Sharing

We may share limited data with service providers who help us operate the app, such as:

- Analytics providers (e.g., Firebase Analytics)
- Crash reporting tools (e.g., Crashlytics)
- Payment processors or Apples in‑app purchase system

We do **not**:
- Sell user data to third parties.
- Share data with data brokers.

### 4.3 Data Retention

- Usage and analytics data: retained for up to **[X months/years – TODO]**.
- Crash logs: retained for up to **[X months/years – TODO]**.
- Account data (if you have accounts): retained while the account is active and for a limited time afterward, unless the user requests deletion.

---

## 5. User Controls & Rights

Depending on your region, users may have rights such as:

- Accessing the data we store about them.
- Requesting correction or deletion of their data.
- Opting out of certain data uses (e.g., marketing emails, tracking).

To exercise these rights or ask privacy‑related questions, users can contact us at:

- Email: **[your‑support‑email@example.com – TODO]**

Within the app, users can:
- Manage camera/microphone/photo permissions via iOS Settings.
- Disable push notifications via iOS Settings.
- [If applicable] Manage in‑app privacy settings via: **[Settings screen path – TODO]**

---

## 6. Childrens Privacy

WallCam is **[NOT / IS]** intended for children under the age of 13 (or the minimum age in your jurisdiction). **[Choose one and adjust text – TODO]**

If we learn that we have inadvertently collected data from a child without appropriate consent, we will delete that data as soon as possible.

---

## 7. Changes to This Privacy Information

We may update this document from time to time to reflect changes in the app or in privacy regulations. The latest version will always be kept in the project repository as `Privacy_Information.md`. If required by law, we will also notify users of material changes within the app.

---

## 8. Quick Summary for App Store Connect (Copy/Paste Helper)

- **Data Collected:** [list high‑level categories, e.g. Contact Info, Identifiers, Usage Data, Diagnostics].
- **Data Linked to User:** [YES/NO per category – TODO].
- **Data Used for Tracking:** [YES/NO per category – TODO].
- **Third‑Party Tracking (Ads/Analytics):** [YES/NO – TODO].

Please ensure this summary matches the checkboxes you select in App Store Connect.
