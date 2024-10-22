# Processes and Jobs
### Writeups and Flags, 

1) pwn.college{gsdD4R4R7x1I0nuDNGEMDLw1naV.dhzM4QDL0kTM2czW}
    - ps displays processes in the terminal
    - `ps -ef` will give 'every process' in 'full' format. 

2) pwn.college{gWE4NuHjG27JR8HYn2gt-NONaG7.dJDN4QDL0kTM2czW}
    -'kill' is used to kill a process
    - check PID with `ps -ef`
    - `kill <PID>`
![Screenshot 2024-10-22 173729](https://github.com/user-attachments/assets/0e909c9e-bd94-43e2-ae8c-6425505aabb4)

3) pwn.college{YwoEiZFyAuzjImZlKeBdNzRda-8.dNDN4QDL0kTM2czW}
    - `/challenge/run`
    - press ctrl +c to give the flag.

4) pwn.college{4WiCyWpKz_d_7pCHMJHpVgaJSfH.dVDN4QDL0kTM2czW}
    - `/challenge/run`
    - ctrl + z to 'suspend' it background
    - `/challenge/run` again to give us the flag. 

5) pwn.college{guma9-NDkL0FmqVF4CgOWrcPRo9.dZDN4QDL2gTN0czW}
    - `/challenge/run` for the challenges,
    - Ctrl + Z to shift it to the background suspended
    - `fg` to resume it again and give us the flag.

6) pwn.college{8zJkD82XCjaP0vAhTP1vSY9Cjy1.dZDN4QDL0kTM2czW}
    - 'bg' resumes stopped background processes
    - run `/challenge/run` then  'ctrl +z' 
    - `bg` will print the flag.  

7) pwn.college{8cKkQbMBafev5UHI0GUwDlzcOYE.ddDN4QDL0kTM2czW}
    -`/challenge/run`, ctrl +z
    - `bg`
    - `/challenge/run` will give us the flag 

![Screenshot 2024-10-22 175149](https://github.com/user-attachments/assets/acec90a7-238f-4cc6-8272-62faf51ad839)

8) pwn.college{Ml1K1alBX9SKQW_FTu2wJGs9HrL.dhDN4QDL0kTM2czW}
    - & will start the process in the background with suspending, 
    - `/challenge/run &` will give us the flag. 

![Screenshot 2024-10-22 175641](https://github.com/user-attachments/assets/64dda2fe-6d19-46f6-9094-f88942fbcd01)

9) pwn.college{Qgousw3DPG8kEiEupzJNxWcJJWj.dlDN4QDL0kTM2czW}
    - `/challenge/run`
    - append `$` to the command and rerun it
    - `/challenge/run &` gives the flag
![Screenshot 2024-10-22 181206](https://github.com/user-attachments/assets/09c86f04-97ee-4e7b-8638-15d7349ebbd7)

10) pwn.college{sbVYneh9y3a0wo_qKvGyovHSl_0.dljN4UDL0kTM2czW}
    - `$?` to get the code. 
    - `/challenge/get-code` program exits with a error code
    - `echo $?` to get the code
    - `/challenge/submit-code 178` will give the flag.
![Screenshot 2024-10-22 182815](https://github.com/user-attachments/assets/ef1426e3-476d-477b-9eab-a6e4f603d263)
   
