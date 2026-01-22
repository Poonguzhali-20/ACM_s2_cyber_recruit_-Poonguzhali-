Challenge description:
  I was given a recording of a hack (a .pcap file) and the website’s internal code (HTML and Python). My goal was to find the stolen login info, log into the site myself, and find the secret "Flag."
  
My approach to find the flag:
 I opened the recording in a tool called Wireshark. I didn't want to see all the background noise, so I used a "Filter" to only show when someone sent data to the login page. In the Filter I entered : http.request.method == "POST". It is used to find sensitive data being sent unencrypted. What I found: I right-clicked the login message and chose Follow > HTTP Stream. This showed me the Username and Password. Then I ran the given python in terminal and then logged into this http://127.0.0.1:8080 using the username = 'isitadmin' and password = 'iamtheadmin' which revealed the flag.
 
Tools and Commands used:
 wireshark
 python interpreter
 web-browser.
 
Flag:
 FLAG{analyzing_is_imp} 
