---
title: Crosstalk — Privacy policy
version: 0.1.0-draft
effective_date: TBD
status: draft, not in force
---
# Crosstalk — Privacy policy

> Draft for review. Not in force until Fedor AB publishes it with an effective date. Text in [square brackets] is waiting for a decision by Fedor AB.

## 1. Who is responsible

Fedor AB (org. nr 559537-2961, Järfälla, Sweden) is the controller of the personal data described here. Contact: [contact email]. Postal address: [postal address].

## 2. The short version

- Crosstalk has no user accounts. We do not ask for your name, email address or phone number.
- To write what the hosts say, the app sends our server the details of the tracks around your current position, your time zone and language, and any note you wrote to the hosts.
- Our server passes that information to an AI provider that writes the script, and passes the script to a second AI provider that turns it into speech. The app asks for your permission before this happens.
- We keep a history of the host segments you heard, tied to a random identifier and not to your name.
- We do not use advertising, analytics or tracking tools, and we do not sell data.

## 3. What we process and why

### 3.1 Sent each time a host segment is requested

| Data | Details | Why |
|---|---|---|
| The tracks around you | For the track that just played and the one coming next: title, artist names, album, year and release date, genre, explicit/clean rating, track and disc numbers, composer and the recording code (ISRC). | So the hosts can talk about the music. |
| What you are playing from | The type (playlist, album or collection), its title, and up to 21 tracks around your current position. A playlist title is whatever you named it. | So the hosts know the context of the track. |
| Time | The time the segment starts and your time zone. | So the hosts know the time of day and the day of the week. |
| Language | The show's language, the languages set on your device and the host language you chose, if any. | To pick the language the hosts speak. |
| Your note | Free text you typed for the hosts in Settings, if any. | So the hosts can respond to it. |
| App details | The app's identifier and version. | To check that your version of the app is supported. |

We do not receive your Apple Music library, your listening history beyond the tracks listed above, your Apple Account, your location or your contacts.

### 3.2 Identifiers

| Data | Details | Why |
|---|---|---|
| Listener identifier | A random identifier. It is not your name or your Apple Account. [To be confirmed: whether it is created per installation or kept in your iCloud Keychain and shared by your devices.] | To keep your host history together and to give the hosts continuity from one segment to the next. |
| App integrity key | Created by Apple's App Attest service on your device, together with the proof Apple issues for it. | To confirm that requests come from a genuine copy of the app, and to prevent abuse. |
| Session token | A short-lived token, valid for at most 15 minutes. | To authorise requests. |
| [Entitlement proof] | [A signed App Store transaction record, if access to Crosstalk depends on an App Store purchase.] | [To confirm that you are entitled to use the service.] |
| Network address | Your IP address, as with any internet connection. | To deliver responses and to protect the service. |

### 3.3 Created and kept by us

| Data | Details | Kept for |
|---|---|---|
| Host history | For each segment you heard: when it aired, the title, artist and album of the track before it, the script, the hosts' names and a short internal summary used for continuity. | [Retention period to be decided] |
| Segments you did not hear | The same record for a segment that was generated but never played. | 24 hours |
| Audio of a segment | The generated audio, held so that the app can fetch it again if the connection drops. | 15 minutes |
| Request records | Which requests were made, when, and whether they succeeded. They contain the listener identifier and no track details. | [Retention period to be decided] |
| Fault-finding capture | The complete text sent to the AI provider and its reply. [To be confirmed: switched off in normal operation and switched on only for a limited time to investigate a fault.] | 30 days |
| Server and network logs | Technical records of requests: time, address requested, result, your IP address, the app and system version your device reports, and the app integrity key reference. [To be confirmed for the production server: the exact fields, and that logs contain no track details and no note text.] | [Retention period to be decided] |

[When the "Build your own show" feature is available: the description of the station and hosts that you write, the result of our automatic check of it, and the accepted world, which is stored on your device.]

### 3.4 Kept only on your device

The app stores the following on your device and nowhere else:

