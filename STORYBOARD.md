# Storyboard: "Samsung Pay on GenMotion"

This keeps the reference's structure, pacing, framing and motion beat for beat. The brand changes: **Samsung Pay** is the badge and **GenMotion** is the checkout platform.
All copy is new, and all artwork is original geometry drawn in code (tiles, phone UI, product). Merchant names are fictional.

| # | Reference beat | Our copy |
|---|---|---|
| 1 | 3-step kinetic line | "The" → "The tap" → "your customers" → "already know by heart" (accent on "know by heart") |
| 2 | ring headline | "Now live in your checkout" (accent on "your checkout") |
| 3 | column caption | "wherever India shops" |
| 4 | introducing | "Introducing" → Samsung Pay badge + "on GenMotion" |
| 5 | white type + phone | "Built for every storefront" → "and every screen". Store "LUMA", a ceramic lamp at ₹4,800. Side label "One tap" |
| 6 | dark + phone | "Checkout / in one tap" → "Verified / on your device" (a fingerprint glyph, not Face ID) |
| 7 | confirm → success | "Confirming payment" → "Payment successful", with a green receipt |
| 8 | lockup | Samsung Pay badge · "now on" · GenMotion Checkout |
| 9 | letter words | "fast" · "safe" · "simple" |
| 10 | CTA + walls | "Bring one-tap pay / to your checkout today" → GenMotion \| Samsung Pay → fictional merchant wall |

The detailed frame-by-frame notes below come from the reference and still set the timings.

Source: 35.07s, 1051 frames @ 30fps, 16:9. Timings below come from scene-cut detection plus 5fps contact sheets.
Frame numbers are global (30fps). Each row is one Three.js scene file.

