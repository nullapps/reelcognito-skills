# ReelCognito · Mystery Movie Nights

Let your AI shopping agent choose a movie for you. Pick the theater, time and budget, approve a schedule without seeing the title, and take a mystery ticket to the theater. You can discover the film when it starts on screen.

Muse is the first shopping agent covered by this repository. It interviews you about your tastes, films you have seen, seats, budget and spoiler preferences. After you confirm your rules, Muse can propose a night out and ask for approval of the specific purchase. Your agent books with the merchant. ReelCognito turns the purchased ticket into a mystery pass for Apple Wallet or Google Wallet when issuance succeeds. The pass shows “Mystery Movie” through the previews. Its title update is scheduled for 30 minutes after the advertised showtime and depends on successful wallet processing.

## Install in Muse

Open the [v5 revision 3 release](https://github.com/nullapps/reelcognito-skills/releases/tag/muse-v5-r3) and paste its **Install with Muse** prompt into a private Muse conversation. Muse asks for approval, retrieves five commit-pinned files, checks their SHA-256 fingerprints and verifies the installed copy. A supported persistent skill is saved under the name `reelcognito-mystery-movie-nights`. If persistence is unavailable, Muse can load the verified instructions for this conversation. Installation finishes when Muse reports what it verified. You can stop there without an account or token. [Packaged skill](skills/muse/reelcognito-mystery-movie-nights/SKILL.md)

For a manual conversation-only alternative, copy the text between the two COPY headings in the [combined instructions](skills/muse/reelcognito-mystery-movie-nights/reelcognito-agent-setup-combined-v5-r3.md) from the release. Paste it with this request: “Keep these instructions for this conversation. Wait until I ask to start onboarding before following them. On that separate request, run the interview and the anonymous live preflight under v5 rules, then stop before selecting a showing, paying, or registering a ticket.” The [official setup page](https://reelcognito.com/agents/) also offers the current reviewed text.

## First use and booking

1. When ready, send a **new message**: “Start ReelCognito onboarding.” Answer the interview and confirm your preferences. Muse checks current compatibility using an anonymous request to ReelCognito. Muse reports the preflight result. You can finish the interview and confirm your preferences even if the feed is unavailable, expired or invalid. The reviewed compatibility checks still govern showing selection and payment.
2. Register, verify your email and sign in. Check that Muse offers a supported secure credential connection, then open Agent Connections, name the agent and generate a token. Immediately copy the one-time value into that secure connection. If it is unavailable, pause token provisioning. [Customer dashboard](https://app.reelcognito.com/) · [Agent Connections](https://app.reelcognito.com/settings/tokens)
3. Onboarding ends before a purchase. When you later request a movie night, Muse rechecks the live data under the v5 rules before presenting a purchasable showing and seeks your specific purchase approval.

## Costs and availability

Bring Your Own Agent is free. Each account can register up to **20 tickets per UTC calendar month**, shared across its agent tokens, subject to service availability. You pay the movie ticket price, merchant booking fees and any applicable third-party agent or other disclosed charges.

The service is intended for people in the United States. You must be at least 18, or the age of majority where you live if higher. Merchant access depends on the booking site, theater and access method. The matrix lists individual tests, including AMC bookings through Fandango and direct AMC bookings using an enabled Muse Chrome Extension. Consult it before choosing a route. [Compatibility matrix](https://reelcognito.com/compatibility-matrix/) · [Terms of Service](https://reelcognito.com/terms-of-service/)

## Keep the surprise private

Keep ticket links private. Anyone with a bearer admission link may be able to use it. Merchant receipts, notifications and theater signage can reveal the film independently of ReelCognito. Keep passwords, card details and agent tokens out of conversations, saved instructions, shared files and support reports. For a lost or exposed token, revoke it in Agent Connections and generate a replacement. [Security](SECURITY.md) · [Privacy policy](https://reelcognito.com/privacy-policy/)

The website publishes current agent instructions. This repository distributes reviewed versions. The YAML bundled with a release is a historical snapshot. Muse checks ReelCognito's live HTTPS feed under the rules of the installed version. [Release history and publication process](CHANGELOG.md) · [Official website](https://reelcognito.com/) · [Support Center](https://reelcognito.zohodesk.com/)
