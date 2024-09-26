```mermaid
flowchart TD
id1((start)) --> 2[gets the random num]
2 --> 3{user guesses a num}
3 -->|correct| 4[done]
3 -->|too much!| 5[do again- go lower]
3 -->|too little!| 6[do again- go higher]
5 --> 3
6 --> 3
4 --> 7[do again?]
7 --> |yes| 2
7 --> |no| id2((end))
```

# The flowchart starts generating the random num then having the user input x number. If the user puts a num higher than the random num then it'll allow them to see it's too much as well as try again and vice versa if it's too little. Finally once guessed it'll allow the user to either try again or end the game.
