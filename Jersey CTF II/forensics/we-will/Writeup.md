**Title:** We Will

**Description**: A flag was left behind but it seems to be protected.

*Some thoughts*:

The challenge is named we-will. Hmm, this sounds familiar. Oh yea, the song: We will rock you. "*We will, we will rock you*"
Oh, that is a big hint right there! I think we need to use rockyou.txt!


*Solving the challenge*:

Run the flag.zip file through zip2john and save the output into a file (flaghash.hash in this case):

```zip2john flag.zip > flaghash.hash```

Now, we need to run JohnTheRipper on this .hash file using the rockyou.txt wordlist:

```john flaghash.hash --wordlist=rockyou.txt```

Let john do its majic, and boom! We got our password: `*@@!^^$25Jjersey` Let's unzip the original file and get our flag!

Flag: `jctf{y0u_r0ck3d_17}`
