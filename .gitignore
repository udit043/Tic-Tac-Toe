#include <iostream>
#include <cstdlib>
#include <conio.h>
#include <windows.h>
using namespace std;
char matrix[3][3];
void cou(void);
int main()
{
	int m,n;
	char ch='y';
	while(ch=='Y'||ch=='y')
	{
		system("cls");
		for (m=0;m<3;m++)
		for (n=0;n<3;n++)
		matrix[m][n]= '\0';
		
		int i,j,clr,sum=0;
		while ( sum < 10)
		{
			if (sum == 0) cou();
			cout<<"Player 1 is 'X': choose the row and column"<<endl;
			cout<<"Row : ";
			cin>>i;
			cout<<"Column : ";
			cin>>j;
			
			for (;i>3 || i<1 || j>3 || j<1 ||('X'==matrix[i-1][j-1]||'O'==matrix[i-1][j-1]);) 
			{
				cout<<"Sorry , you have to choose another place.\n";
				cout<<"row : ";
				cin>>i;
				cout<<"column : ";
				cin>>j;
			}
			matrix[i-1][j-1]='X';
			sum++;
			system("cls");
			cou();

//check if wins
			if (matrix[0][0]=='X' && matrix[0][0]==matrix[1][1] && matrix[1][1]==matrix[2][2]) {cout<<"Player 1 wins"<<endl;break;}
			if (matrix[2][0]=='X' && matrix[2][0]==matrix[1][1] && matrix[1][1]==matrix[0][2]) {cout<<"Player 1 wins"<<endl;break;}
			if (matrix[0][0]=='X' && matrix[0][0]==matrix[1][0] && matrix[1][0]==matrix[2][0]) {cout<<"Player 1 wins"<<endl;break;}
			if (matrix[0][1]=='X' && matrix[0][1]==matrix[1][1] && matrix[1][1]==matrix[2][1]) {cout<<"Player 1 wins"<<endl;break;}
			if (matrix[0][2]=='X' && matrix[0][2]==matrix[1][2] && matrix[1][2]==matrix[2][2]) {cout<<"Player 1 wins"<<endl;break;}
			if (matrix[0][0]=='X' && matrix[0][0]==matrix[0][1] && matrix[0][1]==matrix[0][2]) {cout<<"Player 1 wins"<<endl;break;}
			if (matrix[1][0]=='X' && matrix[1][0]==matrix[1][1] && matrix[1][1]==matrix[1][2]) {cout<<"Player 1 wins"<<endl;break;}
			if (matrix[2][0]=='X' && matrix[2][0]==matrix[2][1] && matrix[2][1]==matrix[2][2]) {cout<<"Player 1 wins"<<endl;break;}

			if (sum == 9){cout<<"The game is over , no one wins !!"<<endl; break;} //sum=9 because there are only 9 boxes in the game
//player 2's turn

			cout<<"Player 2 is 'O': choose the row and column"<<endl;
			cout<<"Row : ";
			cin>>i;
			cout<<"Column : ";
			cin>>j;
			for (;i>3 || i<1 || j>3 || j<1 ||('X'==matrix[i-1][j-1]||'O'==matrix[i-1][j-1]);) 
			{
				cout<<"Sorry , you have to choose another place.\n";
				cout<<"row : ";
				cin>>i;
				cout<<"column : ";
				cin>>j;
			}
			matrix[i-1][j-1]='O';
			sum++;
			//the play box
			system("cls");
			cou();
			//check if wins
			if (matrix[0][0]=='O' && matrix[0][0]==matrix[1][1] && matrix[1][1]==matrix[2][2]) {cout<<"Player 2 wins"<<endl;break;}
			if (matrix[2][0]=='O' && matrix[2][0]==matrix[1][1] && matrix[1][1]==matrix[0][2]) {cout<<"Player 2 wins"<<endl;break;}
			if (matrix[0][0]=='O' && matrix[0][0]==matrix[1][0] && matrix[1][0]==matrix[2][0]) {cout<<"Player 2 wins"<<endl;break;}
			if (matrix[0][1]=='O' && matrix[0][1]==matrix[1][1] && matrix[1][1]==matrix[2][1]) {cout<<"Player 2 wins"<<endl;break;}
			if (matrix[0][2]=='O' && matrix[0][2]==matrix[1][2] && matrix[1][2]==matrix[2][2]) {cout<<"Player 2 wins"<<endl;break;}
			if (matrix[0][0]=='O' && matrix[0][0]==matrix[0][1] && matrix[0][1]==matrix[0][2]) {cout<<"Player 2 wins"<<endl;break;}
			if (matrix[1][0]=='O' && matrix[1][0]==matrix[1][1] && matrix[1][1]==matrix[1][2]) {cout<<"Player 2 wins"<<endl;break;}
			if (matrix[2][0]=='O' && matrix[2][0]==matrix[2][1] && matrix[2][1]==matrix[2][2]) {cout<<"Player 2 wins"<<endl;break;}
	
		}
		cout<<"\nWould you like to play again??? (Y - N)\n";
		cin>>ch;
	}
    Sleep(2000);
    return 0;
}

void cou(void)
{
	//the play box
	gotoxy(28,2);
	textcolor(15);
	cout<<"\n\t\t                1   2   3\n"<<endl;
	cout<<"\t\t             1  ";if(matrix[0][0]=='X') textcolor(11); else textcolor(14); cout<<matrix[0][0];textcolor(15);cout<<" | ";if(matrix[0][1]=='X') textcolor(11); else textcolor(14); cout<<matrix[0][1];textcolor(15);cout<<" | ";if(matrix[0][2]=='X') textcolor(11); else textcolor(14); cout<<matrix[0][2];textcolor(15);cout<<endl;
	cout<<"\t\t               ---|---|---\n";
	cout<<"\t\t             2  ";if(matrix[1][0]=='X') textcolor(11); else textcolor(14); cout<<matrix[1][0];textcolor(15);cout<<" | ";if(matrix[1][1]=='X') textcolor(11); else textcolor(14); cout<<matrix[1][1];textcolor(15);cout<<" | ";if(matrix[1][2]=='X') textcolor(11); else textcolor(14); cout<<matrix[1][2];textcolor(15);cout<<endl;
	cout<<"\t\t               ---|---|---\n";
	cout<<"\t\t             3  ";if(matrix[2][0]=='X') textcolor(11); else textcolor(14); cout<<matrix[2][0];textcolor(15);cout<<" | ";if(matrix[2][1]=='X') textcolor(11); else textcolor(14); cout<<matrix[2][1];textcolor(15);cout<<" | ";if(matrix[2][2]=='X') textcolor(11); else textcolor(14); cout<<matrix[2][2];textcolor(15);cout<<"\n\n\n";
	textcolor(15);
}

