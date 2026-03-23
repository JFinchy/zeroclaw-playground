# Surviving Business Blueprints from Ideation Harvester

## Part 1

**Blueprint 1: QuestLog**
*   **JTBD:** Collect client files/assets on time without sending 15 follow-up emails.
*   **Mechanic:** Gamification
*   **Solution:** Client onboarding turned into a progress bar game. The project kickoff is 'locked' until all assets are uploaded.
*   **Solo Dev Viability:** Simple file upload bucket (S3) + gamified UI.
*   **Pricing:** $29/mo for freelancers.

**Blueprint 2: BurnRate**
*   **JTBD:** Track actual hourly rate on fixed-price projects to avoid losing money.
*   **Mechanic:** Visual Degradation
*   **Solution:** A desktop widget timer for fixed-price gigs. You enter the fixed price, and as time ticks, the widget visually degrades/turns red as your effective hourly rate drops below your minimum threshold.
*   **Solo Dev Viability:** Simple Tauri/Electron app. No complex backend needed.
*   **Pricing:** $49 one-time purchase or $5/mo.

**Blueprint 3: RansomDelivery**
*   **JTBD:** Get paid immediately upon project delivery without chasing invoices.
*   **Mechanic:** Headless / Escrow
*   **Solution:** An API-first file delivery system. You upload the final assets, and it generates a link. The client views a watermarked/low-res version. To download the final high-res version, they enter their credit card. The payment clears via Stripe, and the file instantly unlocks.
*   **Solo Dev Viability:** Extremely viable. S3 presigned URLs + Stripe API.
*   **Pricing:** 1% per transaction + $9/mo.

**Blueprint 4: ScopeSwipe**
*   **JTBD:** Monetize out-of-scope requests without awkward conversations or confrontation.
*   **Mechanic:** Swipe-to-sort (Tinder UI)
*   **Solution:** When a client asks for a "quick change" that's out of scope, you log it with a price. At the end of the week, the client gets a mobile link with a deck of cards showing the ideas and extra costs. They swipe right to approve the charge, left to discard the idea.
*   **Solo Dev Viability:** Simple mobile-first web app + Stripe integration.
*   **Pricing:** $19/mo.

**Blueprint 5: SkinInTheGame**
*   **JTBD:** Clients ghosting discovery calls, wasting unbilled time.
*   **Mechanic:** Escrow / Holds
*   **Solution:** A scheduling link that requires a $50 credit card authorization hold to book. If they show up, it's released. If they no-show, the freelancer captures the fee.
*   **Solo Dev Viability:** Next.js + Stripe Auth & Capture + Calendar API.
*   **Pricing:** 10% cut of captured no-show fees, or $12/mo.

## Part 2

**Blueprint 6: BurnerText**
*   **JTBD:** Small business owners getting texted by clients at 11 PM on their personal phones.
*   **Mechanic:** Ephemeral
*   **Solution:** An SMS proxy bot that generates a temporary 48-hour phone number bridging the customer and the owner's personal cell. The owner texts normally from their native SMS app. After 48 hours, the bridge burns. No VoIP app to download.
*   **Solo Dev Viability:** Twilio proxy API + simple DB. No frontend needed.
*   **Pricing:** $15/mo.

**Blueprint 7: FlowState Update**
*   **JTBD:** Freelancers need to keep anxious clients updated on progress without breaking deep work or writing lengthy status emails.
*   **Mechanic:** Asynchronous Video / Headless
*   **Solution:** A headless CLI tool for developers/designers. You type `update "finished the database schema"` in your terminal. It instantly takes a screenshot of your active window, records 10 seconds of your microphone, and texts/emails an unbranded, professional link to the client. 
*   **Solo Dev Viability:** Extremely high. Simple CLI wrapper + S3 for storage + Twilio/SendGrid API. No complex web dashboard needed.
*   **Pricing:** $9/mo.

**Blueprint 8: ReceiptDrop**
*   **JTBD:** Small business owners have a truck full of crumpled receipts and hate sitting down for hours of data entry.
*   **Mechanic:** Headless / API-first
*   **Solution:** A dedicated WhatsApp or SMS bot. The owner just snaps a picture of a receipt and texts it to the bot. The bot uses AI Vision to extract the vendor, amount, date, and tax category, and pushes it directly to a Google Sheet or Xero/Quickbooks via API. No mobile app to download or log into.
*   **Solo Dev Viability:** High. WhatsApp/Twilio API + OpenAI Vision API + Zapier/Make webhooks. Completely stateless.
*   **Pricing:** $19/mo for up to 100 receipts.

**Blueprint 9: RoastMyDraft**
*   **JTBD:** Freelancers need precise, actionable feedback on visual assets without the vague 'make it pop' email ping-pong.
*   **Mechanic:** Ephemeral / Asynchronous Audio
*   **Solution:** You upload a design or screenshot. It generates a 24-hour expiring link. The client opens it on their phone, taps exactly where they want a change, records a 10-second voice note, and the link burns. The structured feedback drops straight into your Trello/Notion.
*   **Solo Dev Viability:** Canvas API for tapping, Web Audio API for voice, S3 for storage. Very doable.
*   **Pricing:** $15/mo for unlimited active links.

**Blueprint 10: SaaSFreezer**
*   **JTBD:** Small businesses want to cancel expensive $100/mo SaaS subscriptions but are terrified of losing their historical data.
*   **Mechanic:** Offline-first / One-time purchase
*   **Solution:** A tool that connects to popular SaaS APIs (like Mailchimp, old CRMs, Zendesk) and extracts all your raw data into a searchable, offline static HTML/SQLite file. You keep the file forever on your desktop, and confidently cancel the expensive subscription.
*   **Solo Dev Viability:** High. Just build one API extractor at a time. No ongoing server costs to maintain user data.
*   **Pricing:** $49 one-time per export.

**Blueprint 11: Handshake SMS**
*   **JTBD:** Sending legally binding micro-contracts/quotes in under 30 seconds without formatting a PDF proposal.
*   **Mechanic:** Headless / SMS-first
*   **Solution:** You text a bot: 'Build a landing page for $1500 for [client phone number]'. The bot texts the client: 'Jake proposed building a landing page for $1500. Reply YES to legally accept and agree to the standard terms at [shortlink].' A 'YES' reply logs a binding timestamp and triggers a Stripe invoice.
*   **Solo Dev Viability:** Twilio SMS + simple DB + Stripe API.
*   **Pricing:** $10/mo or 1% of the contract.
