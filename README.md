//# rock-paper-scissor-game-
//enjoy rock paper scissors game ....
   #include<stdio.h>
void playround(int round);
int main(){
	playround(1);
	return 0;
}


	void playround(int round){
	
	char player,computer,again;
	printf("WELCOME TO ROCK PAPER SCISSOR\n");
	printf("enter r for rock p paper s for scissor:\n");
	scanf(" %c",&player);
	if(round%3==1){ 
	
	computer='r';
}
	else if(round%3==2){
	
      computer='p';
	}
	else{
		computer='s';
	}
	printf("you said:%c\n",player);
	printf("computer said:%c\n",computer);
	if(player==computer){
		printf("its a draw\n");
		
	}
	else if ((player=='r'&&computer=='s')||
	(player=='p'&&computer=='r')||
	(player=='s'&&computer=='p')){
		printf("u win\n");
		
	}
	else{
		printf("computer wins\n");
	}
	
	printf("do u want to play again?");
	printf("enter y/n\n");
	scanf(" %c", & again);
	if(again=='y'){
	playround(round+1);
		
	}
	else{
	printf("gameover:\n thnks for playing\nsee u next time");
	}
}

	   
