# CatchMeIfYouCan
Game (under process)

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



