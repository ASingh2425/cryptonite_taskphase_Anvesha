# Chaining Commands

### Flags and writeups

1) pwn.college{YxXM5s22Slc363wSHyN3Mm-4NO2.dVTN4QDL0kTM2czW}
    - ; is used to write multiple commands in the same line
    -`/challenge/pwn; /challenge/college` prints the flag. 

2)pwn.college{YhdieRucllPEPzdCQOhNHce6S6V.dFzN4QDL0kTM2czW}
    -first create a shell script using the following commands
   `touch x.sh`
   `chmod +x x.sh`
   `nano x.sh`
   using this command will opens the `x.sh` shell
   in the shell type `/challenge/pwn` in first line and `/challenge/college` in next line
   then exit the shell by clicking `ctrl+X` save the modification made in the shell by clicking on Y and save the file with name `x.sh` 
    - `bash x.sh` to run the shell script giving us the flag
![Screenshot 2024-10-23 235918](https://github.com/user-attachments/assets/866b06e3-6a19-4c0e-97dc-5482531d4f26)

4) pwn.college{IP2yacqS5B6qoCqmcrJTwSsKyVC.dhTM5QDL0kTM2czW}
    - Use the same script from previous problem but just pipe the output to '/challenge/solve'
    - `bash x.sh | /challenge/solve` will give the flag. 

5) pwn.college{chfTJxTAWf2aQRvALlHxOlr9Jdd.dRzNyUDL0kTM2czW}
    - create script to invoke .sh script invoking /challenge/solve
    - `chmod +x ./uwu.sh`changing perms
    - `./uwu.sh` prints the flag. 

![Screenshot 2024-10-24 000554](https://github.com/user-attachments/assets/7ef86256-bd48-4ad5-ac16-dfcb8023177f)
