# File Globbing 
## Notes and Flags

1) pwn.college{EKG9VDKoEO-rAIcct14psKV2d1m.dFjM4QDL0kTM2czW}
    - `*` is the wild character and can be used to replace any file which matches the pattern.
    - for the challenge `/ch*` changes the directory to /challenge
    - wherein you can run `./run` to print the flag.

![Screenshot 2024-10-22 082223](https://github.com/user-attachments/assets/6e85e2d9-e5b9-4287-aa9a-0933806ba1bc)


2) pwn.college{oB7dBwjfcrVo8Hpah57dXwk4Krl.dJjM4QDL0kTM2czW}
    - `?` is another wildcard character but it only replaces upto 1 character 
    - following the same principle, we use `cd /?ha??enge` to change the directory, and then `./run` to print the flag.

![Screenshot 2024-10-22 082442](https://github.com/user-attachments/assets/44beb45c-e98b-4266-b7f5-cd93bc0afbd8)


3) pwn.college{cgVuAi8jrI8kVN0QOXWpvqXzcb5.dNjM4QDL0kTM2czW}
    - `[]` is like a wild-card multiple choice ie the pattern matching will only occur with the characters which are inside the [].
    - following instructions, `cd /challenge/files` 
    - now as per challenge description we use `[]` to pass the arguments to /challenge/run ie `/challenge/run file_[bash]`, this gives us the flag. 

![Screenshot 2024-10-22 082910](https://github.com/user-attachments/assets/0ae09851-4da9-45eb-bc51-7ad1bc71866d)


4) pwn.college{coWGwBqtWoJ82VR5I4NZJKL-lgM.dRjM4QDL0kTM2czW}
    - `[]` can be used to expand on absolute file paths as well. 
    -   `/challenge/run /challenge/files/file_[absh]` gives us the flag. 

![Screenshot 2024-10-22 083520](https://github.com/user-attachments/assets/a5f9f145-43b6-4538-bd03-7f89dded6c2f)

5) pwn.college{AH-PpAb393EJQ51_5kvlwUoNMSW.dVjM4QDL0kTM2czW}

    - This was a tricky one, following description we `cd /challenge/files` and see the files.
    - Interesting thing we notice is that there is only 1 filename with starting with each letter. 
    - so `[cep]*` would expand to the file names we need 
    - running  `/challenge/run [cep]*` gives us the flag. 

![Screenshot 2024-10-22 083714](https://github.com/user-attachments/assets/58ceaea3-3c1a-413e-a84f-3bf454749e60)

6) pwn.college{M4jNbzDs10vwetgmolyATbWGuna.dZjM4QDL0kTM2czW}
    - `[!<patter,letters>]` the "!" or "^"acts as an invert and disincludes the chars in the "[]"
    - Similar to Challenge 5, we notice only 1 filename per letter in the `/challenge/files` directory
    - `/challenge/run [!pwn]*` gives us the flag.

 ![image](https://github.com/user-attachments/assets/66d5ce6b-26d8-45ff-929e-1ee29eb9d7aa)
 
