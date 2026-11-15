---
title: Crosstalk — Privacy policy
version: 0.10.1-draft
effective_date: TBD
status: draft, not in force
---
# Crosstalk — Privacy policy

> Draft for review. Not in force until Fedor AB publishes it with an effective date. Text in [square brackets] is waiting for a decision by Fedor AB.

This policy is also available in Swedish: [Integritetspolicy](sv/privacy).

## 1. Who is responsible

Fedor AB (org. nr 559537-2961) is the controller of the personal data described here. Contact for anything about your data: <privacy@fedor.nu>. Postal address: Fedor AB, Fabriksvägen 8, 176 69 Järfälla, Sweden.

Crosstalk is offered in countries of the European Union and the European Economic Area, and this policy is written for listeners there.

## 2. The short version

- You do not create an account with us. We do not ask for your name, email address or phone number.
- To use Crosstalk you need a Crosstalk purchase in the App Store. Apple handles the payment, and we never see your payment details.
- To write what the hosts say, the app sends our server the details of the tracks around your current position, your time zone and language, and your preferences for the hosts.
- Our server passes that information to an AI provider that writes the script, and passes the script to an AI provider that turns it into speech. The app asks for your permission before this happens.
- We use AI tools from outside companies to help us run and repair the service. While they do that work, they can read what our database holds about your listening, stored under a random identifier. They are not given the logs that contain your IP address.
- We keep a history of the host segments you heard, tied to a random identifier and not to your name.
- We do not use advertising or tracking tools, we do not use outside analytics services, and we do not sell data. [When crash reports and usage statistics are available: we collect them ourselves, on our own server (section 3.5). Usage statistics are collected only if you switch them on.]

## 3. What we process and why

### 3.1 Sent each time a host segment is requested

| Data | Details | Why |
|---|---|---|
| The tracks around you | For the track that just played and the one coming next: title, artist names, album, year and release date, genre, explicit/clean rating, track and disc numbers, composer and the recording code (ISRC). | So the hosts can talk about the music. |
| What you are playing from | The type (playlist, album or collection), its title, and up to 21 tracks around your current position. A playlist title is whatever you named it. | So the hosts know the context of the track. |
| Time | The time the segment starts and your time zone. | So the hosts know the time of day and the day of the week. |
| Language | The show's language, the languages set on your device and the host language you chose, if any. | To pick the language the hosts speak. |
| Your preferences for the hosts | What you set for the hosts in Settings, including any free text you wrote for them. | So the hosts can follow them. |
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
| Sessions and paging markers | The short-lived session token (section 3.2) and the markers the app uses to page through your host history. | Until they expire |
| Identifiers | The listener identifier and the app integrity key with Apple's proof for it. | The app integrity key: 90 days after it was last used. The listener identifier: until nothing we store refers to it. |
| Fault-finding capture | The complete text sent to the AI provider and its reply, including your preferences for the hosts. Switched off in normal operation; we switch it on only to investigate a fault. | 30 days |
| Server and network logs | Technical records of requests and errors: time, address requested, result, your IP address, the app and system version your device reports, and the app integrity key reference. [To be confirmed on the production server: logs contain no track details and no text you wrote for the hosts.] | 14 days |

[When the "Build your own show" feature is available: the description of the station and hosts that you write, the result of our automatic check of it, and the accepted world, which is stored on your device.]

### 3.4 Kept only on your device

The app stores the following on your device and nowhere else:

- your settings: your preferences for the hosts, the show and host language you chose, and how your library is sorted. Your preferences for the hosts are sent with each request for a host segment (section 3.1) and are not stored on our server, except inside a fault-finding capture (section 3.3);
- a list of up to 25 albums and playlists you opened recently, as references without titles;
- a reference to the app integrity key;
- the audio of a host segment while it plays, and, if a segment was interrupted, that audio together with the title, artist and album of the track that follows it, so that the segment can resume.

Deleting the app removes this data. [To be confirmed: except the listener identifier, if it is kept in your iCloud Keychain.] [When usage statistics are available: and except the analytics identifier, see section 3.5.]

