
challenge description:

The challenge was to identify a mysterious ancient structure using only a few clues and one quote.
    The Clues: The structure has thousands of repeating stone steps, no visible water.
    The Quote: "Built to defeat heat, not enemies." This tells us the building wasn't a fort for war, to stay cool in a hot climate.

My approach to find the flag:
    Since it is a forensic challenge ,I took the given image.jpeg file and uploaded it to Google Lens.
Google identified the structure as the Chand Baori step well located in rajastan.I then checked the other clues to make sure I was right ,"Built to defeat heat": it absolutely meant the stepwell here.

Tools and Commands used:
    I mainly used google to find the flag , also , flag{structure_name|state_name} , flag format which is given in the challenge description helped me to get a correct flag. I also used strings , exiftool to find if there were any hidden text found in the image's binary code.
    
Flag:
 flag{chand_baori|Rajasthan}
