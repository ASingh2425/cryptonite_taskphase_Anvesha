# Pondering PATH

### Flags and Writeups, 

1) pwn.college{EK2qToJWlBtzodKSW6FbO4ekuXM.dZzNwUDL0kTM2czW}
    - messing with the PATH variable to so that the 'run' binary cannot find the ls command
    - `PATH=''` this will empty the PATH VARIABLE
    - now running `/challenege/run` will give the flag. 

2) pwn.college{wt7h-bYXxqje9f3mHtuzdePsk9r.dVzNyUDL0kTM2czW}
    - `PATH=/challenge/more_commands/`
    - `/challenge/run` will give the flag,
 
