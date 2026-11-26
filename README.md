# ReelCognito · Mystery Movie Nights

Let your AI shopping agent choose a movie for you. Pick the theater, time and budget, approve a schedule without seeing the title, and take a mystery ticket to the theater. You can discover the film when it starts on screen.

Muse is the first shopping agent covered by this repository. It interviews you about your tastes, films you have seen, seats, budget and spoiler preferences. After you confirm your rules, Muse can propose a night out and ask for approval of the specific purchase. Your agent books with the merchant. ReelCognito turns the purchased ticket into a mystery pass for Apple Wallet or Google Wallet when issuance succeeds. The pass shows “Mystery Movie” through the previews. Its title update is scheduled for 30 minutes after the advertised showtime and depends on successful wallet processing.

## Set up Muse

1. Open the [ReelCognito v5 release](https://github.com/nullapps/reelcognito-skills/releases/tag/muse-v5). Review the release and follow the **Install with Muse** prompt in its notes. Muse will ask before installing anything.
2. For a conversation-only setup, open the combined Markdown in the release's source files and paste the text between its two COPY headings into a fresh, private Muse conversation. Add this request to the same message: “Run setup and the anonymous compatibility preflight only. Finish before selecting a showing, paying, or registering a ticket.” The two sections belong together. The [official setup page](https://reelcognito.com/agents/) also offers the current reviewed instructions with a copy button.
3. Create an account, verify your email, and sign in. Check that Muse offers a supported secure credential connection before generating a token. When it does, open Agent Connections, name the agent and generate a token. Copy it immediately into Muse's supported secure credential connection. If your Muse session lacks that capability, you can complete the interview and resume account setup when a secure connection is available. [Customer dashboard](https://app.reelcognito.com/) · [Agent Connections](https://app.reelcognito.com/settings/tokens)
4. Answer the interview and confirm your preferences. Muse checks the live compatibility manifest before it presents a showing as purchasable. Setup ends before any booking, payment, or ticket registration.

## Costs and availability

Bring Your Own Agent is free. Each account can register up to **20 tickets per UTC calendar month**, shared across its agent tokens, subject to service availability. You pay the movie ticket price, merchant booking fees and any applicable third-party agent or other disclosed charges.

The service is intended for people in the United States. You must be at least 18, or the age of majority where you live if higher. Merchant access depends on the booking site, theater and access method. The matrix lists individual tests, including AMC bookings through Fandango and direct AMC bookings using an enabled Muse Chrome Extension. Consult it before choosing a route. [Compatibility matrix](https://reelcognito.com/compatibility-matrix/) · [Terms of Service](https://reelcognito.com/terms-of-service/)

## Keep the surprise private

Keep ticket links private. Anyone with a bearer admission link may be able to use it. Merchant receipts, notifications and theater signage can reveal the film independently of ReelCognito. Keep passwords, card details and agent tokens out of conversations, saved instructions, shared files and support reports. For a lost or exposed token, revoke it in Agent Connections and generate a replacement. [Security](SECURITY.md) · [Privacy policy](https://reelcognito.com/privacy-policy/)

The website publishes current agent instructions. This repository distributes reviewed versions. The YAML bundled with a release is a historical snapshot. Muse checks ReelCognito's live HTTPS feed under the rules of the installed version. [Release history and publication process](CHANGELOG.md) · [Official website](https://reelcognito.com/) · [Support Center](https://reelcognito.zohodesk.com/)
