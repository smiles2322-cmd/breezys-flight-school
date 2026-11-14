# Breezy's Flight School (v1)

A gentle 3D flying game for kids (about ages 4 to 10) by **Smiles 2322**.
Breezy, a little pegasus foal, learns to fly with help from **Grandma Cloudmane**.
Breezy and Grandma Cloudmane are original characters made for this game.

## Play it
It's a web app (PWA). Put this folder on any web host (for example GitHub Pages under `/breezys-flight-school/`) and open `index.html`.
All paths are relative, so it works in a sub-folder. After the first visit it works offline.
On a phone: open the link, then **Share > Add to Home Screen** (iPhone) or **Install app** (Android Chrome).
Opening `index.html` straight from a file won't work, because browsers block 3D modules from `file://`. It needs a web address, even a local one (`python3 -m http.server`).

## What's inside
- **5 lessons:** First Flaps, Glide & Turn, Up & Down, Cloud Rings, Soft Landing.
- **Free Flight:** Cloud Island with floating islands, 3 rainbows to fly through, and a waterfall. There are 41 stars and 12 feathers to find.
- **Simple flight feel:** flapping gives lift, Breezy glides when you let go, and she banks into turns. Climbing slows you down and diving speeds you up. If she gets too slow, she does a soft float instead of falling, and breezes push her sideways.
- **No fail states:** water gives a happy splash and bounce, and grass is a landing (flap to take off again). If you miss a ring, just circle around.
- **3 help levels:** Little Flyer (steers toward the goal and flaps when low), Junior Flyer, and Sky Champ.

## Controls
- **Phone:** thumb stick on the left, big FLAP button on the right. **Tilt steering** is optional (turn it on in Settings; iPhone asks for permission).
- **Keyboard:** Arrow keys or WASD to steer and climb or dive, **Space** to flap, **H** to hear where the next goal is, **Esc** to pause.
- **Speaker button:** Grandma says where the next goal is, for example "Ring ahead, a little left and up."

## Blind & Low Vision mode
This mode is off by default, so sighted players never get it unless they want it. The game offers it once on first launch, and it's always in Settings.
- **Sound beacon:** each goal plays its own beeping tone in 3D sound (HRTF). The tone moves left and right with the goal, gets higher when the goal is above you and lower when it's below, and beeps faster and louder as you get closer, like a parking sensor. When the goal is behind you, the beeps sound muffled. Headphones help a lot.
- **Low warning:** a rising whoosh plays when Breezy is close to the ground or water, along with a vibration pattern and Grandma saying "Low! Flap!"
- **Voice:** Grandma reads every lesson step and gives directions every few seconds.
- **Vibration:** a tick when you pass a ring or get a star, a pattern when you're near the ground, and a happy buzz when you finish.
- **Extra flying help:** Breezy steers and climbs toward the goal on her own, rings are much bigger, breezes are tiny, and there's no time pressure. You can finish every lesson by listening and tapping FLAP (or pressing Space).
- Screen reader labels, live announcements, full keyboard play, Reduce Motion, High Contrast, and Large Text.

**iPhone note:** Safari on iPhone and iPad doesn't support web vibration, so the sounds carry those cues there instead. Android Chrome vibrates.
**Screen reader note:** if you use VoiceOver or TalkBack and hear things twice, turn off "Grandma's voice" in Settings. The screen reader still gets every update.

## Sound
All music and sound effects are made live in the browser with Web Audio, including wing flaps, wind, chimes, the waterfall, and a gentle music loop. There's no recorded or copyrighted audio. Grandma's voice uses the device's built-in text-to-speech, so it sounds a little different on each device.

## Privacy
There are no ads, accounts, purchases, tracking, or network calls. Progress and settings are saved only on the device (localStorage).

## Files
`index.html`, `style.css`, `js/game.js` (game plus bundled Three.js), `sw.js` (offline cache), `manifest.webmanifest`, `icons/`, and `THIRD_PARTY_LICENSES.txt`.
