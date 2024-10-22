# Shell Varibles, 

### Writeups and Flags. 

1) pwn.college{M0QuOas2Frzyx47WUqevROBCIzR.ddTN1QDL0kTM2czW}
    - `echo $FLAG` 
    - '$' refers to a shell varible, echo prints the command. 

2) pwn.college{AY-wgE0bgbexPQ_w0Cjqx4hsc2E.dlTN1QDL0kTM2czW}
    - ` PWN=COLLEGE`
    - prints the flag. 

3) pwn.college{EqoqFi_oDzXOtoVM6QAPIW5N1gh.dBjN1QDL0kTM2czW}
    - `PWN="COLLEGE YEAH"` 
    - needs quotes so shell does interprete it as a new command.
4) pwn.college{MC1773eYbCqcZQhQ5mdi6w58bZO.dJjN1QDL0kTM2czW}
    - Need to export variables so that child processes see them,
    - for the challenge:
    - `PWN=COLLEGE`
    - `export PWN`
    - `COLLEGE=PWN`
    - `/challenge/run` will print the flag. 
![Screenshot 2024-10-22 094803](https://github.com/user-attachments/assets/53082404-fd75-49cd-9596-7e5d0a132252)


5) pwn.college{c37-xo4sFcQpSGDAjoPKk5kkSRS.dhTN1QDL0kTM2czW}
    - `env`  will print all the exported varibles of the shell, 
    - lot of data, hence `env | grep FLAG` gives us the flag. 

6) pwn.college{kiVXqsheRmD9RnXUztBNgYlv76o.dVzN0UDL0kTM2czW}
    - `PWN=$(/challenge/run)`
    - `echo $PWN`

7) pwn.college{IwM36OCHtuf3VbmfUDhTCLWJImW.dhzN1QDL0kTM2czW}
    - 'read'' will read input in terminal on stdin
    - `read PWN` and then enter input `"COLLEGE"` will print the flag. 

8) pwn.college{4_QiZvcgBAAT2IylROZir8UGEdu.dBjM4QDL0kTM2czW}
    - `read PWN < /challenge/read_me` 
    - give in to the stdin of Read which writes it to PWN.
