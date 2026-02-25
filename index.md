# Hospital Database App – Privacy Policy (Draft)

**Last updated:** February 25, 2026

> NOTE: This is a draft generated template. You must review it with your own legal advisor and adapt it to your actual hospital policies, local laws (e.g., GDPR, HIPAA, or local health data rules), and infrastructure before publishing.

## 1. Who we are

This application ("Hospital Database") is developed and operated by the hospital or clinic that deploys it ("we", "our"). It is intended for use by authorized healthcare staff only and is not a consumer health app.

If you are a patient, please contact your hospital directly for questions about how your data is handled.

## 2. What this app does

Hospital Database is an internal tool for authorized staff to:

- Register outpatient (OPD) and inpatient (IPD) visits.
- Record history, examination, investigations, imaging, treatments, operations, and discharge summaries.
- Manage birth records and related notes.
- Track vital signs and other clinical parameters.
- Coordinate investigations and OT calls using notifications.

It is **not** intended for direct patient use or self‑diagnosis.

## 3. Data we collect and process

The app is designed to store and process personal and health information about patients, including but not limited to:

- Identifiers: patient ID, hospital ID, OPD/Admission numbers, dates of birth, sex.
- Contact and demographic information: names, addresses, age, gender.
- Clinical data: history, examination findings, diagnoses, investigations, imaging results, treatments, operations, discharge summaries, birth records, and follow‑up notes.
- Vital signs and other observations recorded during care.
- Technical logs and metadata: timestamps of actions, basic device information, and limited analytics as configured by the hospital.

The exact data stored depends on how your hospital configures and uses the app.

## 4. How and where data is stored

The app uses a combination of:

- **Cloud Firestore (Google Firebase)** – for primary storage of clinical records, notifications, and configuration.
- **Firebase Storage** – for selected files such as hospital logos or imaging exports if configured.
- **Local databases on the device (Room/SQLite)** – for caching and offline access to selected records, vital signs, and settings.

All network communication with Firebase uses HTTPS/TLS.

Access to the Firebase project is restricted to the hospital's authorized administrators and infrastructure.

## 5. How we use the data

Data entered into the app is used for purposes such as:

- Providing and documenting clinical care to patients.
- Managing hospital workload, bed occupancy, and OT scheduling.
- Generating internal reports and summaries.
- Sending internal notifications to staff about investigations, imaging, and OT calls.

We do **not** use patient data for advertising or unrelated marketing.

## 6. Sharing and disclosure

Patient data recorded in this app is generally only shared with:

- Authorized hospital staff and departments involved in direct patient care.
- External providers only to the extent required by law or as part of the hospital's official referral/consult process.

We do not sell patient data.

Third‑party services used by this app (for example Google Firebase) act as data processors on behalf of the hospital. They may process data only according to contractual terms and applicable law.

## 7. Legal basis and consent

The legal basis for processing patient data through this app is typically:

- Provision of healthcare and treatment.
- Compliance with legal obligations regarding medical record‑keeping.
- Legitimate interests of the hospital in managing operations and patient safety.

The exact legal basis depends on your jurisdiction and your hospital's policies.

## 8. Data retention

Medical records are retained in accordance with the hospital's retention policy and local laws. This may include long‑term or permanent retention of certain records.

Technical logs or notifications may be retained for a shorter period, as required for operational and audit purposes.

## 9. Security

We implement reasonable technical and organizational safeguards, including:

- Authentication for staff access (e.g., username/password or other mechanisms configured by the hospital).
- Partitioned Firebase projects and access control for administrators.
- Encrypted connections (HTTPS/TLS) between app and backend.
- Limited logging of sensitive data.

No system can be 100% secure. The hospital continuously reviews and improves security measures.

## 10. Your rights

Depending on your jurisdiction, patients may have rights to:

- Access their personal data.
- Request correction of inaccurate data.
- Request deletion or restriction of processing, subject to legal and medical record‑keeping requirements.

To exercise these rights, patients should contact the hospital directly using the contact details below.

## 11. Contact

This application is used by multiple hospitals and clinics.

For questions about this app or how your data is handled, patients should contact **the specific hospital or clinic where they received care** and where this app is being used. That hospital or clinic is responsible for:

- Acting as the data controller for the patient records it creates in this app.
- Providing its own official contact details (address, email, phone) for privacy and data‑protection questions.
- Responding to requests to access, correct, or delete medical records in accordance with local law and its internal policies.

If you are a hospital or clinic administrator deploying this app, please ensure that your staff and patients know how to reach your official contact point for medical records and privacy matters (for example, by publishing it on your own website, admission forms, or notice boards).

## 12. Changes to this policy

We may update this policy from time to time. The "Last updated" date at the top will indicate the latest revision. Significant changes may also be communicated through internal channels.

---

**Implementation note for developers/administrators:**

1. Review and customize this file, then host the final version on a publicly reachable URL (for example on your hospital's website or GitHub Pages).
2. Update the `privacy_policy_url` string in `app/src/main/res/values/strings.xml` to point to that URL.
3. Use that same URL in the Google Play Console for the app listing and Data Safety form.
