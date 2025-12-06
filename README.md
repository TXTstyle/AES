# AES

An AES-128 implementation for the [IS1500](https://www.kth.se/student/kurser/kurs/IS1500) course mini-project. The algorithm includes encrypting/decrypting with both ECB and CBC modes. The project includes a picture of Tux, the Linux mascot, as example input, to prove that the implementation works correctly. Tux will be displayed out of the board's VGA output after encryption and decryption.


## Inputs

Switches on the board are used control the program:

| **Switch** | **Function**               |
|------------|----------------------------|
| 1          | Encryption/Decryption      |
| 2          | ECB/CBC                    |
| 10         | Insert key                 |

In key insert mode, the first 8 switches are used to input the 128-bit key in 16 steps (8 bits at a time). To input a set 8 bits, set the switches(switch 1-8) and then push the button (*btn_1*). Switch 9 resets the key input process. The 7 segement display displays the number of bytes entered so far.

## Run

To run the AES implementation, use the following command:

```bash
make
dtekv-run main.bin
```