### 3.5 Crash reports and usage statistics

[This section applies when these two features are available. Usage statistics are off until you switch them on. Crash reports have their own switch in Settings. It starts on or off depending on the country of your App Store, and Settings shows which. The app reads that country on your device and does not send it to us.]

**Crash reports.** After a crash or a freeze the app sends our server the technical report that iOS prepared: which part of the app's code was running (the stack trace), the app version and build, the device model and the iOS version. Before sending, the app removes the region, process numbers, memory addresses, the text of error messages and the exact time. We use a report only to find and fix the fault. The report carries no identifier. [To be confirmed on the production server: no log line ties a report to your IP address or to your app integrity key.] We keep a report for 90 days. You can switch crash reports off in Settings.

**Usage statistics.** If you switch them on, the app sends our server a short list of events: when playback starts, how long it takes until you hear sound, when a host segment starts and ends, when you skip, when you switch the hosts on or off, and the steps from setup to purchase. Each event carries an analytics identifier, a random number that the app creates when you agree. The analytics identifier is a different number from your listener identifier, but the two can be linked: events such as the start and end of a host segment carry the time, and your host history records when each segment aired. Anyone who reads both, including the AI tools in section 5, can match them by time. We use the events to see how the app performs and to improve it. We also use the analytics identifier to give different listeners different versions of a feature and compare the results.

The analytics identifier is kept in the keychain of your device. It stays there if you delete the app, and after you install the app again it is used only if you agree again. Switching usage statistics off removes it from your device and deletes the events stored under it on our server at once. Your purchase, your host history and your preferences for the hosts are not affected. We keep events for 90 days, and we delete everything stored under an analytics identifier after 90 days without activity.

We run both on our own server. No outside analytics company receives this data. The AI tools that help us run the service (section 5) can read it.

## 4. Legal basis

- **Performing our agreement with you** (GDPR Article 6(1)(b)). Checking your purchase, generating host segments, keeping your host history and giving the hosts continuity are what you ask Crosstalk to do under the [terms of use](terms).
- **Our legitimate interests** (Article 6(1)(f)). We have an interest in keeping the service secure, preventing abuse and keeping the service working. This covers the app integrity check, limits on how often segments can be generated, logs, fault-finding, and the use of AI tools to monitor and repair the service (section 5). [If we count active installs: it also covers counting how many copies of the app were active in the last 30 days. We count the listener identifiers seen in that time and keep only the total.] [When crash reports are available: where the switch starts on, it also covers finding and fixing faults from crash reports (section 3.5).] You can object to this processing; see section 8.
- **Your consent** (Article 6(1)(a)). [When available:] usage statistics, and crash reports where the switch starts off and you turn it on (section 3.5). You can withdraw it at any time by switching them off in Settings. That does not affect what was done before.

Before the first host segment, the app asks you to allow sharing with AI services. The screen says in short what is shared and why, and this policy gives the details: the data in section 3.1 and the recipients in section 5. Your permission covers the AI providers that write and voice the hosts and the AI tools that help us run the service. Without that permission the hosts cannot work, and none of the data in section 3.1 is sent to our server or to any AI provider. You can change your choice at any time in Settings. Switching the hosts off stops new data from being sent. What is already stored stays for the periods in section 3.3 and can still be read by the AI tools in section 5; you can ask us to delete it (section 8).

The app still contacts our server when it starts, to check that your version is supported and that the app is genuine. That contact leaves the technical records listed under "Server and network logs" in section 3.3. The AI tools in section 5 are not given those logs.

## 5. Who receives your data

We use other companies in four roles. Each of them is our processor: it acts on our instructions and may not use your data for its own purposes. [To be confirmed for each company when its contract is signed.]

