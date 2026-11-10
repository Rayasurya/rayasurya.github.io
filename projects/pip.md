# Pip: A desk pet that reads a room through its air, with no camera and no microphone.

- When: October to November 2026
- Type: Hardware experiment, built by hand, working on a wall
- Case study: https://rayasurya.com/projects/pip/
- Code on GitHub: https://github.com/Rayasurya/Pip-Air-Pet

**What it is.** An ESP32 board with a CO2 sensor that also measures heat and humidity, a light sensor, a touch pad, a buzzer and a 1.3-inch screen. The face on the screen shows how the room feels, and a bubble shows why. Built 16 to 19 Oct 2026; the whole order, tools included, came to about ₹5,570. Raya built it with AI coding tools and designed and directed every decision.

**Bugs only the real board showed.** One part of the code asked for 21 KB when the board gives a task 8 KB of scratch memory, so the board kept restarting. And sin(180°) came out as −0.00000009 on the board, which turned into "not a number" and froze a drawing. After both fixes it runs at about 13 frames a second. The firmware has 102 tests.

**In a real room.** 18.8 days on a wall, 17,106 readings (one a minute), typical CO2 572 ppm. 164.6 hours are missing from the log: on 12 of 19 nights Pip was off for over 2 hours, because its screen kept Raya awake or the power went.

**What the real data showed.** The forecast, trained on simulated rooms, did not hold in the real room: 20 minutes ahead it missed by 86 ppm on average, against 27 ppm for guessing "no change", and 4 of its 15 warnings were followed by stuffy air (1,000 ppm within 45 minutes). Pip also could not tell a sleeping person from an empty room: asleep, CO2 stayed 112 ppm above outdoor air but steady, and Pip said "someone here" under 1% of the time. In and out come from Raya's own routine, not a log.

**Honesty notes.** The readings, the log and the bugs are real. The forecast test and the parked-car results are simulated: in simulation (2,400 parked cars and vans), after 10 earlier parkings the same sensor found 99.6% of infants in a closed car within 10 minutes (270 cases). No user research was done.

---
More about Raya Surya: https://rayasurya.github.io/llms-full.txt · Contact: raya.work.ux@gmail.com
