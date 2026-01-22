In the second challenge , A jpg file and challenge description txt file was given. In the challenge description , we are asked to extract the flag from the given image file. Also in the hint, it is mentioned that analyze binary file in hexadecimal format.

My Approach to find the flag:

So typical binary files are jpg and exe. Since in the description, as a hint , we are already told to use a command. So I know that "strings" is command tool which is used to extract readable texts from binary file. After that , in the linux terminal , I used "strings" command with the given jpg file. Finally I got the flag name in the terminal.

Tools and Command used:

string command in the linux terminal.

Flag: flag{jai_mahismathi}
