# Comprehending_commands

## Flags and notes

1) pwn.college{I3Xu_md-Xcgstr4TZQnQO42N85V.dFzN1QDL0kTM2czW}
    - `cat flag` gives us the flag.
  
![image](https://github.com/user-attachments/assets/6eac67fb-ae0f-44c4-acd2-b317f1542d8f)

      
2) pwn.college{gNOu3t_PmLMssCPplg8ZW7LbME-.dlTM5QDL0kTM2czW}
    `cat /flag` gives the flag.

   
3)pwn.college{kHwL_tATkGfkbE5WeHhn3HaqiXZ.dBjM5QDL0kTM2czW}
    - running `cd /` gives us the directory where flag is located. 
    - `cat /opt/angr-management/-internal/flag` gives us the flag. 

![Screenshot 2024-10-21 192040](https://github.com/user-attachments/assets/8a1652eb-dbd8-49d6-a197-e912d529d09a)

    
4) pwn.college{cjzEfEPXoO_zh7b005-pZYrCu3s.ddTM4QDL0kTM2czW}
    - ` grep pwn.college /challenge/data.txt ` gives us the flag,
    - grep matchs the 'pwn.college' string from 'data.txt'
   
5)pwn.college{UxjKiEQEk0n7oGo77dIj5SvjxzE.dhjM4QDL0kTM2czW}
    - `cd /challenge` to get to the directory
    - `ls` lists the files in the directory
    - `./7449-renamed-run-24708` is the renamed run, running the command gives us the flag. 

![image](https://github.com/user-attachments/assets/50b3d7f1-1acc-4415-a684-2e1189fe4fc1)


6)pwn.college{oXBlUzy36bZdrq1mkuMJ-Rgsyr6.dBzM4QDL0kTM2czW}
    - `touch /tmp/pwn`
    - `touch /tmp/college`
    - the above two commanbds create files needed, 
    - `/challenge/run` prints the commands, 

![Screenshot 2024-10-21 193222](https://github.com/user-attachments/assets/19364cd5-2cfc-4496-b9db-349dfbf90600)


7) pwn.college{A1F6qYzuAIK94TNx2Gni5JRDJnA.dZTOwUDL0kTM2czW}
    - `rm delete_me` removes the the file 'delete_me'
    - `/challenge/check` prints the flag.

8)pwn.college{40S3pmQshyToTxi64ysKG1wWLRs.dBTN4QDL0kTM2czW}
    - `cd /` as told in the description
    - ` ls -a` prints the all the files including hidden files,     
    -  `cat  .flag-2376312051133938` prints the flag. 

![Screenshot 2024-10-21 194041](https://github.com/user-attachments/assets/c53f2492-8057-442b-ba4a-dadcd11e3bde)

    
9)pwn.college{MbmmoysPYbHAzEcaFZj1nIHMqi5.dljM4QDL0kTM2czW}
    - use a combination of `ls -a <direcotryname> ` and `cat <directoryname>/<cluefile>` repeatedly
    - will need to sometimes cd into the particular directory to read the next directory,
    - continue the process till you find the last directory printing the flag. 

![image](https://github.com/user-attachments/assets/952b0481-6771-49de-a6e7-44744ac0ac83)
![Screenshot 2024-10-21 195041](https://github.com/user-attachments/assets/fe14fb24-c4d8-4e83-b1f8-a82c18cda433)


10) pwn.college{gChb0gzonDWGB225zIgi5ECODih.dFzM4QDL0kTM2czW}
    - `mkdir /tmp/pwn` will make a directory
    - `touch /tmp/pwn/college` will make a file in the directory created as prescribed.
    - `/challenge/run` will print the flag.

   ![Screenshot 2024-10-21 195630](https://github.com/user-attachments/assets/8b18ec43-7a2b-4d9c-8f89-f534268d8604)
  
11) pwn.college{s1PPlE54aO7NLjx5yOp-jU4kGVb.dJzM4QDL0kTM2czW}
    - `find / -name flag -type f` will print the path to flag. 
    - '/' tells the directory to search 
    - -name is the name of the file
    - -type f specifies that we need to search files by default find searches for directories. 

![Screenshot 2024-10-22 074455](https://github.com/user-attachments/assets/179a466a-d070-495d-8b50-592da3e1c25e)


12) pwn.college{gNoNRwkU0oe1eo_pc4QeGLJaEeh.dlTM1UDL0kTM2czW}
    - we need create a symlink to the /flag directory
    - '/challenge/catflag' will read the the /home/hacker/not-the-flag file,
    - `ln -s /flag /home/hacker/not-the-flag` will create the soft link to not-the-flag file
    - `/challenge/catflag` copy and read out the flag from 'not-the-flag' thus printing the flag to the terminal. 
