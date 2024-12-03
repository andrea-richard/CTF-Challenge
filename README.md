This is my CTF Challenge for Cybersecurity Club at Cornell University.

ACCESS THE CHALLENGE HERE: [https://andrea-richard.github.io/CTF-Challenge/](url)

CHALLENGE OVERVIEW:
I have created a website in HTML containing an element with the flag encrypted within it. There are no hints provided and the user is allowed to access any portion of the website and the HTML source code 
to solve the CTF. I would rank it as a low-moderate difficulty for a beginner and low difficulty for a intermediate to advanced player. There are two main steps in solving the challenge: first is identifying
the element with the flag and the second is decrypting the flag.

EXPLANATION OF STENOGRAPHY:
While I kept my challenge overview general so the answer wouldn't be given away, this challenge is an example of steganography. I encrypted my flag in the Snoopy icon at my website header via another 
GitHub page ([https://stylesuxx.github.io/steganography/](url)). One application of steganography is hiding text within an image without altering its outward appearance, as I have done here. But there are 
numerous applications of steganography in the real world. One way to think of it is as a method to hide information in plain sight without raising any immediate alarms. This is where steganography
differs from crypotgraphy, which "scrambles" a code in such a way that it cannot be understood without knowing how it was encrypted in the first place. Encrypted codes raise immediate alarms at first glance
just from how random they look, while steganographed images look the same with and without the text encoded within it.

My project uses both steganography and cryptography to encode the flag. The flag is encoded in base64 and then encoded into my image. 

STEP-BY-STEP SOLUTION:
1. Right-click and select "Inspect" for the source HTML code.
2. Open the code body for <header>. (Notice the img src name is "snoopy encoded.png").
3. Download the image. (Right-click the image and "Save As..." on the webpage or hover over its line in the code and press on the source to download it from there).
<img width="415" alt="image" src="https://github.com/user-attachments/assets/3f7bb2ca-1d19-4b54-a91f-8d04222503a8">
<img width="485" alt="image" src="https://github.com/user-attachments/assets/a262ea90-81ff-4a4d-a6e4-cb98fe0036e8">
<br>
5. Enter the image into any online decoder.
   <br>
6. The text result is in base64, enter the text into any online decoder.
   <br>
7. The flag is: flag{they'reeatingthedogs}