- your settings: your note to the hosts, the show and host language you chose, and how your library is sorted;
- a list of up to 25 albums and playlists you opened recently, as references without titles;
- a reference to the app integrity key;
- the audio of a host segment while it plays, and, if a segment was interrupted, that audio together with the title, artist and album of the track that follows it, so that the segment can resume.

Deleting the app removes this data. [To be confirmed: except the listener identifier, if it is kept in your iCloud Keychain.]

## 4. Legal basis

- **Performing our agreement with you** (GDPR Article 6(1)(b)). Generating host segments, keeping your host history and giving the hosts continuity are what you ask Crosstalk to do under the [terms of use](terms).
- **Our legitimate interests** (Article 6(1)(f)). We have an interest in keeping the service secure and preventing abuse. This covers the app integrity check, limits on how often segments can be generated, logs, and fault-finding. You can object to this processing; see section 8.

Before the first host segment, the app asks you to confirm that the data in section 3.1 may be sent to the AI providers in section 5. Without that confirmation the hosts cannot work, and none of that data is sent to our server or to the AI providers. The app still contacts our server when it starts, to check that your version is supported and that the app is genuine.

## 5. Who receives your data

We use these companies as processors. They act on our instructions and may not use your data for their own purposes.

| Recipient | What they receive | Purpose |
|---|---|---|
| Anthropic (Anthropic Ireland, Limited) | The text we assemble for the script: the track and playlist details, the time, your note, the show's description, and the scripts of your most recent segments. No identifier of you is included. | Writing the hosts' script. |
| Google ([Google Cloud EMEA Limited]) | The finished script, the chosen voices and the language. No identifier of you is included. | Turning the script into speech. |
| [Hosting provider] | Everything our server stores. | Running our server. |

Under Anthropic's commercial terms, Anthropic may not train its models on this content. Under Google's terms for its paid service, Google does not use this content to improve its products.

Apple is involved as an independent provider, not as our processor: Apple delivers the app, plays the music through your Apple Music subscription, and issues the app integrity proof. Apple's privacy policy applies to what Apple does.

We share data with authorities only when the law requires it.

## 6. Transfers outside the EU/EEA

Our contracts are with these providers' European companies, but they and their affiliates may process data in the United States and other countries. Such transfers are covered by the European Commission's standard contractual clauses or, for US companies certified under it, by the EU-US Data Privacy Framework. You can ask us for a copy of the safeguards.

[Our own server is located in [country].]

## 7. How long we keep data

The periods are listed in section 3.3. When a period ends we delete the data or make it anonymous. If you ask us to delete your data, we delete your host history, your request records and your identifiers.

Anthropic and Google keep the content we send them for a limited time under their own terms, to detect misuse, and then delete it. [Periods to be confirmed against the signed contracts.]

## 8. Your rights

You have the right to:

- get a copy of the personal data we hold about you;
- have incorrect data corrected;
- have your data deleted;
- have our use of your data restricted;
- receive the data you provided in a portable format;
- object to processing that we base on our legitimate interests.

Because Crosstalk has no accounts, we can only find your data through the identifier in your app. [Use "Delete my data" in the app's Settings, or send us the identifier shown there.] Write to [contact email]. We answer within one month.

You can also complain to the Swedish Authority for Privacy Protection (Integritetsskyddsmyndigheten, IMY), <https://www.imy.se>, or to the data protection authority in the country where you live.

## 9. Children

Crosstalk is for adults. You must be at least [18] years old to use it, and we do not knowingly process data about anyone younger.

## 10. Automated checks

[When the "Build your own show" feature is available: a world you create is checked automatically against our rules before it can be used. You can ask a person to look at a refusal by writing to us.]

We do not make decisions about you that have legal or similarly significant effects by automated means.

## 11. Security

Data travels between the app and our server over an encrypted connection. Requests are accepted only from a genuine copy of the app. Access to the server is limited to Fedor AB.

## 12. Changes to this policy

Each version has a version number and an effective date at the top. If we make a material change, the app will tell you and, where needed, ask you to accept the new version. Earlier versions remain available at <https://legal.fedor.nu/crosstalk/>.
