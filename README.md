//Author : Marcus ALexander Tadili
//Section : HCCL4


//slide 16
//Grade tracker

	  #include <iostream>
 	 using namespace std;

  	int main() {

	int inum;

  	cout << "Grade tracker!\n\n";
	cout << "Type your grade percentage: ";
	cin >> inum;

	if (inum >= 70) {
		cout << "You are A above.\n Congratulation!" << endl;
	}
	else if (inum <= 69 && inum >= 60) {
		cout << "Great job!\n B is your grade!" << endl;
	}
	else if (inum <= 59 && inum >= 50) {
		cout << "Good job! You can do this!\n C is your grade!" << endl;
	}
	else if (inum <= 49 && inum >= 40) {
		cout << "Thats okay! nice try!\n D is your grade!" << endl;
	}
	else if (inum <= 39) {
		cout << "Nice try! You can still do this!\n F is your grade!" << endl;
	}


	return 0;
 	 }


// slide 17
// starting a band

 	 #include <iostream>
  	#include <string>
 	 using namespace std;


 	 int main() {

  	bool musicalFriend = true;
  	string friendPlays = "guitar";
  	string sname;
  	int inum;
  	int Inum;

  	cout << "Enter your friend's name: ";
  	cin >> sname;

  	cout << endl << sname << " you play guitar? " << endl;
  	cout << "Type 1 or 2 only" << endl << "1 = Yes" << endl << "2 = No" << endl;
  	cin >> inum;

  	if (inum == 1)
		musicalFriend = true;
	  if (inum == 2)
		musicalFriend = false;

  	if (musicalFriend == true) {
		cout << sname << ", My friend, we need a person to play guitar. Do you play Guitar or other instruments? " << endl;
		cout << "Type " << endl << "Guitar" << endl << "Other instrument" << endl;
		cin >> friendPlays;

		if ((friendPlays.compare("Guitar") == 0) ||
			(friendPlays.compare("Other instrument") == 0))

			cout << sname << " My friend, Welcome to the band!" << endl;
		else
			cout << sname << " Sorry bro, we really need someone that knows how to play guitar. We still friends by the way"
			<< endl;
  	}
  	if (musicalFriend == false) {
		cout << "Sorry bro, but we still friends right? " << endl;
		cout << "Type 1 or 2 only" << endl << "1 = Yes" << endl << "2 = No" << endl;
		cin >> Inum;

		if (Inum == 1) {
			cout << "Cool! We're still friends!" << endl;
		}
		else if (Inum == 2) {
			cout << "That's okay. " << sname <<" I know you hate me." << endl;
		}
		else {
			cout << "Invalid! " << endl;
		}
  	}
	
  	return 0;
	  }

// slide 19
// killing time

 	 #include <iostream>
 	 using namespace std;


	  int main() {

	int ibored;

	cout << "Killing time!\n";
	cout << "Enter the time your friends going to be late (mins) " << endl;
	cin >> ibored;

	if (ibored >= 15) {

		int pocketMoney;
		cout << "Enter how much money in your pocket: ";
		cin >> pocketMoney;

		if (pocketMoney > 5) {
			cout << "Buy a coffee!" << endl;
		}
		else {
			cout << "Go for a walk around the town!" << endl;
		}
  	}
  	else {
  		cout << "Sit in the food zone and wait!" << endl;
  	}
	  return 0;
   }

// slide 20
// earthquake

 	 #include <iostream>
  	using namespace std;


 	 int main() {

	float magnitude;
	cout << "Earthquake Magnitude!\n";
	cout << "Type the Magnitude: ";
	cin >> magnitude;

	if (magnitude < 2.0 && magnitude > 0)
		cout << magnitude << " is Less than 2.0 - Micro" << endl;
	else if (magnitude >= 2 && magnitude < 3.0)
		cout << magnitude << " is 2.0 to less than 3.0 - Very Minor" << endl;
	else if (magnitude >= 3 && magnitude < 4.0)
		cout << magnitude << " is 3.0 to less than 4.0 - Minor" << endl;
	else if (magnitude >= 4 && magnitude < 5.0)
		cout << magnitude << " is 4.0 to less than 5.0 - Light" << endl;
	else if (magnitude >= 5 && magnitude < 6.0)
		cout << magnitude << " is 5.0 to less than 6.0 - Moderate" << endl;
	else if (magnitude >= 6 && magnitude < 7.0)
		cout << magnitude << " is 6.0 to less than 7.0 - Strong" << endl;
	else if (magnitude >= 7 && magnitude < 8.0)
		cout << magnitude << " is 7.0 to less than 8.0 - Major" << endl;
	else if (magnitude >= 8 && magnitude < 10.0)
		cout << magnitude << " is 8.0 to less than 10.0 - Great" << endl;
	else if (magnitude >= 10)
		cout << magnitude << " is More than 10.0 - Meteoric" << endl;
	else
		cout << magnitude << " is invalid input!" << endl;


	return 0;
 	 }
