**Title:** Corrupted File

*Description:* Can you find a way to fix our corrupted .jpg file?


*Solution:*

We see that the JPG image file is corrupted and we need to fix it so that it will display. 
Let's look into the file header. Spinning up a hex editor, we can see that the file is missing the default JPG file header of `FF D8 FF E0`

After addding these 4 bytes to the beginning of the file in a hex editor, we can save the file and simply open it with a regular file viewer.

Flag: ```jctf{OaZdSdMo8F}```
