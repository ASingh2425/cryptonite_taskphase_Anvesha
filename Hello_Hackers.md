# Report on Hello Hackers Challenges

## Challenge 1 : Intro To Commands

**Step 1:** Opened WSL terminal. Using the ssh keys linked it to pwn.college
`ssh -i ./key hacker@dojo.pwn.college`
It displays `No active challenge session; start a challenge!`, if the challenge is not started. It then closes the connection with a message **Connection to dojo.pwn.college closed.**
If the Challenge is first started and then the connection is established using SSH keys. Its successfully connected.

**Step 2:** Tried executing the same example as the one given in the challenge. Typed `whoami` and received `hacker` as the output.

**Step 3:** Now I understood how to invoke a command. As required I typed `hello` in the next prompt.
I got  the output as:
`Success! Here is your flag:`
`pwn.college{ARZhMbAU5AhS3QMduiqlOL0pMj2.ddjNyUDL0kTM2czW}`

![Screenshot 2024-10-22 074910](https://github.com/user-attachments/assets/9c9d0133-bf3c-4a26-9c7f-2dabed03e6e0)


## Challenge 2 : Intro to Arguments

**Step 1:** Opened WSL and established connection (_using SSH key_) after starting the challenge.

**Step 2:** First executed the `echo` command using two arguments as shown in the example. Then used `hello` command with one argument `hackers`
prompt: `hello hackers`
**OUTPUT RECEIVED**
`Success! Here is your flag:
pwn.college{UJRSjU-PVy49KSO7CJe_MNFTK4k.dhjNyUDL0kTM2czW}`

![Screenshot 2024-10-22 075029](https://github.com/user-attachments/assets/02e4cc61-de58-4d43-8b1d-c8bd7055c2d9)
