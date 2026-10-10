BRAIN ENDURANCE TRAINING · IPHONE WEB APP V1

This is a touch-friendly, offline-capable web app prototype. It stores data locally in the browser on each device; it does not upload results.

Battery order and target active timing:
PVT pre 3:00; Stroop 3:00; Simon 3:00; Flanker 3:00; 2-back 6:00; PVT post 2:00. Total target duration 20 minutes.

Controls:
PVT: tap response button or Space. Stroop: R/G/B/Y keys or colour buttons. Simon: R/B keys or buttons. Flanker: left/right arrow keys or buttons. 2-back: tap MATCH or press Space when the letter matches the one two trials earlier.

Training programme: 9-week cycle, build/build+/deload repeated three times. Three completed training sessions advance the week. Assessment mode uses fixed stimulus settings and does not advance the schedule.

INSTALL ON IPHONE
The first install should be served over HTTPS for Home Screen installation and offline caching. Recommended simple route:
1. Create a GitHub account and a new repository.
2. Upload index.html, app.js, styles.css, manifest.webmanifest, sw.js, icon-192.png and icon-512.png.
3. In repository Settings > Pages, publish from the main branch/root.
4. Open the published HTTPS URL in Safari on the iPhone.
5. Tap Share > Add to Home Screen. Open once while online, then test airplane mode.

TEST ON WINDOWS
Open index.html in a modern browser for a quick check. Offline service-worker installation requires HTTPS or localhost, not file://.

DATA
Local storage is not automatically shared between iPhone and Windows. Export CSV and download JSON backups regularly. Clearing website/browser data may delete results.

IMPORTANT LIMITATIONS
This is a personal prototype, not a validated research or diagnostic instrument. Reaction time depends on device, display refresh, touch latency, browser and input method. Do not treat iPhone touch RT and Windows keyboard RT as interchangeable without validation. The overall battery timer is fixed at 20 minutes, while task transitions and asynchronous callbacks can introduce small timing differences. Test the timing and scoring on the actual iPhone before using results for a formal experiment. Task variants are simplified, not exact replicas of proprietary tests.


UPDATED BUILD SETTINGS (v7)
- Pre-PVT: 3:00
- Stroop: 3:00 (existing setting retained)
- Simon: 3:00 (existing setting retained)
- Flanker: 3:00 (existing setting retained)
- 2-back: 5:00; each letter is visible for 500 ms followed by a fixation marker for the remainder of a 3,000 ms trial cycle. The response window remains open for the full cycle, and trials advance automatically on the fixed timing.
- Post-PVT: 3:00
- Results compare pre/post mean and median reaction time, percentage change, lapses and false starts.
