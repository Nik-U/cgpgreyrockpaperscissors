# Rock, Paper, Scissors Move Generator
This program generates "random" moves to play CGP Grey's rock, paper, scissors game.
Run the program to get the list of moves to play:

```shell
go run github.com/Nik-U/cgpgreyrockpaperscissors@latest
```

Alternatively, you can run the program [directly in the Go Playground](https://go.dev/play/p/ZDVtt2X_l65).

The game can be found here: https://www.youtube.com/watch?v=PmWQmZXYd74

**Do not use this program unless you have already played the game legitimately.**

## The Reality
More truthfully, this program is intended to make a point about "nothing up my sleeve" seeds used to generate cryptographic parameters, such as elliptic curve parameters.

The common approach of hashing an English sentence using a secure cryptographic hash function to derive parameters does not prevent an adversary from choosing parameters that it finds "interesting" (e.g., due to susceptibility to some private attack) if those parameters occur with some reasonable probability, like, say, *one in a trillion*.

In reality, the moves generated by this program are not very "random" or "uncontrolled" at all.
Readers are encouraged to spot the attack in this program.