Palette: dark backgrounds are near-black (#050507) with a soft grey-blue diagonal light shaft. Accent is periwinkle/violet (#8b8cf5 → #6d6ff0).
Light acts use white (#ffffff) with navy→royal-blue type (#0b1a4a → #1f3fd1). Success green is #12a150.
Type: Inter / SF-style grotesk, weight 500, tight tracking.

| # | File | Global frames | Len | Look |
|---|------|---------------|-----|------|
| 1 | 01-hook-type.ts | 0–112 | 112 | Dark + light shaft, kinetic type |
| 2 | 02-icon-orbit.ts | 112–217 | 105 | Black, 3D icon tiles orbit a headline |
| 3 | 03-icon-column.ts | 217–250 | 33 | Black, macro icon tiles scroll past camera |
| 4 | 04-introducing.ts | 250–342 | 92 | Dark gradient, badge reveal, zoom-through |
| 5 | 05-phone-flow.ts | 342–522 | 180 | White, type + phone shopping flow |
| 6 | 06-secure-sheet.ts | 522–683 | 161 | Dark + violet floor glow, phone right, type left |
| 7 | 07-confirm-success.ts | 683–789 | 106 | Violet → green glow, coin → check → receipt |
| 8 | 08-now-on.ts | 789–828 | 39 | Dark gradient, badge lockup |
| 9 | 09-easy-secure-private.ts | 828–915 | 87 | White, letter-by-letter kinetic words |
| 10 | 10-cta-lockups.ts | 915–1051 | 136 | White: CTA line → partner lockup → merchant wall → black |

---

## 1. Hook type (0–112)
- **Background:** black, with a wide soft grey light shaft running top-left to bottom-right that drifts slowly.
- **f0–10:** "The" sits large (~150px) at centre-left.
- **f10–14:** it shrinks to ~100px while "experience" slides in from the right with a motion blur. They settle as "The experience", centred.
- **f40:** hard swap to "your customers" (same size, centred), with a slight scale push.
- **f64:** swap to "have been waiting for". "have" is white; "been waiting for" is the violet accent, and the colour sweeps left to right.
- **f108–112:** everything cuts to pure black. That black frame is the handoff.

## 2. Icon orbit, "Now set to transform" (112–217)
- **f112–118:** about 16 3D payment tiles (shield, check badge, cart, rupee coin, T-shirt, trend chart, paper plane, globe, shopping bag, stacked coins, up-arrow, progress bar) fly in from behind the camera, blurred and oversized.
- **f118–135:** they decelerate into a tilted elliptical ring around the centre.
- **f120:** "Now" appears (small, ~40px). "set" follows at f126 and "to transform" at f132. "transform" is violet.
- **f135–217:** the ring rotates slowly (about 40° in total). The tiles bob a little.
- **Handoff:** the camera pushes into the ring.

## 3. Icon column, "the way India pays" (217–250)
- A macro close-up: a vertical column of large rounded icon tiles (white and black) scrolls upward past the camera at speed, with a gap in the middle.
- **f221:** "the way India pays" types in word by word in the gap. "India" rises into place.
- **f250:** cut.

## 4. Introducing (250–342)
- **Background:** dark with a soft blue-grey radial glow.
- **f252:** "Introducing" in small type (~30px), centred. It fades in and holds.
- **f292:** it is replaced by the white rounded **Pay badge** (~260×160px), which scales in 0.96→1.
- **f298–305:** "on [partner]" fades in beneath it.
- **f330–342:** the badge rushes toward the camera. The frame fills with a white, blurred, oversized "Pa". **Handoff:** white.

## 5. Phone flow (342–522), white background
- **f342:** "A world of" is set left of centre.
- **f350:** "possibilities" slides in from the right in navy→blue.
- **f372:** swap to "for your business".
- **f390:** the words part and a phone rises from below through the gap to the centre (the product page: a perfume bottle and a product title).
- **f415–435:** the camera tilts down the phone to the "ADD TO BAG" bar, and a round touch indicator taps it.
- **f450:** the checkout list shows (Cash on delivery, PayLater, "Continue"), which gets a tap.
- **f462–480:** the Payment Options sheet scrolls up. It holds the recommended black Pay button, then Cards, Netbanking and EMI.
- **f480:** the phone slides right and "One Button" slides in on the left (blue).
- **f510:** a tap on the Pay button.
- **f515–522:** the Pay sheet slides up and the scene cross-cuts to dark.

## 6. Secure sheet (522–683)
- **Background:** black with a violet glow rising from the bottom (the floor).
- **Layout:** the phone is on the right, slightly angled, with the Pay sheet open (₹4,800, card image). The type is on the left.
- **f540:** "Frictionless / checkout" (2 lines) wipes in letter by letter.
- **f585:** swap to "Designed / to be secure". The camera pushes in and the phone grows and moves up.
- **f600–640:** a side-button double-click pulse (a circle at the phone's right edge).
- **f645:** a Face ID glyph animates in the phone's top island: a spinning ring, then a smiley check.
- **f675–683:** blur/zoom exit.

## 7. Confirm → success (683–789)
- **f683:** the phone is centred and cropped at the top. It reads "Confirming Payment" with a spinning gold coin.
- **f705–735:** a blue swoosh trail sweeps into the coin.
- **f742:** "Payment successful" and the coin turns into a green check.
- **f750:** the whole screen floods green. A receipt card shows with a check-burst icon. The glow behind turns green.
- **f780–789:** the phone slides up out of frame, leaving the green glow.

## 8. Now on (789–828)
- **Background:** dark gradient.
- The Pay badge sits at centre-top, with "now on" below it and then "[partner] Checkout". Everything is static, except a slow drift and a gradient shift.

## 9. Easy · secure · private (828–915)
- **f828–834:** a white wipe comes up from the bottom (the violet haze clears).
- **f834:** "easy" is built letter by letter. Each letter rises from below and fades from grey to navy→blue.
- **f852:** "secure" is built the same way, on a 3-frame stagger.
- **f870:** "private" is built the same way and holds until f915.
- The words are huge, about 170px.

## 10. CTA + lockups (915–1051)
- **f915–925:** "Bring the experience / to your customers today!" is built word by word, with grey words darkening to black.
- **f963:** swap to the partner lockup "[Razorpay] | [Apple Pay]", small and centred.
- **f1000:** swap to a merchant logo wall: 3 on top, 2 below, with thin dividers.
- **f1047–1051:** a cut to black.
