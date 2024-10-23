#Untangling Users

##Becoming root with su

1) pwn.college{kAmdT2LnxZGytkvibccYcGYv1Dp.dVTN0UDL0kTM2czW}
    -`su` is used to spawn a root shell when checked with the root password (obeselete)
    - to get the flag run `su` 
    - use password `hack-the-planet`
    - `cat /flag` to get the flag. 
![Screenshot 2024-10-23 202403](https://github.com/user-attachments/assets/10e77c0c-c02d-4a77-870b-5cc02734b7d0)

2)pwn.college{waFbVQsfe918jQnilOxjyQtt5FQ.dZTN0UDL0kTM2czW}
    - become user zarus with `su zardus` with the given password 'dont-hack-me'
    - `/challenge/run` will give you the fla.g
![Screenshot 2024-10-23 223059](https://github.com/user-attachments/assets/522b78f9-e6b3-4b8f-9fd8-595a4779e313)

3) pwn.college{8Rr_ZmfCB_0vgohlzg1NUtl263S.ddTN0UDL0kTM2czW}
    - we need use JohntheRipper to crack the leaked shadow file given to us. 
    - run `john /challenge/shadow-leak` this process will run for some time cracking the password, 
    - use the <password> with `su zardus`
    - now run `/challenge/run` which will give you the flag. 
![Screenshot 2024-10-23 223658](https://github.com/user-attachments/assets/1f82f829-ee08-4358-9817-10f25be2b43e)

4) pwn.college{Y6g22L0ihLZqO2-nFiUexcdJZDj.dhTN0UDL0kTM2czW}
    - sudo is mordern replacement for su, for security purposes. 
    - `sudo cat /flag` will give the flag. 
