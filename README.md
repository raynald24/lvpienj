#include <iostream>
using namespace std; 

int main(){
	string name, gender, league;
	char genderChoose, again, order;
	int chooseLeague;
	
	do{
		for(int i=0; i<1; i++){
			cout << "************************************************************************************************************" 	<< endl;
			cout << "	                   Welcome to the homepage of stadium's ticket purchase                                  "  << endl;
			cout << "************************************************************************************************************" 	<< endl;
			cout << endl;
		}
		
		//People want to order ticket or no
		cout << "Do you want to order the ticket? [y/n]" << endl;
		do {
			for (int j=0; j<1; j++) {
			cin >> order;
			
			if (order == 'y' || order == 'Y'){
				// Input Data
				cout << "Please input your data : "<< endl	;
				cout << "Name               			= "			; cin >> name;
				cout << "Gender(M for Male/F for Female) 	= "			; bool o = true;
				while (o = true){
					cin >> genderChoose;
				if (genderChoose == 'm' || genderChoose == 'M'){
						gender ="Male";
						o = false;
						continue;
				}
				else if (genderChoose == 'f' || genderChoose == 'F') {
						gender = "Female";
						o = false;
						continue;
				}
				else {
						cout << "Please input the right input" << endl;
				}
				}
				
				//Choose the league
				cout << "Please select the league : " << endl;
				cout << "---------------------------------" << endl;
				cout << "|No. | League				|" << endl;
				cout << "---------------------------------" << endl;
				cout << "|1.  | La Liga				|" << endl;
				cout << "|2.  | Premier League		|" << endl;
				cout << "|3.  | Serie A Italia		|" << endl;
				cout << "|4.  | Bundesliga			|" << endl;
				cout << "|5.  | Ligue 1 Uber Eats	|" << endl;
				cout << "|6.  | World Cup			|" << endl;
				cout << "|7.  | Liga 1 Indonesia	|" << endl;
				cout << "   ---------------------------------" << endl;
				cout << "Input your choice [1/2/3/4/5/6/7] = "; cin >> chooseLeague;
				cout << endl;
				
					switch(chooseLeague){
						case 1 :
							league = "La Liga";
							cout << "You choose the La Liga" << endl;
							break;
						case 2 :
							league = "Premier League";
							cout << "You choose the Premier League" << endl;
							break;	
						case 3 :
							league = "Serie A Italia";
							cout << "You choose the Serie A Italia" << endl;
							break;	
						case 4 :
							league = "Bundesliga";
							cout << "You choose the Bundesliga" << endl;
							break;
						case 5 :
							league = "Ligue 1 Uber Eats";
							cout << "You choose the Ligue 1 Uber Eats" << endl;
							break;
						case 6 :
							league = "World Cup";
							cout << "You choose the World Cup" << endl;
							break;
						case 7 :
							league = "Liga 1 Indonesia";
							cout << "You choose the Liga 1 Indonesia" << endl;
							break;
						default :
							cout << "Wrong Input" << endl;
							cout << endl;
					}
				}
				else if (order == 'n' || order == 'N') {
					cout << "Have a great day, hope you have enough money later" << endl;
				}
				else {
					cout << "Please enter the right input" << endl;
				}
			 }}while (order != 'Y' || order != 'y' || order != 'N' || order != 'n');
				
			
		cout << "Do you want to order the ticket again? (y/n)"; cin >> again;
		
	}while(again == 'y' || again == 'Y');
		cout << "Thank you to order the ticket" << endl;
	
	return 0;
}
