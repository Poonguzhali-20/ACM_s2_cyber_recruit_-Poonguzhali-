Challenge description:

This challenge is kinda "visual detective game". Here the given image file is totally empty of secret data, so I can’t rely on any technical extraction of flag. I am only given a photo of a real room made of human bones—with things like bone chandeliers and skull walls—and a riddle about death being helpful to the living. Since the file itself won't tell us anything, I have to use the physical clues in the picture to figure out exactly what this is and what city it’s hiding in.

My approach to find the flag:

Since all the technical "hacker" tools came up empty, I realized the answer wasn't hidden in the file. Since the file had no metadata, the fastest way was to upload the photo to Google Lens or Google Images. I looked for the most distinct part of the picture—the bone coat of arms in the center—to see where it was located. I typed the phrase "This is the place where death delights in helping the living" into Google. Google immediately linked it to famous bone chapels and ossuaries.The search results for both the image and the quote pointed to the same spot: the Sedlec Ossuary (the "Bone Church").Once I had the name of the building, I did a quick search for "Sedlec Ossuary location" to get the city name, which is Kutná Hora.

Tools and commands used:

ExifTool: I used this to check for "hidden" text like GPS coordinates or timestamps. It told me the image was "clean," which was the hint to stop looking at the code and start looking at the picture.

Strings: I ran this to see if the flag was written in plain text inside the file's computer code.

Steghide & Stegsnow: I used these to check if a password was protecting a secret file hidden inside the image or the text file.

Google Lens / Image Search: This was my most important "tool." By searching for the bone shield, I identified the building.

Google Search: I used this to search for the quote, which confirmed the specific chapel. Also flag format which is given in challenge description helped me to get the right flag.

Flag:
 flag{sedlec_ossuary_kutna_hora} 
