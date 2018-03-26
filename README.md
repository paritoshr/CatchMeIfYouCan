# CatchMeIfYouCan
Game (under process)

Game to Catch your opponent[Guess Current position] .

start with a random genrated Grid of size  5x5 ,6x6 (dynamic take input, bigger the grid more is the difficulty)
Player could set their own positions to start the game . 
player can call out  catch after very loop it has to be the player starting the loop .

A loop is compleated with steps 

* first move is to call out a operator for your oponent 
* opponent set direction on himself 
* Operation combining Operator and direction is preformed 
* Result is notified to the Loop initiator 
* based on this initiator can make a guess and call out a catch for oponents current position 






Operators : + , -, * [can extend or create your Own dynamic]  , works on Curent and next , current * Next or Current - Next 
Directoin : L(Left), R, U(up), D


Methods 

setPosition
SendOperator
Catch


Initial state 5x5 grid with [1-4]

1,2,3,1,2
2,3,1,3,4
3,2,4,1,2
3,4,2,1,2
1,4,3,2,1


Player 1 => setPosition[0,2]    

1,2,3[P1],1,2
2,3,1,3,4
3,2,4,1,2
3,4,2,1,2
1,4,3,2,1


Player 2 => setPosition[3,2]

1,2,3,1,2
2,3,1,3,4
3,2,4,1,2
3,4,2[P2],1,2
1,4,3,2,1

Initiate 
Player1 =>SendOperator(+)   // Current + Next  

Player2 => SetDirection(L)  //(L(Left), R, U(Up), D)

Player 1 Notified with  Result Of operation (2 [current position] + 1(Left)) =3

chance for player to Catch 

Catch([2,3]) current position , Scoring -2 if wrong  



