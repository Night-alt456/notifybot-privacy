# NotifyBot Privacy Policy

Last updated: October 20, 2026

## Overview

NotifyBot does not collect personal information about community members; it only stores the settings a community's managers give it. NotifyBot is a bot for [Root](https://rootapp.com) that posts a message, and optionally pings a role, when a watched Twitch or Kick streamer goes live or a watched YouTube channel posts a video or goes live.

This policy explains what the bot stores, who it talks to, and how to have your data removed. It applies to every Root community where NotifyBot is installed. Effective date: October 20, 2026.

## What the bot stores

The bot stores one settings record per community, in the key-value store that Root provides to every bot. It contains:

- The ID of the channel where announcements are posted, and the ID and name of the role to ping.
- The list of watched channels: platform (Twitch, Kick or YouTube), the channel name or ID, the display name, whether the streamer was last seen live, and the IDs of recently seen YouTube videos.
- Housekeeping: the time of the last check, the time the welcome message was posted, and the text of the last error for each watched channel.

The bot also receives the Root user ID of anyone who runs a `/announce` command, to check whether that person is a bot manager. That ID is used for the check only and is not saved. The bot does not store or log the content of other chat messages, and it does not collect names, email addresses, IP addresses, or any other details about community members.

## How the data is used

The stored settings are used for one purpose: deciding when to post an announcement and where to post it. Every couple of minutes the bot checks each watched channel, compares the result with what it remembers, and posts only when something is new.

The bot does not sell or share data, show ads, build profiles, or use any data for analytics or marketing.

## Third-party services

The bot contacts four outside services, and none of these requests include information about community members. They carry only the public channel name or ID being checked, plus the bot's own credentials.

- **Root** hosts the bot, stores its settings, and delivers its messages. Root's own terms and privacy policy apply to that data.
- **Twitch** and **Kick**: the bot asks whether a given streamer is live. Their own privacy policies apply.
- **YouTube**: the bot reads YouTube's public channel feeds and pages, and may use the YouTube API Services for channel lookups and live checks. By using the bot you are also subject to the [YouTube Terms of Service](https://www.youtube.com/t/terms), and Google handles data under the [Google Privacy Policy](https://policies.google.com/privacy).

## Retention and deletion

A community's settings are kept until a manager removes them or the bot is uninstalled. A manager can remove any watched channel at any time with `/announce remove`, which deletes that entry from the stored settings. When the bot is uninstalled, its stored data is handled according to Root's rules for bot data.

To ask for your community's data to be deleted, or to ask what is stored, contact me using the details below.

## Security, children, changes and contact

Only people in the community's "Bot managers" setting can run `/announce` commands, and the bot only has permission to post messages and mention roles in the channels it is allowed to use. No system is perfectly secure, but the bot keeps as little data as it can.

NotifyBot is not directed at children and knowingly collects no information from anyone, children included. Use of Root itself is governed by Root's age requirements.

If this policy changes, the new version will be posted here with an updated effective date.

Questions or deletion requests: Night002 - On Root.
