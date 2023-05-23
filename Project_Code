class Results():
    def __init__(self, P1, P2):
        self.P1 = P1
        self.P2 = P2
    def tie(self, P1, P2):
        if(P1 == P2):
            return True
        else:
            return False
    def P1win(self, P1, P2):
        if(((P1.upper() == "R") and (P2.upper() == "S")) or ((P1.upper() == "S") and (P2.upper() == "P")) or ((P1.upper() == "P") and (P2.upper() == "R")) or ((P1.upper() == "PAPER") and (P2.upper() == "ROCK")) or ((P1.upper() == "ROCK") and (P2.upper() == "SCISSORS")) or ((P1.upper() == "SCISSORS") and (P2.upper() == "PAPER")) or ((P1.upper() == "ROCK") and (P2.upper() == "SCISSOR")) or ((P1.upper() == "SCISSOR") and (P2.upper() == "PAPER"))):
            return True
        else:
            return False

def Play():
    ValidChoice = False;
    while(ValidChoice == False):
        P1 = input("Player 1; Rock, Paper or Scissors: ")
        if((P1.upper() == "R") or (P1.upper() == "ROCK") or (P1.upper() == "S") or (P1.upper() == "SCISSOR") or (P1.upper() == "SCISSORS") or (P1.upper() == "P") or (P1.upper() == "PAPER")):
            ValidChoice = True
    
    while(ValidChoice == False):
        P2 = input("Player 2; Rock, Paper or Scissors: ")
        if((P2.upper() == "R") or (P2.upper() == "ROCK") or (P2.upper() == "S") or (P2.upper() == "SCISSOR") or (P2.upper() == "SCISSORS") or (P2.upper() == "P") or (P2.upper() == "PAPER")):
            ValidChoice = True
    
    Game = Results(P1, P2)
    if(Game.tie(P1, P2)):
        print("Tie")
    elif(Game.P1win(P1, P2)):
        print("Player 1 wins")
    else:
        print("Player 2 wins")

Status = False

Ans = input("Are you ready to play? ")

if((Ans.lower() == ("y")) or (Ans.lower() == ("yes"))):
    Play()
    Status = True
else:
    Status = False
while(Status == True):
    Ans2 = input("Wanna play again? ")
    if((Ans.lower() == ("y")) or (Ans.lower() == ("yes"))):
        Status = True
        Play()
    else:
        Status = False
