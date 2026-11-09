# Hopcress 1.0 TEST
Native Android Hamle endpoint-placement puzzle. Android 8+ (min26), target35. Package com.gg007.hopcress. Twelve original unique boards on a compact 4x4 grid.

## Rules
Hamle endpoint puzzle on a 4x4 grid. Choose one of five A-E buttons, then tap a destination exactly the printed number of cell steps from its original gold badge, in one straight cardinal direction. Every stone must move; no staying, turns or wrapping. Paths may cross, overlap and pass through other origins or endpoints: this is simultaneous placement, not obstacle sliding. All final stones need distinct cells and cannot share edges; diagonal contact is allowed. All cells without a final stone must connect through edges. Old origin cells become empty unless another stone ends there. Tap the selected endpoint again to clear it; choose another endpoint to replace it. Undo/reset, next and level selection; saved palette and optional trail guides. No timer or score.

## Download and status
https://mega.co.nz/#!gE11RCSQ!hkxC1nN7UnsNLuROtZPpQoNz8n15IDOO3BriQMazXHo
APK SHA256 1e769cdc8864a5d3bc67f1b30badc107e65c1be8b49e556e5f93c3ffeafc2d5b; 16878 bytes. Original signing certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. Anonymous downloaded bytes match. No requested permissions. Original icon unchanged.

## Checks
Independent row/column endpoint calculation and Set/queue connectivity versus production direction arithmetic and bit flood agree on all 12,288 complete direction assignments and 65,536 full-board dark/white shape masks. Twelve distinct original start/distance boards each admit exactly one assignment; their final positions comprise ten distinct endpoint sets. Every stone has at least two in-bounds choices before endpoint constraints. Tests cover selection, replace/clear, bounds, undo, reset, solved lock, malformed data, allowed diagonal contact, forbidden side contact and isolated white corner cases. Portable generator seed 581009 reproduces the twelve boards in 264 attempts. A six-stone candidate produced no boards because connected-white 4x4 shapes allow at most five separated stones; generation changed to five before production and oracle tests. Actual drawing-adapter taps solve all twelve, with undo/replay, next, levels, menu, privacy and saved palette/trail guides checked. Six drawing previews inspected, not phone screenshots. Phone runtime/performance/external-browser QA and full Git source commit remain incomplete. Signed TEST, not final or Play published.

## Functional difference
Reviewed all 189 prior studio descriptions and byte-current 803 web registry records using functional terms. No Hamle/exact-distance endpoint-separation match found in reviewed corpus; corpus is partial. Homebriar sends fixed-distance circles into one-per-country endpoints with disjoint tracks that cannot pass starts. Hopcress has no countries or route blocking: crossing moves instead produce isolated final stones and one connected empty clearing. Railcress counts available sliding space of parked cars, not exact-distance relocation. Kakuru candidate was dropped because exact rule sources were not established, not silently replaced with Kakuro. Known Hamle adaptation with original boards, code and visuals, no copied layouts/code/art and no origin claim. Competition archive, solver documentation and author rules agree on the final position constraints. One author mentions exiting and re-entering the grid while remaining straight; no wrapping permission is inferred from that odd wording. This edition keeps endpoints in the grid and allows crossing paths. Hamle Sudoku removes ordinary Hamle final-adjacency and white-connectivity rules and is not used as the rule set.
Rules https://www.janko.at/Raetsel/OAPC/060.a.htm ; independent rules https://www.cross-plus-a.com/html/cros7haml.htm .

## Build
JDK17, Android SDK35/build-tools35.0.0. python generate-levels.py reproduces levels.json. javac -d /tmp/blue-test src/com/gg007/hopcress/Board.java BoardTest.java then java -cp /tmp/blue-test com.gg007.hopcress.BoardTest. bash build.sh makes an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to your own private signing material. No signing secret is included.

## Privacy and branding
Hopcress runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Palette, trail guides and solved-board marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 original icon, menu studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and publishing
Complete source/APK, exact cumulative 190-card studio and published catalog/studio sources and updater privately preserved at https://files.instinct.com/qx0cl3y7t78s-hopcress-source-archive . Repository https://github.com/iLanis-agent/hopcress holds README only; full Git source commit pending. Existing Jekyll static includes retained without changes; no Pages settings changes or client loader. Both site publications verified separately.
