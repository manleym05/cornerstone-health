# Privacy Policy

**Last updated: 12 August 2026**

Cornerstone Health is a personal health dashboard operated by an individual ("we", "us").
This policy describes exactly what data the service collects, where it is stored, who can
see it, and how to have it deleted.

It is written to describe the system as actually built. If the system changes, this document
changes with it.

## Who operates this service

Cornerstone Health is an individual's personal project, not a company. Contact:
**manleym05@gmail.com**.

## What we collect

**From your Öura account, with your explicit consent, we request two permission scopes:**

| Scope | What it grants | What we actually read |
|---|---|---|
| `personal` | Basic profile information | Used to associate your data with your account |
| `daily` | Daily summary metrics | Readiness score, sleep score, HRV balance, resting heart rate |

For each day, we store a single record containing: the date, readiness score, sleep score,
HRV balance, resting heart rate, and the time the record was retrieved.

**We do not request, receive, or store:** heart-rate detail, workouts, tags, sessions, SpO2,
stress, heart-health, ring configuration, or your email address from Öura.

**From your use of the service, we store:** your account identifier, email address, and
password credentials — all held by Amazon Cognito, an AWS identity service. We never see or
store your password ourselves.

**We do not collect:** location data, device identifiers, advertising identifiers, browsing
behaviour, or analytics of any kind. There are no third-party trackers, cookies for
advertising, or marketing pixels.

## Access tokens

Connecting your Öura account produces an access token and a refresh token. These are:

- Exchanged and held **entirely on the server**. They are never sent to your browser, never
  written into a web page, and never stored on your device.
- **Encrypted before storage** using AWS Key Management Service (envelope encryption), on top
  of the storage layer's own encryption at rest.
- Never logged, and never included in any error message or API response.

## Where your data is stored

All data is stored in Amazon Web Services (AWS), in the United States, in an AWS account
controlled by the operator. Specifically:

- **Amazon DynamoDB** — your daily records and your encrypted tokens. Encrypted at rest.
- **Amazon Cognito** — your sign-in credentials.
- **AWS Key Management Service** — the encryption key protecting your tokens.

Data is logically separated per user: every record is keyed to your account identifier, and
the service has no operation that returns one user's data to another user.

## Who your data is shared with

**Nobody.** Your health data is not sold, rented, shared, or disclosed to any third party.
There are no advertisers, no data brokers, no analytics providers, and no partners.

The only third party involved is **Amazon Web Services**, which hosts the infrastructure and
stores the data on our behalf as a processor. AWS does not access or use your data.

We may disclose data if legally compelled to do so by valid legal process, or where necessary
to protect someone's safety.

## How long we keep it

Your daily records are kept for as long as your account exists. There is no automatic
expiry today.

If you disconnect Öura, we stop collecting new data immediately, and the stored access tokens
become unusable.

If you delete your account, all of your data — records, tokens, and account — is deleted.

## Your rights and choices

You can, at any time:

- **Disconnect Öura** from your Öura account's connected-applications page, revoking access
  immediately.
- **Request a copy** of everything stored about you.
- **Request deletion** of your account and all associated data.
- **Ask what is stored** and get a straight answer.

Email **manleym05@gmail.com** for any of these. Requests are honoured within 30 days, and in
practice much sooner.

Depending on where you live, you may have additional rights under laws such as the GDPR or
CCPA. We will honour those rights regardless of where you live.

## Security

- Health data and tokens are encrypted at rest.
- Öura tokens receive an additional layer of application-level encryption.
- Access requires authentication; each request is authorised against your own account only.
- Only the minimum necessary Öura permissions are requested.

No system is perfectly secure, and this is a personal project rather than a commercial
service with a dedicated security team. That is a reason to be candid about it rather than
to imply otherwise. If you discover a security problem, please email the address above.

## Children

This service is not intended for anyone under 16, and we do not knowingly collect data from
children.

## Changes

If this policy changes materially, the date at the top will be updated and, where the change
affects how your data is handled, we will contact you directly at your registered email.

## Contact

**manleym05@gmail.com**
