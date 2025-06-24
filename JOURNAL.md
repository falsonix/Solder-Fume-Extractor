---
title: Fume Extractor
author: falsonix (AKA fals)
description: Semi 3D printed solder fume extractor
created_at (MM/DD/YYYY): 06/24/2025
---

**Total time spent on this project as of the latest entry: 0.45 hours**

# June 24th, 2025 [Introduction & Research] - 0.45 hours {IN PROGRESS}
This is my second project for Highway, and as such it will be a lot smaller than my previous one. *yes, i REALLY want to go to Undercity.* Also, the format for both the `JOURNAL.md` file as well as the folder containing the CAD files will be similar or exactly the same.

For this project, my goal is to design a very simple solder fume extractor that meets the following criteria:
- Easy to build for beginners
- Affordable ($15-20 USD cost goal)
- Works well
- Fan speed adjustable by a potentiometer/dial/encoder (PWM)

I began with researching types of fans and which would be a good one for this application. A fan that runs off of DC at a lower voltage would be preferred for this project, as I'd like to be able to power the unit via USB-C in the end. A couple fan types were of note, that fit my above criteria.

---

**Standard 120/140mm PC Case Fan**

Pros:
- Inexpensive (approx. $5-10 USD)
- Large(ish) size
- PWM-driven
- Widely available
- 12V DC

Cons:
- Many different styles, mounting holes might not line up on each
- Connector/wiring differs slightly between each model

<img src="https://github.com/user-attachments/assets/91de67c9-8e34-4a43-a4c2-3b90fdcc9ea5" width=250>

---

**9025 Fan**

Pros:
- Inexpensive (approx. $4-5 USD)
- Smaller size, but still large enough
- Generic part available from sites like AliExpress
- 12/24V DC

Cons:
- Not PWM-driven

<img src="https://github.com/user-attachments/assets/5f93c853-6fd8-4142-afe4-8da1acdb852f" width=250>

---

In the end, I chose to go with the PC case fan, in a 140mm size. This was mostly due to the fact that these are everywhere online, and don't cost that much. I now needed a way of actually controlling the fan's speed, and a microcontroller would be the simplest way of doing so. (one might be able to get away with using a 555 timer to generate the PWM signal, but I like to code and keep the physical electronics relatively simple).
