#Perceibing Permissions

### Flags and Writeups

1) pwn.college{0dhwBx7P4sDKs3IeypMfFo6taWj.dFTM2QDL0kTM2czW}
    - `chown` is used to change the owner of the files, 
    - `chown hacker /flag` changes the owner of file to hacker so we can as 'hacker' user can read it.  
    - ` cat /flag` gives us the flag. 

2) pwn.college{0Xn6jJ5v1z5fazHn--iPjXMio8I.dFzNyUDL0kTM2czW}
    - `chgrp` is used to change the group ownership of files
    - `chgrp hacker /flag` 
    - `cat /flag` will give us the flag. 

3) pwn.college{cfM0iQRijz8eBVWkO7QwbAwy_64.dJzNyUDL0kTM2czW}
    - use `id` to find out your group name `<grp3185>` in this case.
    - `chgrp grp3185 /flag`
    - `cat /flag` will give us the flag. 

![Screenshot 2024-10-22 183700](https://github.com/user-attachments/assets/b4f466ea-4fb6-4964-ad95-af175717d042)

4) pwn.college{QFpalUDhZMKxTP3r1DMBz-2sTc1.dNzNyUDL0kTM2czW}
    - `chmod` to change file perms. 
    - `chmod a+r /flag`gives read perm to all user, groups,and others
    - `cat /flag` will give you the flag. 

5) pwn.college{UUePWVOrAGo34acRoYXe52Xq4Xk.dJTM2QDL0kTM2czW}
    - `chmod +x /challenge/run` to give it execute perms
    - `/challenge/run` will give the flag.

6) pwn.college{45Sx2oD8XoPlNULsCrBYZ5RGaVm.dBTM2QDL0kTM2czW}
   - use `chmod` to alter the current permissions of `/challenge/pwn` into the needed permissions, 8 times
   - at last use `chmod` againto make `/flag` file readable by typing `chmod u=r,g=r,o=r /flag`
   - `cat /flag` will give the flag
![Screenshot 2024-10-22 192352](https://github.com/user-attachments/assets/f2bf02e8-c068-4332-8b22-05f2dad0d94a)

7)pwn.college{w_JDigIFMEK2fF6GuAbig3zQWsc.dNTM5QDL0kTM2czW}
    - Go through Various rounds advance chmodding for a file
    - `chmod +r /flag` change the perm of the flag. 
    - `cat /flag` to give us the flag.

![Screenshot 2024-10-23 200620](https://github.com/user-attachments/assets/d64b6c5d-f4ff-49c5-aef3-bb2690adb977)

8) pwn.college{g6FhwfeYemVfQ1Abo8VSExZr-LJ.dNTM2QDL0kTM2czW}
    - Set SUID bit for /challenge/getroot with:
    - `chmod +s /challenge/getroot`
    - run program which spawns a root shell, `cat /flag`
