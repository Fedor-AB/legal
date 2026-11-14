---
title: Crosstalk — Privacy policy
version: 0.3.1-draft
effective_date: TBD
status: draft, not in force
---
# Crosstalk — Privacy policy

> Draft for review. Not in force until Fedor AB publishes it with an effective date. Text in [square brackets] is waiting for a decision by Fedor AB.

## 1. Who is responsible

Fedor AB (org. nr 559537-2961) is the controller of the personal data described here. Contact for anything about your data: <privacy@fedor.nu>. Postal address: Fedor AB, Fabriksvägen 8, 176 69 Järfälla, Sweden.

## 2. The short version

- You do not create an account with us. We do not ask for your name, email address or phone number.
- To use Crosstalk you need a Crosstalk purchase in the App Store. Apple handles the payment, and we never see your payment details.
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
| Listener identifier | A random identifier that the app creates and attaches to your App Store purchase of Crosstalk. It is not your name or your Apple Account. [To be confirmed when this part of the app is built: the identifier is kept in your iCloud Keychain, so your devices share it and it survives reinstalling the app.] | To keep your host history together and to give the hosts continuity from one segment to the next. |
| App integrity key | Created by Apple's App Attest service on your device, together with the proof Apple issues for it. | To confirm that requests come from a genuine copy of the app, and to prevent abuse. |
| Session token | A short-lived token, valid for at most 15 minutes. | To authorise requests. |
| Purchase record | The signed App Store transaction record for your Crosstalk purchase. Our server reads from it the app identifier, the product, the expiry date, whether the purchase was refunded or revoked, and the listener identifier. It contains no name, no Apple Account and no payment details. We check the record and do not keep it. | To confirm that you are entitled to use the service. |
| Network address | Your IP address, as with any internet connection. | To deliver responses and to protect the service. |

### 3.3 Created and kept by us

| Data | Details | Kept for |
|---|---|---|
| Host history | For each segment you heard: when it aired, the title, artist and album of the track before it, the script, the hosts' names and a short internal summary used for continuity. | 90 days |
| Segments you did not hear | The same record for a segment that was generated but never played. | 24 hours |
| Audio of a segment | The generated audio, held so that the app can fetch it again if the connection drops. | 15 minutes |
| Request records | Which requests were made, when, and whether they succeeded. They contain the listener identifier and no track details. | 30 days |
| Identifiers | The listener identifier and the app integrity key with Apple's proof for it. | [Retention period to be decided] |
| Fault-finding capture | The complete text sent to the AI provider and its reply. [To be confirmed: switched off in normal operation and switched on only for a limited time to investigate a fault.] | 30 days |
| Server and network logs | Technical records of requests and errors: time, address requested, result, your IP address, the app and system version your device reports, and the app integrity key reference. [To be confirmed on the production server: logs contain no track details and no note text.] | 14 days |

[When the "Build your own show" feature is available: the description of the station and hosts that you write, the result of our automatic check of it, and the accepted world, which is stored on your device.]

### 3.4 Kept only on your device

The app stores the following on your device and nowhere else:

- your settings: your note to the hosts, the show and host language you chose, and how your library is sorted;
- a list of up to 25 albums and playlists you opened recently, as references without titles;
- a reference to the app integrity key;
- the audio of a host segment while it plays, and, if a segment was interrupted, that audio together with the title, artist and album of the track that follows it, so that the segment can resume.

Deleting the app removes this data. [To be confirmed: except the listener identifier, if it is kept in your iCloud Keychain.]

## 4. Legal basis

- **Performing our agreement with you** (GDPR Article 6(1)(b)). Checking your purchase, generating host segments, keeping your host history and giving the hosts continuity are what you ask Crosstalk to do under the [terms of use](terms).
- **Our legitimate interests** (Article 6(1)(f)). We have an interest in keeping the service secure and preventing abuse. This covers the app integrity check, limits on how often segments can be generated, logs, and fault-finding. You can object to this processing; see section 8.

Before the first host segment, the app asks you to confirm that the data in section 3.1 may be sent to the AI providers in section 5. Without that confirmation the hosts cannot work, and none of that data is sent to our server or to the AI providers. The app still contacts our server when it starts, to check that your version is supported and that the app is genuine.

## 5. Who receives your data

