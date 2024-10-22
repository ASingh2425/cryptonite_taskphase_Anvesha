# Digesting Documentation
## flags and notes, 

1) pwn.college{sUxyZfX-BMSRS-2EnDy7AMVgQq7.dRjM5QDL0kTM2czW}
	- `/challenge/challenge --giveflag`
	- The challenege is on reading documentation on linux command and understand how to properly use them

 ![Screenshot 2024-10-22 075330](https://github.com/user-attachments/assets/387bcf0d-55f9-4f76-bc31-1821488b0bb1)

2) pwn.college{gL2OsFoQW8t6FFhfGv_6vHJvNvn.dVjM5QDL0kTM2czW}
	- `/challenge/challenge --printfile /flag`
	- As per the given description of the command /challenge/challenge binary reads any file given as an crgument to --printfile.
	- / flag was passed as argument to the file, to print the flag to the challenge solving the challenge. 

![Screenshot 2024-10-22 075605](https://github.com/user-attachments/assets/37929b69-ed71-4a91-b587-6bcf082436e2)


3) pwn.college{kO9uJbtpx8oFA9_ac7sv-9C51jZ.dRTM4QDL0kTM2czW}
	- `man challenge`
	- `/challenge/challenge --kubtpx 989`
	- the man page of challenge gave us info on how to "use" the command, 
	- Followed instructions to read the command.

![Screenshot 2024-10-22 075829](https://github.com/user-attachments/assets/9c889eb7-61c7-42da-981b-d5c50f83f5a9)

4) pwn.college{EU-o3a_-O5D578zC4IcoBwV6Zvh.dVTM4QDL2gTN0czW}
	- searched the documentation using " man challenge "
    - results show on how to get the flag aka `/challenge/challenge --hzsk`

![Screenshot 2024-10-22 080308](https://github.com/user-attachments/assets/78a644f8-6a31-4f4c-8b9a-ed60f332df44)

![Screenshot 2024-10-22 080421](https://github.com/user-attachments/assets/11ce855c-84c0-48d0-b284-2e2bb2e7d04a)

5) pwn.college{UGv69sK6uEQ7XAx8m0UDgLGSq1d.dZTM4QDL0kTM2czW}

	- This was a tricky one couldn't figure out at start how to proceed with the challenge
	- rereading the challenge description, proceeded to read the `man man` page
	- found the command man -k <term to search>
	- That's it !! there it was 
	- Read the man page and solved the challenge. 

![Screenshot 2024-10-22 081123](https://github.com/user-attachments/assets/50a84114-5c1f-4a2c-9354-2393614dab3e)

6) pwn.college{02RFUSTBATML6nrO7oiyZRSQO3X.ddjM4QDL0kTM2czW}
	- Straight forward ran `/challenge/challenge -h`
	- the help page gave all necessary information to solve the challenge. 

![Screenshot 2024-10-22 081456](https://github.com/user-attachments/assets/e899e6ed-5560-4aff-942b-cd6c473a8085)


7) pwn.college{0594kbZv7PNYLcfUeVKfux21Wre.dRTM5QDL0kTM2czW}
	- Challenge Description taught about the shell builtins, 
	- `help challenge` gives us the info about the builtin command "challenge"
    - That's it !! 'challenge --secret 0594kbZv` gives out the flag.
  
![Screenshot 2024-10-22 081715](https://github.com/user-attachments/assets/bda5f298-9370-4858-bd64-c1a9b1c8ef6d)

