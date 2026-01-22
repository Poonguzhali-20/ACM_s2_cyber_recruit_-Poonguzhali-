Challenge description:
  In the challenge description , 4 important things were given.
     *Html
     *Html's birth
     *flag format
     *Html coded txt file.
     
My approach to find the flag:
     I opened the text file and realized it was actually a webpage "blueprint" (HTML). I saw a lot of weird text ending in ==. 
I recognized this "Base64" pattern as a secret code. While there were many small pieces of code, I found one long string in the CSS section labeled "random noise". I decoded that long string. When it turned into another code, I didn't give up—I decoded it again and again until a real name appeared. Once I saw the name of the man who invented the web, I found out that this is the flag.

Tools and commands:
   cat find_right_flag.txt, to read the file content.
   echo "VmpGamQyVkdXWGROU0d4V1lUSm9VVll3V2xaUFVUMDk=" | base64 -d | base64 -d | base64 -d.
    First -d: Decodes the "noise" into the first hidden layer.
    Second -d: Decodes that layer into the second hidden layer.
    Third -d: Finally reveals TIM_BERNERS_LEE
 
Flag:
  flag{TIM_BERNERS_LEE} 