We use these companies as processors. They act on our instructions and may not use your data for their own purposes.

| Recipient | What they receive | Purpose |
|---|---|---|
| Anthropic (Anthropic Ireland, Limited) | The text we assemble for the script: the track and playlist details, the time, your note, the show's description, and the scripts of your most recent segments. No identifier of you is included. | Writing the hosts' script. |
| Google ([Google Cloud EMEA Limited]) | The finished script, the chosen voices and the language. No identifier of you is included. | Turning the script into speech. |
| [Cloud provider: name to be added] | Everything our server stores. | Running our server, in [EU region]. |

Under Anthropic's commercial terms, Anthropic may not train its models on this content. Under Google's terms for its paid service, Google does not use this content to improve its products.

Apple is involved as an independent provider, not as our processor: Apple delivers the app, handles your purchase and payment, plays the music through your Apple Music subscription, and issues the app integrity proof. Apple's privacy policy applies to what Apple does.

We share data with authorities only when the law requires it.

## 6. Transfers outside the EU/EEA

This section describes how data leaves the EU. It applies to every listener, because all listeners' data is handled in the same systems.

Our contracts are with these providers' European companies, but they and their affiliates may process data in the United States and other countries. Such transfers are covered by the European Commission's standard contractual clauses or, for US companies certified under it, by the EU-US Data Privacy Framework. You can ask us for a copy of the safeguards.

Our own server runs at a cloud provider inside the EU: [provider and region to be added].

## 7. How long we keep data

The periods are listed in section 3.3. When a period ends we delete the data. If you ask us to delete your data, we delete your host history, your request records and your identifiers without waiting for those periods to end.

Anthropic and Google keep the content we send them for a limited time under their own terms, to detect misuse, and then delete it. [Periods to be confirmed against the signed contracts.]

## 8. Your rights

You have the right to:

- get a copy of the personal data we hold about you;
- have incorrect data corrected;
- have your data deleted;
- have our use of your data restricted;
- receive the data you provided in a portable format;
- object to processing that we base on our legitimate interests.

Because you have no account with us, we can only find your data through the listener identifier in your app. Write to <privacy@fedor.nu>. [To be added when built: how to delete your data from the app's Settings, and where the app shows your identifier.] We answer within one month.

You can also complain to the Swedish Authority for Privacy Protection (Integritetsskyddsmyndigheten, IMY), <https://www.imy.se>, or to the data protection authority in the country where you live.

### 8.1 If you live outside the EU and EEA

Crosstalk is offered in App Store countries around the world. The [terms of use](terms) list the countries where it is not offered. We apply this policy, and the rights listed above, to every listener wherever they live. Your own country's law may give you further rights, and nothing here takes them away.

- **Switzerland.** The Federal Act on Data Protection applies. You can turn to the Federal Data Protection and Information Commissioner, <https://www.edoeb.admin.ch>.
- **United States.** We do not sell your personal data, and we do not share it for advertising. We use it only for the purposes in section 3 and disclose it only to the recipients in section 5. If the law of your state gives you rights to know, correct or delete your data, use the contact above, and we will not treat you differently for doing so.
- **Other countries.** Contact us in the same way. We will handle your request under this policy and under the law that applies to you.

Wherever you live, your data is processed in the EU, where our server is, and in the countries where our AI providers operate, including the United States.

## 9. Children

Crosstalk is for adults. You must be at least 18 years old, or the age of majority where you live if that is higher. The app is rated 18+ in the App Store, and we do not knowingly process data about anyone younger.

[To be added when built: in places where the law requires an app to confirm that its users are adults, the app asks Apple for your age range. Apple tells the app only the range, never your date of birth.]

## 10. Automated checks

[When the "Build your own show" feature is available: a world you create is checked automatically against our rules before it can be used. You can ask a person to look at a refusal by writing to us.]

We do not make decisions about you that have legal or similarly significant effects by automated means.

## 11. Security

Data travels between the app and our server over an encrypted connection. Requests are accepted only from a genuine copy of the app. Access to the server is limited to Fedor AB.

## 12. Changes to this policy

Each version has a version number and an effective date at the top. If we make a material change, the app will tell you and, where needed, ask you to accept the new version. Earlier versions remain available at <https://legal.fedor.nu/crosstalk/>.