| Role | Company | What it receives | Purpose |
|---|---|---|---|
| Script-writing AI | [Company to be added when the contract is signed. We expect to use one of Anthropic's Claude models, bought either from Anthropic or through a cloud provider.] | The text we assemble for the script: the track and playlist details, the time, your preferences for the hosts, the show's description, and the scripts of your most recent segments. No identifier of you is included. | Writing the hosts' script. |
| Speech AI | Google [contracting company to be added when the contract is signed] | The finished script, the chosen voices and the language. No identifier of you is included. | Turning the script into speech. |
| Hosting | [Cloud provider to be added] | Everything our server stores. | Running our server, in [EU region]. |
| AI tools that help us operate the service | [Companies to be named here when they are chosen.] Providers of AI models and AI coding tools, which are American groups. We use them under business terms that make them our processors. | What a tool reads while it works: the database behind the service as it is, except the tables that hold app integrity keys and session tokens, which are closed to the tools. That includes your host history, request records and paging markers (section 3.3), stored under your listener identifier. [When crash reports and usage statistics are available: the tools can also read those reports and events (section 3.5).] Your preferences for the hosts are not stored in the database. A fault-finding capture, when one is switched on, contains them, so a tool can then read personal details you wrote for the hosts. We do not hold your name or your Apple Account, so a tool cannot see them. The tools are not given the server and network logs, which contain IP addresses. | Monitoring the service, finding and repairing faults, and maintaining it. |

Our contracts with the AI providers do not allow them to train their models on your data. [To be confirmed against each signed contract.]

If we add or replace a company in this table, we publish a new version of this policy first, and the app tells you about the change. You can ask us at any time which companies have received your data.

Apple is involved as an independent provider, not as our processor: Apple delivers the app, sells you the purchase and takes the payment, plays the music through your Apple Music subscription, and issues the app integrity proof. Apple's privacy policy applies to what Apple does.

We share data with authorities only when the law requires it.

## 6. Transfers outside the EU/EEA

Our own server runs at a cloud provider inside the EU: [provider and region to be added].

The AI providers and the providers of AI tools in section 5 are American groups. Even where our contract is with a provider's European company, that company and its affiliates may process data in the United States and other countries. Such transfers are covered by the European Commission's standard contractual clauses or, for US companies certified under it, by the EU-US Data Privacy Framework. You can ask us for a copy of the safeguards.

## 7. How long we keep data

The periods are listed in section 3.3. When a period ends we delete the data. If you ask us to delete your data, we delete your host history, your request records and your identifiers without waiting for those periods to end [and, when usage statistics are available, your usage events].

The AI providers keep the content we send them for a limited time under their own terms, to detect misuse, and then delete it. [Periods to be confirmed against the signed contracts.]

## 8. Your rights

You have the right to:

- get a copy of the personal data we hold about you;
- have incorrect data corrected;
- have your data deleted;
- have our use of your data restricted;
- receive the data you provided in a portable format;
- object to processing that we base on our legitimate interests;
- withdraw a consent you gave, at any time. [When usage statistics are available: by switching them off in Settings.]

Because you have no account with us, we can only find your data through the listener identifier in your app. Write to <privacy@fedor.nu>. [When usage statistics are available: your usage events are stored under the analytics identifier, so send us that identifier as well. Without it we look for them by matching their times with your host history.] [To be added when built: how to delete your data from the app's Settings, and where the app shows your identifier.] We answer within one month.

You can also complain to the Swedish Authority for Privacy Protection (Integritetsskyddsmyndigheten, IMY), <https://www.imy.se>, or to the data protection authority in the country where you live.

## 9. Children

Crosstalk is for adults. You must be at least 18 years old. The app is rated 18+ in the App Store, and we do not knowingly process data about anyone younger.

## 10. Automated checks

[When the "Build your own show" feature is available: a world you create is checked automatically against our rules before it can be used. You can ask a person to look at a refusal by writing to us.]

We do not make decisions about you that have legal or similarly significant effects by automated means.

## 11. Security

Data travels between the app and our server over an encrypted connection. Requests are accepted only from a genuine copy of the app. Access to the server and the data on it is limited to the people at Fedor AB who run the service and to the AI tools they use for that work, described in section 5.

## 12. Changes to this policy

Each version has a version number and an effective date at the top. If we make a material change, the app will tell you and, where needed, ask you to accept the new version. Earlier versions remain available at <https://legal.fedor.nu/crosstalk/>.
