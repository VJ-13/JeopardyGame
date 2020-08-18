import java.util.Scanner;
public class Game {
	public static void categories() {
		//method to represent the categories
		String[] categories={"History(1)", "Geography(2)", "Math(3)", "Science(4)", "Computer(5)", "Sports(6)"};
		//categories is set to a string with array 
		System.out.println();
		//adds a line
		System.out.println("Board: ");
		System.out.println("_________________________________________________________________________________________________________________________________________________");
		//prints the outline of the board
		for(int a=0; a<categories.length; a++) {
			System.out.print(categories[a] + "             ");
			//prints the categories in order to represent the board
		}
		System.out.print("\t|");
		//prints the outline of the board
		System.out.println();
		//adds a line
	}


	public static void questions(int x) {
		//method to represent the question with the parameter to print specific question
		String[] questions=new String[30];
		//question is set to a string with array 

		//History Questions
		questions[0]= "What year did World War 1 Started?";//History 200
		questions[1]= "Who is the Father of History?";//History 400
		questions[2]= "\'Mein Kampf\' is the autobiography of which political leader?";//History 600
		questions[3]= "Which year did the first Ancient Greek Olympic Game ocuured?";//History 800
		questions[4]= "Who built the Great Wall of China?"; //History 1000

		//Geography Questions
		questions[5]= "What is Earth's largest continent?"; //Geography 200
		questions[6]="What country has the most natural lakes?"; //Geography 400
		questions[7]="What is the driest place on Earth?"; //Geography 600
		questions[8]="What is the oldest city in the world?"; //Geography 800
		questions[9]="What is the only continent with land in all four hemispheres?"; //Geography 1000

		//Math Questions
		questions[10]= "Choose a prime number: "; //Math 200
		questions[11]="What number does \"giga\" stand for?"; //Math 400
		questions[12]="How many square feet are there in a square yard?"; //Math 600
		questions[13]="What Greek mathematician noticed that the morning star and evening star were one and the same, in 530 B.C.?"; //Math 800
		questions[14]="I am the first positive number (aside from one) that is both a square and a cube number. What am I?"; //Math 1000

		//Science Questions
		questions[15]="What planet is farthest from the sun?"; //Science 200
		questions[16]="How many new species are discovered each year?"; //Science 400
		questions[17]="Which of the following evolved first?"; //Science 600
		questions[18]="What is the most abundant element in the Universe?"; //Science 800
		questions[19]=" What layer of the Earth's atmosphere makes radio communications possible?"; //Science 1000

		//Computer Questions
		questions[20]="In computer terminology, what does RAM stands for?"; //Computer 200
		questions[21]="What was the first portable computer?"; //Computer 400
		questions[22]="Convert this binary\'10001111\' into decimal."; //Computer 600
		questions[23]="How many megabytes(MB) are in a terabytes(TB)?"; //Computer 800
		questions[24]="What company developed a computer with the codename \"Lisa\" in the 1980's?"; //Computer 1000

		//Sports Questions
		questions[25]="What is Canada's national sport"; //Sports 200
		questions[26]="Who won the NBA Championship in 2019?"; //Sports 400
		questions[27]="What country won the first World Cup?"; //Sports 600
		questions[28]="When did Canada first host the Olympics?"; //Sports 800
		questions[29]="Who is the most decorated Olympian of all time?"; //Sports 1000

		System.out.println(questions[x]);
		//prints the question with the parameter used in the method
	}
	public static void answers(int y) {
		//method to represent the answers with the parameter to print the specific multiple choice for the questions
		String[][] answers=new String[30][4];
		//answers is set to a string with a two dimensional array

		//History Answers
		answers[0][0]= "A.1918";
		answers[0][1]= "B.1914";
		answers[0][2]= "C.1819";
		answers[0][3]= "D.1939";
		//History 200 the correct answer is B
		answers[1][0]= "A.Thucydides";
		answers[1][1]= "B.Archimedes";
		answers[1][2]= "C.Herodotus";
		answers[1][3]= "D.Homer";
		//History 400 the correct answer is C
		answers[2][0]= "A.Joseph Stalin";
		answers[2][1]= "B.Benito Mussoline";
		answers[2][2]= "C.Winston Churchill";
		answers[2][3]= "D.Adolf Hitler";
		//History 600 the correct answer is D
		answers[3][0]= "A.776 BC";
		answers[3][1]= "B.552 BC";
		answers[3][2]= "C.800 BC";
		answers[3][3]= "D.235 BC";
		//History 800 the correct answer is A
		answers[4][0]= "A.Gaozu of Han";
		answers[4][1]= "B.Han Wudi";
		answers[4][2]= "C.Xuande";
		answers[4][3]= "D.Qin Shi Huang";
		//History 1000 the correct answer is D

		//Geography Answers
		answers[5][0]= "A.Asia";
		answers[5][1]= "B.Europe";
		answers[5][2]= "C.Antarctica";
		answers[5][3]= "D.Africa";
		//Geography 200 the correct answer is A
		answers[6][0]= "A.Australia";
		answers[6][1]= "B.India";
		answers[6][2]= "C.Canada";
		answers[6][3]= "D.United States";
		//Geography 400 the correct answer is C
		answers[7][0]= "A.Sahara Desert";
		answers[7][1]= "B.Kufra, Librya";
		answers[7][2]= "C.Atacama Desert";
		answers[7][3]= "D.McMurdo, Antarctica";
		//Geography 600 the correct answer is D
		answers[8][0]= "A.Jericho";
		answers[8][1]= "B.Damascus";
		answers[8][2]= "C.Athens";
		answers[8][3]= "D.Jerusalem";
		//Geography 800 the correct answer is B
		answers[9][0]= "A.Antarctica";
		answers[9][1]= "B.Africa";
		answers[9][2]= "C.Australia";
		answers[9][3]= "D.Asia";
		//Geography 1000 the correct answer is B

		//Math Answers
		answers[10][0]= "A.67";
		answers[10][1]= "B.33";
		answers[10][2]= "C.56";
		answers[10][3]= "D.49";
		//Math 200 the correct answer is A
		answers[11][0]= "A.One quadrillion";
		answers[11][1]= "B.One billion";
		answers[11][2]= "C.One million";
		answers[11][3]= "D.One trillion";
		//Math 400 the correct answer is B
		answers[12][0]= "A.9";
		answers[12][1]= "B.12";
		answers[12][2]= "C.3";
		answers[12][3]= "D.36";
		//Math 600 the correct answer is A
		answers[13][0]= "A.Thales of Miletus";
		answers[13][1]= "B.Archimedes";
		answers[13][2]= "C.Euclid";
		answers[13][3]= "D.Pythagoras";
		//Math 800 the correct answer is D
		answers[14][0]= "A.16";
		answers[14][1]= "B.32";
		answers[14][2]= "C.64";
		answers[14][3]= "D.128";
		//Math 1000 the correct answer is C

		//Science Answers
		answers[15][0]= "A.Pluto";
		answers[15][1]= "B.Neptune";
		answers[15][2]= "C.Uranus";
		answers[15][3]= "D.Saturn";
		//Science 200 the correct answer is B
		answers[16][0]= "A.8,000";
		answers[16][1]= "B.80";
		answers[16][2]= "C.1,800";
		answers[16][3]= "D.18,000";
		//Science 400 the correct answer is D
		answers[17][0]= "A.Cockroaches";
		answers[17][1]= "B.Trees";
		answers[17][2]= "C.Humans";
		answers[17][3]= "D.Sharks";
		//Science 600 the correct answer is D
		answers[18][0]= "A.Lithium";
		answers[18][1]= "B.Helium";
		answers[18][2]= "C.Hydrogen";
		answers[18][3]= "D.Oxygen";
		//Science 800 the correct answer is C
		answers[19][0]= "A.Ionosphere";
		answers[19][1]= "B.Stratosphere";
		answers[19][2]= "C.Exosphere";
		answers[19][3]= "D.Thermosphere";
		//Science 1000 the correct answer is A

		//Computer Answers
		answers[20][0]= "A.Read Acess Memory";
		answers[20][1]= "B.Random Alternative Memory";
		answers[20][2]= "C.Random Acess Memory";
		answers[20][3]= "D.Read All Memory";
		//Computer 200 the correct answer is C
		answers[21][0]= "A.Epson HX-20";
		answers[21][1]= "B.Osborne I";
		answers[21][2]= "C.Cray I";
		answers[21][3]= "D.IBM 5155";
		//Computer 400 the correct answer is B
		answers[22][0]= "A.143";
		answers[22][1]= "B.160";
		answers[22][2]= "C.79";
		answers[22][3]= "D.95";
		//Computer 600 the correct answer is A
		answers[23][0]= "A.100000 MB";
		answers[23][1]= "B.131072 MB";
		answers[23][2]= "C.1024 MB";
		answers[23][3]= "D.1048576 MB";
		//Computer 800 the correct answer is D
		answers[24][0]= "A.Apple";
		answers[24][1]= "B.Microsoft";
		answers[24][2]= "C.IBM";
		answers[24][3]= "D.Commodore";
		//Computer 1000 the correct answer is A

		//Sports Answers
		answers[25][0]= "A.Lacrosse";
		answers[25][1]= "B.Football";
		answers[25][2]= "C.Basketball";
		answers[25][3]= "D.Ice Hockey";
		//Sports 200 the correct answer is D
		answers[26][0]= "A.Los Angeles Clippers";
		answers[26][1]= "B.Los Angeles Lakers";
		answers[26][2]= "C.The Toronto Raptors";
		answers[26][3]= "D.Golden State Warriors";
		//Sports 400 the correct answer is C
		answers[27][0]= "A.Argentina";
		answers[27][1]= "B.Switzerland";
		answers[27][2]= "C.Uruguay";
		answers[27][3]= "D.Brazil";
		//Sports 600 the correct answer is C
		answers[28][0]= "A.2010";
		answers[28][1]= "B.1976";
		answers[28][2]= "C.1896";
		answers[28][3]= "D.1980";
		//Sports 800 the correct answer is B
		answers[29][0]= "A.Carl Lewis";
		answers[29][1]= "B.Michael Phelps";
		answers[29][2]= "C.Paavo Nurmi";
		answers[29][3]= "D.Mary Lou Retton";
		//Sports 1000 the correct answer is B

		for(int x=0; x<answers[0].length; x++) {
			//loops through the elements of the two dimensional array 
			System.out.println(answers[y][x]);
			//prints the all the multiple choice for the specific question
		}
	}
	public static void correctanswer(int x) {
		//method to represent the correctanswer with the parameter to print the specific answer
		String[] correctanswer=new String[30];
		//correctanswer is set to a string with array

		//History
		correctanswer[0]= "B.1914";
		correctanswer[1]= "C.Herodotus";
		correctanswer[2]= "D.Adolf Hitler";
		correctanswer[3]= "A.776 BC";
		correctanswer[4]= "D.Qin Shi Huang";

		//Geography
		correctanswer[5]= "A.Asia";
		correctanswer[6]= "C.Canada";
		correctanswer[7]= "D.McMurdo, Antarctica";
		correctanswer[8]= "B.Damascus";
		correctanswer[9]= "B.Africa";

		//Math
		correctanswer[10]= "A.67";
		correctanswer[11]= "B.One billion";
		correctanswer[12]= "A.9";
		correctanswer[13]= "D.Pythagoras";
		correctanswer[14]= "C.64";

		//Science
		correctanswer[15]= "B.Neptune";
		correctanswer[16]= "D.18,000";
		correctanswer[17]= "D.Sharks";
		correctanswer[18]= "C.Hydrogen";
		correctanswer[19]= "A.Ionosphere";

		//Computer
		correctanswer[20]= "C.Random Acess Memory";
		correctanswer[21]= "B.Osborne I";
		correctanswer[22]= "A.143";
		correctanswer[23]= "D.1048576 MB";
		correctanswer[24]= "A.Apple";

		//Sports
		correctanswer[25]= "D.Ice Hockey";
		correctanswer[26]= "C.The Toronto Raptors";
		correctanswer[27]= "C.Uruguay";
		correctanswer[28]= "B.1976";
		correctanswer[29]= "B.Michael Phelps";

		System.out.println(correctanswer[x]);
		//prints the correctanswer with the parameter used in the method
	}
	public static void rules() {
		//method to represent the rules 

		System.out.println();
		System.out.println("How to play:");
		System.out.println("1. Player one picks the category by picking the coresponding number.");
		System.out.println("2. Player one picks the points.");
		System.out.println("3. Then the player one answer's the question given, by choosing the coresponding alapahbet.");
		System.out.println("4. If the answer is correct, the player get the points but if its wrong he gets no points.");
		System.out.println("5. After a point in the category is choosen it will be shown as 0 meaning you may not pick it again.");
		System.out.println("6. If accidentally you pick the same points in the same category your turn will be skipped.");
		System.out.println("7. After Player one turn, Player two choses the category by picking the coresponding number.");
		System.out.println("8. Player two picks the points.");
		System.out.println("9. Then the player two answer's the question given by choosing the coresponding alapahbet.");
		System.out.println("10. If the answer is correct the player gets the points but if its wrong he gets no points.");
		System.out.println("11. This continues until all the points from all the category is represented by 0.");
		System.out.println();
		System.out.println("Now you are ready to play the game.");
		System.out.println("Hope you enjoy it.");
		System.out.println();
		//prints the rules for the players
	}

	public static void main(String[] args) {
		
//START
		Scanner in=new Scanner(System.in);
		
	//Welcomes the Players
		String start, playerOne = null, playerTwo=null; 
		//start, playerOne and playerTwo is set to a String value
		System.out.println();
		//adds a line
		System.out.println("Welcome to Jeopardy");
		System.out.println();
		//adds a line
		System.out.println("Would you like to see how to play the game?");
		System.out.println("Type \"yes\" to see how to play the game and \"no\" to start the game:");
		//prompt the user
		start=in.next();
		//gets the input from the user
		while(!start.equals("yes") && !start.equals("Yes") && !start.equals("no") && !start.equals("No") ) {
			//checks if the user wrote anything except yes, Yes, no, No
			//it keeps running until a valid input is entered by the user
			System.out.println("--------------------------------------------------");
			System.out.println("There is an Error put yes or no only");
			//shows an error
			System.out.println("Type \"yes\" to see how to play the game and \"no\" to start the game:");
			//prompt the user again
			start=in.next();
			//gets the input from the user
		}
		if(start.equals("yes") || start.equals("Yes")) {
			//runs if the user inputed yes or Yes 
			rules();
			//prints the rules to play the game
		}
		System.out.println("Player 1 enter your name: ");
		//prompt the user
		playerOne=in.next();
		//gets input from the user
		System.out.println("Player 2 enter your name: ");
		//prompt the user
		playerTwo=in.next();
		//gets input from the user
		System.out.println("Hello " + playerOne + " and " + playerTwo);
		System.out.println("Preparing the board...");
		//Welcome's the players
		int p1c_category, p1c_points, p1points = 0,p2c_category, p2c_points, p2points = 0;
		//p1c_category, p2c_category, p1c_points, p2c_points, p1points, p2points is set to a integer value
		String p1answer,p2answer; 
		//p1answer and p2answer is set to a string value
		
	//Initialize the points 
		int[][] points= new int[6][6];
		//points is set to integer with array
		for(int i=0; i<6; i++) {
			//loops through the array index
			for(int j=0; j<6; j++) {
				//loops through the elements
				points[i][j]=j*200;
				//initializes all the points 
			}
		}

	//Loops through the code until all the points are 0
		for(int i=1; i<points.length; i++) {
			//loops through the array index
			for(int j=0; j<points[0].length; j++) {
				//loops through the elements
				while(points[j][i]!=0) {
					//checks if all the points is equal to 0 
					//keeps running until all the points are equal to 0

//PLAYER ONE TURN

	//Prints The Board 
					categories();
					//prints the categories
					for(int o=1; o<points.length; o++) {
						//loops through the array index
						for(int p=0; p<points[0].length; p++) {
							//loops through the elements
							System.out.print(points[p][o]+ "\t\t\t");
							//prints all the points
						}
						System.out.print("|");
						//prints the outline for the board
						System.out.println();
						//adds a line
					}
					System.out.println("________________________________________________________________________________________________________________________________________________|");
					//prints the outline for the board
					System.out.println();
					//adds a line

	//Prompt The User For Categories
					System.out.println(playerOne + " what category would you like to choose (Choose a coresponding number): ");
					//prompt the user
					p1c_category=in.nextInt();
					//gets the input from user
					while (p1c_category<0 || p1c_category>6) {
						//keeps running until a valid input of category is not placed
						System.out.println("--------------------------------------------------");
						System.out.println("There is an Error put the number from 1 to 6 coresponding to the catrgory");
						//shows an error
						System.out.println(playerOne + " what category would you like to choose(Choose a coresponding number): ");
						//prompt the user again
						p1c_category=in.nextInt();
						//prompt the user again
					}

	//Prompt The User For Points
					System.out.println(playerOne + " Select the amount of points for category " + p1c_category + ": ");
					//prompt the user
					p1c_points=in.nextInt();
					//gets the input from the user
					while(p1c_points!= 200 && p1c_points!= 400 && p1c_points!= 600 && p1c_points!= 800 && p1c_points!= 1000) {
						//keeps running until a valid input of points is placed
						System.out.println("--------------------------------------------------");
						System.out.println("There is an Error put the number coresponding to the points");
						//shows an error
						System.out.println(playerOne + " Select the amount of points for category " + p1c_category + ": ");
						//prompt the user again
						p1c_points=in.nextInt();
						//prompt the user again
					}

					p1c_category=p1c_category-1;
					//the category is minus by 1 to make it easier for the coder and the user

	//Category 0 History(1) For Player One

					if(p1c_category==0) {
						//runs if the category inputed by the user is History(1)
		//Points 200
						if(p1c_points==200) {
							//runs if the points inputed by the user is 200
							while(points[p1c_category][1]!=0) {
								//keeps running until the points selected is equal to 0
								int k=0;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k);
								//prints the multiple choice
								System.out.println(playerOne + " Choose the corresponding alpahbet:");
								//prompt the user
								p1answer=in.next();
								//gets the input
								while(!p1answer.equals("a") && !p1answer.equals("A") && !p1answer.equals("b") && !p1answer.equals("B") && !p1answer.equals("c") && !p1answer.equals("C") && !p1answer.equals("d") && !p1answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerOne + " Choose the corresponding alpahbet:");
									//prompt the user again
									p1answer=in.next();
									//gets the input again
								}
								if (p1answer.equals("b") || p1answer.equals("B")) {
									//runs if the answer inputed by the user is b or B
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									p1points= p1points+p1c_points;
									//calculates the points
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p1c_category][1]=0;
								//makes the points selected to 0 so it can't be chosen again
							}

						}

		//Points 400
						else if(p1c_points==400) {
							//runs if the points inputed by the user is 400
							while(points[p1c_category][2]!=0) {
								//keeps running until the points selected is equal to 0
								int k=1;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k);
								//prints the multiple choice
								System.out.println(playerOne + " Choose the corresponding alpahbet:");
								//prompt the user
								p1answer=in.next();
								//gets the input
								while(!p1answer.equals("a") && !p1answer.equals("A") && !p1answer.equals("b") && !p1answer.equals("B") && !p1answer.equals("c") && !p1answer.equals("C") && !p1answer.equals("d") && !p1answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerOne + " Choose the corresponding alpahbet:");
									//prompt the user again
									p1answer=in.next();
									//gets the input again
								}
								if (p1answer.equals("c") || p1answer.equals("C")) {
									//runs if the answer inputed by the user is c or C
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p1points= p1points+p1c_points;
									//calculates the points
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p1c_category][2]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}

		//Points 600
						else if(p1c_points==600) {	
							//runs if the points inputed by the user is 600
							while(points[p1c_category][3]!=0) {
								//keeps running until the points selected is equal to 0
								int k=2;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k);
								//prints the multiple choice
								System.out.println(playerOne + " Choose the corresponding alpahbet:");
								//prompt the user
								p1answer=in.next();
								//gets the input from the user
								while(!p1answer.equals("a") && !p1answer.equals("A") && !p1answer.equals("b") && !p1answer.equals("B") && !p1answer.equals("c") && !p1answer.equals("C") && !p1answer.equals("d") && !p1answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerOne + " Choose the corresponding alpahbet:");
									//prompt the user again
									p1answer=in.next();
									//gets the input from the user again
								}
								if (p1answer.equals("d") || p1answer.equals("D")) {
									//runs if the answer inputed by the user is d or D
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p1points= p1points+p1c_points;
									//calculates the points
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p1c_category][3]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}

		//Points 800
						else if(p1c_points==800) {
							//runs if the points inputed by the user is 800
							while(points[p1c_category][4]!=0) {
								//keeps running until the points selected is equal to 0
								int k=3;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k);
								//prints the answer
								System.out.println(playerOne + " Choose the corresponding alpahbet:");
								//prompt the user
								p1answer=in.next();
								//gets the input by the user
								while(!p1answer.equals("a") && !p1answer.equals("A") && !p1answer.equals("b") && !p1answer.equals("B") && !p1answer.equals("c") && !p1answer.equals("C") && !p1answer.equals("d") && !p1answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerOne + " Choose the corresponding alpahbet:");
									//prompt the user again
									p1answer=in.next();
									//gets the input from the user again
								}
								if (p1answer.equals("a") || p1answer.equals("A")) {
									//runs if the answer inputed by the user is a or A
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p1points= p1points+p1c_points;
									System.out.println("Your points are: " + p1points);
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p1c_category][4]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}

		//Points 1000
						else if(p1c_points==1000) {
							//runs if the points inputed by the user is 1000
							while(points[p1c_category][5]!=0) {
								//keeps running until the points selected is equal to 0
								int k=4;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k);
								//prints the answer
								System.out.println(playerOne + " Choose the corresponding alpahbet:");
								//prompt the user
								p1answer=in.next();
								//gets the input from the user
								while(!p1answer.equals("a") && !p1answer.equals("A") && !p1answer.equals("b") && !p1answer.equals("B") && !p1answer.equals("c") && !p1answer.equals("C") && !p1answer.equals("d") && !p1answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerOne + " Choose the corresponding alpahbet:");
									//prompt the user again
									p1answer=in.next();
									//gets the input from the user again
								}
								if (p1answer.equals("d") || p1answer.equals("D")) {
									//runs if the answer inputed by the user is d or D
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p1points= p1points+p1c_points;
									System.out.println("Your points are: " + p1points);
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p1c_category][5]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}

					}

	//Category 1 Geography(2) For Player One
					if(p1c_category==1) {
						//runs if the category inputed by the user is Geography(2)
		//Points 200			
						if(p1c_points==200) {
							//runs if the points inputed by the user is 200
							while(points[p1c_category][1]!=0) {
								//keeps running until the points selected is equal to 0
								int k=5;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k);
								//prints the answer
								System.out.println(playerOne + " Choose the corresponding alpahbet:");
								//prompt the user
								p1answer=in.next();
								//gets input from the user
								while(!p1answer.equals("a") && !p1answer.equals("A") && !p1answer.equals("b") && !p1answer.equals("B") && !p1answer.equals("c") && !p1answer.equals("C") && !p1answer.equals("d") && !p1answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerOne + " Choose the corresponding alpahbet:");
									//prompt the user again
									p1answer=in.next();
									//gets input from the user again
								}
								if (p1answer.equals("a") || p1answer.equals("A")) {
									//runs if the answer inputed by the user is a or A
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p1points= p1points+p1c_points;
									//calculates the points
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p1c_category][1]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}

		//Points 400
						else if(p1c_points==400) {
							//runs if the points inputed by the user is 400
							while(points[p1c_category][2]!=0) {
								//keeps running until the points selected is equal to 0
								int k=6;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k);
								//prints the answer
								System.out.println(playerOne + " Choose the corresponding alpahbet:");
								//prompt the user
								p1answer=in.next();
								//gets input from the user
								while(!p1answer.equals("a") && !p1answer.equals("A") && !p1answer.equals("b") && !p1answer.equals("B") && !p1answer.equals("c") && !p1answer.equals("C") && !p1answer.equals("d") && !p1answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerOne + " Choose the corresponding alpahbet:");
									//prompt the user again
									p1answer=in.next();
									//gets input from the user again
								}
								if (p1answer.equals("c") || p1answer.equals("C")) {
									//runs if the answer inputed by the user is c or C
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p1points= p1points+p1c_points;
									//calculates the points
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p1c_category][2]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}

		//Points 600	
						else if(p1c_points==600) {
							//runs if the points inputed by the user is 600
							while(points[p1c_category][3]!=0) {
								//keeps running until the points selected is equal to 0
								int k=7;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k);
								//prints the answer
								System.out.println(playerOne + " Choose the corresponding alpahbet:");
								//prompt the user
								p1answer=in.next();
								//gets input from the user
								while(!p1answer.equals("a") && !p1answer.equals("A") && !p1answer.equals("b") && !p1answer.equals("B") && !p1answer.equals("c") && !p1answer.equals("C") && !p1answer.equals("d") && !p1answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerOne + " Choose the corresponding alpahbet:");
									//prompt the user again
									p1answer=in.next();
									//gets input from the user again
								}
								if (p1answer.equals("d") || p1answer.equals("D")) {
									//runs if the answer inputed by the user is d or D
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p1points= p1points+p1c_points;
									//calculates the points
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p1c_category][3]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}

		//Points 800
						else if(p1c_points==800) {	
							//runs if the points inputed by the user is 800
							while(points[p1c_category][4]!=0) {
								//keeps running until the points selected is equal to 0
								int k=8;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k);
								//prints the answer
								System.out.println(playerOne + " Choose the corresponding alpahbet:");
								//prompt the user
								p1answer=in.next();
								//gets input from the user
								while(!p1answer.equals("a") && !p1answer.equals("A") && !p1answer.equals("b") && !p1answer.equals("B") && !p1answer.equals("c") && !p1answer.equals("C") && !p1answer.equals("d") && !p1answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerOne + " Choose the corresponding alpahbet:");
									//prompt the user again
									p1answer=in.next();
									//gets input from the user again
								}
								if (p1answer.equals("b") || p1answer.equals("B")) {
									//runs if the answer inputed by the user is b or B
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p1points= p1points+p1c_points;
									//calculates the points
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p1c_category][4]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}

		//Points 1000
						else if(p1c_points==1000) {
							//runs if the points inputed by the user is 1000
							while(points[p1c_category][5]!=0) {
								//keeps running until the points selected is equal to 0
								int k=9;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k);
								//prints the answer
								System.out.println(playerOne + " Choose the corresponding alpahbet:");
								//prompt the user
								p1answer=in.next();
								//gets input from the user
								while(!p1answer.equals("a") && !p1answer.equals("A") && !p1answer.equals("b") && !p1answer.equals("B") && !p1answer.equals("c") && !p1answer.equals("C") && !p1answer.equals("d") && !p1answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerOne + " Choose the corresponding alpahbet:");
									//prompt the user again
									p1answer=in.next();
									//gets input from the user again
								}
								if (p1answer.equals("b") || p1answer.equals("B")) {
									//runs if the answer inputed by the user is b or B
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p1points= p1points+p1c_points;
									//calculates the points
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p1c_category][5]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}

					}

	//Category 2 Math(3) For Player One
					if(p1c_category==2) {
						//runs if the category inputed by the user is Math(3)
		//Points 200			
						if(p1c_points==200) {
							//runs if the points inputed by the user is 200
							while(points[p1c_category][1]!=0) {
								//keeps running until the points selected is equal to 0
								int k=10;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k);
								//prints the answer
								System.out.println(playerOne + " Choose the corresponding alpahbet:");
								//prompt the user
								p1answer=in.next();
								//gets input from the user
								while(!p1answer.equals("a") && !p1answer.equals("A") && !p1answer.equals("b") && !p1answer.equals("B") && !p1answer.equals("c") && !p1answer.equals("C") && !p1answer.equals("d") && !p1answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerOne + " Choose the corresponding alpahbet:");
									//prompt the user again
									p1answer=in.next();
									//gets input from the user again
								}
								if (p1answer.equals("a") || p1answer.equals("A")) {
									//runs if the answer inputed by the user is a or A
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p1points= p1points+p1c_points;
									//calculates the points
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p1c_category][1]=0;
								//makes the points selected to 0 so it can't be chosen again
							}

						}

		//Points 400
						else if(p1c_points==400) {
							//runs if the points inputed by the user is 400
							while(points[p1c_category][2]!=0) {
								//keeps running until the points selected is equal to 0
								int k=11;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k);
								//prints the answer
								System.out.println(playerOne + " Choose the corresponding alpahbet:");
								//prompt the user
								p1answer=in.next();
								//gets input from the user
								while(!p1answer.equals("a") && !p1answer.equals("A") && !p1answer.equals("b") && !p1answer.equals("B") && !p1answer.equals("c") && !p1answer.equals("C") && !p1answer.equals("d") && !p1answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerOne + " Choose the corresponding alpahbet:");
									//prompt the user again
									p1answer=in.next();
									//gets input from the user again
								}
								if (p1answer.equals("b") || p1answer.equals("B")) {
									//runs if the answer inputed by the user is b or B
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p1points= p1points+p1c_points;
									//calculates the points
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p1c_category][2]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}

		//Points 600
						else if(p1c_points==600) {
							//runs if the points inputed by the user is 600
							while(points[p1c_category][3]!=0) {
								//keeps running until the points selected is equal to 0
								int k=12;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k);
								//prints the answer
								System.out.println(playerOne + " Choose the corresponding alpahbet:");
								//prompt the user
								p1answer=in.next();
								//gets input from the user
								while(!p1answer.equals("a") && !p1answer.equals("A") && !p1answer.equals("b") && !p1answer.equals("B") && !p1answer.equals("c") && !p1answer.equals("C") && !p1answer.equals("d") && !p1answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerOne + " Choose the corresponding alpahbet:");
									//prompt the user again
									p1answer=in.next();
									//gets input from the user again
								}
								if (p1answer.equals("a") || p1answer.equals("A")) {
									//runs if the answer inputed by the user is a or A
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p1points= p1points+p1c_points;
									//calculates the points
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p1c_category][3]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}

		//Points 800
						else if(p1c_points==800) {
							//runs if the points inputed by the user is 800
							while(points[p1c_category][4]!=0) {
								//keeps running until the points selected is equal to 0
								int k=13;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k);
								//prints the answer
								System.out.println(playerOne + " Choose the corresponding alpahbet:");
								//prompt the user
								p1answer=in.next();
								//gets input from the user
								while(!p1answer.equals("a") && !p1answer.equals("A") && !p1answer.equals("b") && !p1answer.equals("B") && !p1answer.equals("c") && !p1answer.equals("C") && !p1answer.equals("d") && !p1answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerOne + " Choose the corresponding alpahbet:");
									//prompt the user again
									p1answer=in.next();
									//gets input from the user again
								}
								if (p1answer.equals("d") || p1answer.equals("D")) {
									//runs if the answer inputed by the user is d or D
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p1points= p1points+p1c_points;
									//calculates the points
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p1c_category][4]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}

		//Points 1000
						else if(p1c_points==1000) {
							//runs if the points inputed by the user is 1000
							while(points[p1c_category][5]!=0) {
								//keeps running until the points selected is equal to 0
								int k=14;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k);
								//prints the answer
								System.out.println(playerOne + " Choose the corresponding alpahbet:");
								//prompt the user
								p1answer=in.next();
								//gets input from the user
								while(!p1answer.equals("a") && !p1answer.equals("A") && !p1answer.equals("b") && !p1answer.equals("B") && !p1answer.equals("c") && !p1answer.equals("C") && !p1answer.equals("d") && !p1answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerOne + " Choose the corresponding alpahbet:");
									//prompt the user again
									p1answer=in.next();
									//gets input from the user again
								}
								if (p1answer.equals("c") || p1answer.equals("C")) {
									//runs if the answer inputed by the user is c or C
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p1points= p1points+p1c_points;
									//calculates the points
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p1c_category][5]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}

					}

	//Category 3 Science(4) For Player One
					if(p1c_category==3) {
						//runs if the category inputed by the user is Science(4)
		//Points 200
						if(p1c_points==200) {
							//runs if the points inputed by the user is 200
							while(points[p1c_category][1]!=0) {
								//keeps running until the points selected is equal to 0
								int k=15;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k);
								//prints the answer
								System.out.println(playerOne + " Choose the corresponding alpahbet:");
								//prompt the user
								p1answer=in.next();
								//gets input from the user
								while(!p1answer.equals("a") && !p1answer.equals("A") && !p1answer.equals("b") && !p1answer.equals("B") && !p1answer.equals("c") && !p1answer.equals("C") && !p1answer.equals("d") && !p1answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerOne + " Choose the corresponding alpahbet:");
									//prompt the user again
									p1answer=in.next();
									//gets input from the user again
								}
								if (p1answer.equals("b") || p1answer.equals("B")) {
									//runs if the answer inputed by the user is b or B
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p1points= p1points+p1c_points;
									//calculates the points
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p1c_category][1]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}

		//Points 400
						else if(p1c_points==400) {	
							//runs if the points inputed by the user is 400
							while(points[p1c_category][2]!=0) {
								//keeps running until the points selected is equal to 0
								int k=16;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k);
								//prints the answer
								System.out.println(playerOne + " Choose the corresponding alpahbet:");
								//prompt the user
								p1answer=in.next();
								//gets input from the user
								while(!p1answer.equals("a") && !p1answer.equals("A") && !p1answer.equals("b") && !p1answer.equals("B") && !p1answer.equals("c") && !p1answer.equals("C") && !p1answer.equals("d") && !p1answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerOne + " Choose the corresponding alpahbet:");
									//prompt the user again
									p1answer=in.next();
									//gets input from the user again
								}
								if (p1answer.equals("d") || p1answer.equals("D")) {
									//runs if the answer inputed by the user is d or D
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p1points= p1points+p1c_points;
									//calculates the points
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p1c_category][2]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}

		//Points 600
						else if(p1c_points==600) {
							//runs if the points inputed by the user is 600
							while(points[p1c_category][3]!=0) {
								//keeps running until the points selected is equal to 0
								int k=17;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k);
								//prints the answer
								System.out.println(playerOne + " Choose the corresponding alpahbet:");
								//prompt the user
								p1answer=in.next();
								//gets input from the user
								while(!p1answer.equals("a") && !p1answer.equals("A") && !p1answer.equals("b") && !p1answer.equals("B") && !p1answer.equals("c") && !p1answer.equals("C") && !p1answer.equals("d") && !p1answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerOne + " Choose the corresponding alpahbet:");
									//prompt the user again
									p1answer=in.next();
									//gets input from the user again
								}
								if (p1answer.equals("d") || p1answer.equals("D")) {
									//runs if the answer inputed by the user is d or D
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p1points= p1points+p1c_points;
									//calculates the points
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p1c_category][3]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}

		//Points 800
						else if(p1c_points==800) {
							//runs if the points inputed by the user is 800
							while(points[p1c_category][4]!=0) {
								//keeps running until the points selected is equal to 0
								int k=18;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k);
								//prints the answer
								System.out.println(playerOne + " Choose the corresponding alpahbet:");
								//prompt the user
								p1answer=in.next();
								//gets input from the user
								while(!p1answer.equals("a") && !p1answer.equals("A") && !p1answer.equals("b") && !p1answer.equals("B") && !p1answer.equals("c") && !p1answer.equals("C") && !p1answer.equals("d") && !p1answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerOne + " Choose the corresponding alpahbet:");
									//prompt the user again
									p1answer=in.next();
									//gets input from the user again
								}
								if (p1answer.equals("c") || p1answer.equals("C")) {
									//runs if the answer inputed by the user is c or C
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p1points= p1points+p1c_points;
									//calculates the points
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p1c_category][4]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}

		//Points 1000
						else if(p1c_points==1000) {
							//runs if the points inputed by the user is 1000
							while(points[p1c_category][5]!=0) {
								//keeps running until the points selected is equal to 0
								int k=19;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k);
								//prints the answer
								System.out.println(playerOne + " Choose the corresponding alpahbet:");
								//prompt the user
								p1answer=in.next();
								//gets input from the user
								while(!p1answer.equals("a") && !p1answer.equals("A") && !p1answer.equals("b") && !p1answer.equals("B") && !p1answer.equals("c") && !p1answer.equals("C") && !p1answer.equals("d") && !p1answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerOne + " Choose the corresponding alpahbet:");
									//prompt the user again
									p1answer=in.next();
									//gets input from the user again
								}
								if (p1answer.equals("a") || p1answer.equals("A")) {
									//runs if the answer inputed by the user is a or A
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p1points= p1points+p1c_points;
									//calculates the points
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p1c_category][5]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}			
					}
	//Category 4 Computer(5) For Player One
					if(p1c_category==4) {
						//runs if the category inputed by the user is Computer(5)
		//Points 200
						if(p1c_points==200) {	
							//runs if the points inputed by the user is 200
							while(points[p1c_category][1]!=0) {
								//keeps running until the points selected is equal to 0
								int k=20;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k);
								//prints the answer
								System.out.println(playerOne + " Choose the corresponding alpahbet:");
								//prompt the user
								p1answer=in.next();
								//gets input from the user
								while(!p1answer.equals("a") && !p1answer.equals("A") && !p1answer.equals("b") && !p1answer.equals("B") && !p1answer.equals("c") && !p1answer.equals("C") && !p1answer.equals("d") && !p1answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerOne + " Choose the corresponding alpahbet:");
									//prompt the user again
									p1answer=in.next();
									//gets input from the user again
								}
								if (p1answer.equals("c") || p1answer.equals("C")) {
									//runs if the answer inputed by the user is c or C
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p1points= p1points+p1c_points;
									//calculates the points
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p1c_category][1]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}

		//Points 400
						else if(p1c_points==400) {				
							//runs if the points inputed by the user is 400
							while(points[p1c_category][2]!=0) {
								//keeps running until the points selected is equal to 0
								int k=21;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k);
								//prints the answer
								System.out.println(playerOne + " Choose the corresponding alpahbet:");
								//prompt the user
								p1answer=in.next();
								//gets input from the user
								while(!p1answer.equals("a") && !p1answer.equals("A") && !p1answer.equals("b") && !p1answer.equals("B") && !p1answer.equals("c") && !p1answer.equals("C") && !p1answer.equals("d") && !p1answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerOne + " Choose the corresponding alpahbet:");
									//prompt the user again
									p1answer=in.next();
									//gets input from the user again
								}
								if (p1answer.equals("b") || p1answer.equals("B")) {
									//runs if the answer inputed by the user is b or B
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p1points= p1points+p1c_points;
									//calculates the points
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p1c_category][2]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}

		//Points 600
						else if(p1c_points==600) {	
							//runs if the points inputed by the user is 600
							while(points[p1c_category][3]!=0) {
								//keeps running until the points selected is equal to 0
								int k=22;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k);
								//prints the answer
								System.out.println(playerOne + " Choose the corresponding alpahbet:");
								//prompt the user
								p1answer=in.next();
								//gets input from the user
								while(!p1answer.equals("a") && !p1answer.equals("A") && !p1answer.equals("b") && !p1answer.equals("B") && !p1answer.equals("c") && !p1answer.equals("C") && !p1answer.equals("d") && !p1answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerOne + " Choose the corresponding alpahbet:");
									//prompt the user again
									p1answer=in.next();
									//gets input from the user again
								}
								if (p1answer.equals("a") || p1answer.equals("A")) {
									//runs if the answer inputed by the user is a or A
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p1points= p1points+p1c_points;
									//calculates the points
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p1c_category][3]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}

		//Points 800
						else if(p1c_points==800) {
							//runs if the points inputed by the user is 800
							while(points[p1c_category][4]!=0) {
								//keeps running until the points selected is equal to 0
								int k=23;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k);
								//prints the answer
								System.out.println(playerOne + " Choose the corresponding alpahbet:");
								//prompt the user
								p1answer=in.next();
								//gets input from the user
								while(!p1answer.equals("a") && !p1answer.equals("A") && !p1answer.equals("b") && !p1answer.equals("B") && !p1answer.equals("c") && !p1answer.equals("C") && !p1answer.equals("d") && !p1answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerOne + " Choose the corresponding alpahbet:");
									//prompt the user again
									p1answer=in.next();
									//gets input from the user again
								}
								if (p1answer.equals("d") || p1answer.equals("D")) {
									//runs if the answer inputed by the user is d or D
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p1points= p1points+p1c_points;
									//calculates the points
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p1c_category][4]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}

		//Points 1000
						else if(p1c_points==1000) {
							//runs if the points inputed by the user is 1000
							while(points[p1c_category][5]!=0) {
								//keeps running until the points selected is equal to 0
								int k=24;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k);
								//prints the answer
								System.out.println(playerOne + " Choose the corresponding alpahbet:");
								//prompt the user
								p1answer=in.next();
								//gets input from the user
								while(!p1answer.equals("a") && !p1answer.equals("A") && !p1answer.equals("b") && !p1answer.equals("B") && !p1answer.equals("c") && !p1answer.equals("C") && !p1answer.equals("d") && !p1answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerOne + " Choose the corresponding alpahbet:");
									//prompt the user again
									p1answer=in.next();
									//gets input from the user again
								}
								if (p1answer.equals("a") || p1answer.equals("A")) {
									//runs if the answer inputed by the user is a or A
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p1points= p1points+p1c_points;
									//calculates the points
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p1c_category][5]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}		
					}
					
	//Category 5 Sports(6) For Player One
					if(p1c_category==5) {
						//runs if the category inputed by the user is Sports(6)
		//Points 200
						if(p1c_points==200) {	
							//runs if the points inputed by the user is 200
							while(points[p1c_category][1]!=0) {
								//keeps running until the points selected is equal to 0
								int k=25;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k);
								//prints the answer
								System.out.println(playerOne + " Choose the corresponding alpahbet:");
								//prompt the user
								p1answer=in.next();
								//gets input from the user
								while(!p1answer.equals("a") && !p1answer.equals("A") && !p1answer.equals("b") && !p1answer.equals("B") && !p1answer.equals("c") && !p1answer.equals("C") && !p1answer.equals("d") && !p1answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerOne + " Choose the corresponding alpahbet:");
									//prompt the user again
									p1answer=in.next();
									//gets input from the user again
								}
								if (p1answer.equals("d") || p1answer.equals("D")) {
									//runs if the answer inputed by the user is d or D
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p1points= p1points+p1c_points;
									//calculates the points
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p1c_category][1]=0;
								//makes the points selected to 0 so it can't be chosen again
							}					
						}

		//Points 400
						else if(p1c_points==400) {
							//runs if the points inputed by the user is 400
							while(points[p1c_category][2]!=0) {
								//keeps running until the points selected is equal to 0
								int k=26;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k);
								//prints the answer
								System.out.println(playerOne + " Choose the corresponding alpahbet:");
								//prompt the user
								p1answer=in.next();
								//gets input from the user
								while(!p1answer.equals("a") && !p1answer.equals("A") && !p1answer.equals("b") && !p1answer.equals("B") && !p1answer.equals("c") && !p1answer.equals("C") && !p1answer.equals("d") && !p1answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerOne + " Choose the corresponding alpahbet:");
									//prompt the user again
									p1answer=in.next();
									//gets input from the user again
								}
								if (p1answer.equals("c") || p1answer.equals("C")) {
									//runs if the answer inputed by the user is c or C
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p1points= p1points+p1c_points;
									//calculates the points
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p1c_category][2]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}

		//Points 600
						else if(p1c_points==600) {
							//runs if the points inputed by the user is 600
							while(points[p1c_category][3]!=0) {
								//keeps running until the points selected is equal to 0
								int k=27;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k);
								//prints the answer
								System.out.println(playerOne + " Choose the corresponding alpahbet:");
								//prompt the user
								p1answer=in.next();
								//gets input from the user
								while(!p1answer.equals("a") && !p1answer.equals("A") && !p1answer.equals("b") && !p1answer.equals("B") && !p1answer.equals("c") && !p1answer.equals("C") && !p1answer.equals("d") && !p1answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerOne + " Choose the corresponding alpahbet:");
									//prompt the user again
									p1answer=in.next();
									//gets input from the user again
								}
								if (p1answer.equals("c") || p1answer.equals("C")) {
									//runs if the answer inputed by the user is c or C
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p1points= p1points+p1c_points;
									//calculates the points
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p1c_category][3]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}

			//Points 800
						else if(p1c_points==800) {	
							//runs if the points inputed by the user is 800
							while(points[p1c_category][4]!=0) {
								//keeps running until the points selected is equal to 0
								int k=28;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k);
								//prints the answer
								System.out.println(playerOne + " Choose the corresponding alpahbet:");
								//prompt the user
								p1answer=in.next();
								//gets input from the user
								while(!p1answer.equals("a") && !p1answer.equals("A") && !p1answer.equals("b") && !p1answer.equals("B") && !p1answer.equals("c") && !p1answer.equals("C") && !p1answer.equals("d") && !p1answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerOne + " Choose the corresponding alpahbet:");
									//prompt the user again
									p1answer=in.next();
									//gets input from the user again
								}
								if (p1answer.equals("b") || p1answer.equals("B")) {
									//runs if the answer inputed by the user is c or C
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p1points= p1points+p1c_points;
									//calculates the points
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p1c_category][4]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}
						
		//Points 1000
						else if(p1c_points==1000) {
							//runs if the points inputed by the user is 1000
							while(points[p1c_category][5]!=0) {
								//keeps running until the points selected is equal to 0
								int k=29;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k);
								//prints the answer
								System.out.println(playerOne + " Choose the corresponding alpahbet:");
								//prompt the user
								p1answer=in.next();
								//gets input from the user
								while(!p1answer.equals("a") && !p1answer.equals("A") && !p1answer.equals("b") && !p1answer.equals("B") && !p1answer.equals("c") && !p1answer.equals("C") && !p1answer.equals("d") && !p1answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerOne + " Choose the corresponding alpahbet:");
									//prompt the user again
									p1answer=in.next();
									//gets input from the user again
								}
								if (p1answer.equals("b") || p1answer.equals("B")) {
									//runs if the answer inputed by the user is c or C
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p1points= p1points+p1c_points;
									//calculates the points
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p1points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p1c_category][5]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}							
					}
								
//PLAYER TWO TURN

	//Prints The Board 
					categories();
					//prints the categories
					for(int o=1; o<points.length; o++) {
						//loops through the array index
						for(int p=0; p<points[0].length; p++) {
							//loops through the elements
							System.out.print(points[p][o]+ "\t\t\t");
							//prints all the points
						}
						System.out.print("|");
						//prints the outline for the board
						System.out.println();
						//adds a line
					}
					System.out.println("________________________________________________________________________________________________________________________________________________|");
					//prints the outline for the board
					System.out.println();
					//adds a line

	//Prompt The User For Categories
					System.out.println(playerTwo + " what category would you like to choose (Choose a coresponding number): ");
					//prompt the user
					p2c_category=in.nextInt();
					//gets the input from user
					while (p2c_category<0 || p2c_category>6) {
						//keeps running until a valid input of category is not placed
						System.out.println("--------------------------------------------------");
						System.out.println("There is an Error put the number from 1 to 6 coresponding to the catrgory");
						//shows an error
						System.out.println(playerTwo + " what category would you like to choose (Choose a coresponding number): ");
						//prompt the user again
						p2c_category=in.nextInt();
						//gets the input from user again
					}

	//Prompt The User For Points
					System.out.println(playerTwo + " Select the amount of points for category " + p2c_category + ": ");
					//prompt the user
					p2c_points=in.nextInt();
					//gets the input from user
					while(p2c_points!= 200 && p2c_points!= 400 && p2c_points!= 600 && p2c_points!= 800 && p2c_points!= 1000) {
						//keeps running until a valid input of category is not placed
						System.out.println("--------------------------------------------------");
						System.out.println("There is an Error put the number coresponding to the points");
						//shows an error
						System.out.println(playerTwo + " Select the amount of points for category " + p2c_category + ": ");
						//prompt the user again
						p2c_points=in.nextInt();
						//gets the input from user again
					}
					p2c_category=p2c_category-1;
					//the category is minus by 1 to make it easier for the coder and the user

	//Category 0 History(1) For Player Two							
					if(p2c_category==0) {
						//runs if the category inputed by the user is History(1)
		//Points 200
						if(p2c_points==200) {
							//runs if the points inputed by the user is 200
							while(points[p2c_category][1]!=0) {
								//keeps running until the points selected is equal to 0
								int k=0;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k); 
								//prints the answer
								System.out.println(playerTwo + " Choose the corresponding alpahbet:");
								//prompt user
								p2answer=in.next();
								//gets input from user
								while(!p2answer.equals("a") && !p2answer.equals("A") && !p2answer.equals("b") && !p2answer.equals("B") && !p2answer.equals("c") && !p2answer.equals("C") && !p2answer.equals("d") && !p2answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerTwo + " Choose the corresponding alpahbet:");
									//prompt user again
									p2answer=in.next();
									//gets input from user again
								}
								if (p2answer.equals("b") || p2answer.equals("B")) {
									//runs if the answer inputed by the user is b or B
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p2points= p2points+p2c_points;
									//calculates the points
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p2c_category][1]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}

		//Points 400
						else if(p2c_points==400) {
							//runs if the points inputed by the user is 400
							while(points[p2c_category][2]!=0) {
								//keeps running until the points selected is equal to 0
								int k=1;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k); 
								//prints the answer
								System.out.println(playerTwo + " Choose the corresponding alpahbet:");
								//prompt user
								p2answer=in.next();
								//gets input from user
								while(!p2answer.equals("a") && !p2answer.equals("A") && !p2answer.equals("b") && !p2answer.equals("B") && !p2answer.equals("c") && !p2answer.equals("C") && !p2answer.equals("d") && !p2answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerTwo + " Choose the corresponding alpahbet:");
									//prompt user again
									p2answer=in.next();
									//gets input from user again
								}
								if (p2answer.equals("c") || p2answer.equals("C")) {
									//runs if the answer inputed by the user is c or C
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p2points= p2points+p2c_points;
									//calculates the points
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p2c_category][2]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}
						
		//Points 600
						else if(p2c_points==600) {
							//runs if the points inputed by the user is 600
							while(points[p2c_category][3]!=0) {
								//keeps running until the points selected is equal to 0
								int k=2;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k); 
								//prints the answer
								System.out.println(playerTwo + " Choose the corresponding alpahbet:");
								//prompt user
								p2answer=in.next();
								//gets input from user
								while(!p2answer.equals("a") && !p2answer.equals("A") && !p2answer.equals("b") && !p2answer.equals("B") && !p2answer.equals("c") && !p2answer.equals("C") && !p2answer.equals("d") && !p2answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerTwo + " Choose the corresponding alpahbet:");
									//prompt user again
									p2answer=in.next();
									//gets input from user again
								}
								if (p2answer.equals("d") || p2answer.equals("D")) {
									//runs if the answer inputed by the user is d or D
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p2points= p2points+p2c_points;
									//calculates the points
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p2c_category][3]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}
						
			//Points 800
						else if(p2c_points==800) {	
							//runs if the points inputed by the user is 800
							while(points[p2c_category][4]!=0) {
								//keeps running until the points selected is equal to 0
								int k=3;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k); 
								//prints the answer
								System.out.println(playerTwo + " Choose the corresponding alpahbet:");
								//prompt user
								p2answer=in.next();
								//gets input from user
								while(!p2answer.equals("a") && !p2answer.equals("A") && !p2answer.equals("b") && !p2answer.equals("B") && !p2answer.equals("c") && !p2answer.equals("C") && !p2answer.equals("d") && !p2answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerTwo + " Choose the corresponding alpahbet:");
									//prompt user again
									p2answer=in.next();
									//gets input from user again
								}
								if (p2answer.equals("a") || p2answer.equals("A")) {
									//runs if the answer inputed by the user is a or A
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p2points= p2points+p2c_points;
									//calculates the points
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p2c_category][4]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}

		//Points 1000
						else if(p2c_points==1000) {
							//runs if the points inputed by the user is 1000
							while(points[p2c_category][5]!=0) {
								//keeps running until the points selected is equal to 0
								int k=4;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k); 
								//prints the answer
								System.out.println(playerTwo + " Choose the corresponding alpahbet:");
								//prompt user
								p2answer=in.next();
								//gets input from user
								while(!p2answer.equals("a") && !p2answer.equals("A") && !p2answer.equals("b") && !p2answer.equals("B") && !p2answer.equals("c") && !p2answer.equals("C") && !p2answer.equals("d") && !p2answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerTwo + " Choose the corresponding alpahbet:");
									//prompt user again
									p2answer=in.next();
									//gets input from user again
								}
								if (p2answer.equals("d") || p2answer.equals("D")) {
									//runs if the answer inputed by the user is d or D
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p2points= p2points+p2c_points;
									//calculates the points
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p2c_category][5]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}				
					}

	//Category 1 Geography(2) For Player Two							
					if(p2c_category==1) {
						//runs if the category inputed by the user is Geography(2)
		//Points 200
						if(p2c_points==200) {
							//runs if the points inputed by the user is 200
							while(points[p2c_category][1]!=0) {
								//keeps running until the points selected is equal to 0
								int k=5;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k); 
								//prints the answer
								System.out.println(playerTwo + " Choose the corresponding alpahbet:");
								//prompt user
								p2answer=in.next();
								//gets input from user
								while(!p2answer.equals("a") && !p2answer.equals("A") && !p2answer.equals("b") && !p2answer.equals("B") && !p2answer.equals("c") && !p2answer.equals("C") && !p2answer.equals("d") && !p2answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerTwo + " Choose the corresponding alpahbet:");
									//prompt user again
									p2answer=in.next();
									//gets input from user again
								}
								if (p2answer.equals("a") || p2answer.equals("A")) {
									//runs if the answer inputed by the user is a or A
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p2points= p2points+p2c_points;
									//calculates the points
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p2c_category][1]=0;
								//makes the points selected to 0 so it can't be chosen again
							}	
						}

		//Points 400
						else if(p2c_points==400) {	
							//runs if the points inputed by the user is 400
							while(points[p2c_category][2]!=0) {
								//keeps running until the points selected is equal to 0
								int k=6;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k); 
								//prints the answer
								System.out.println(playerTwo + " Choose the corresponding alpahbet:");
								//prompt user
								p2answer=in.next();
								//gets input from user
								while(!p2answer.equals("a") && !p2answer.equals("A") && !p2answer.equals("b") && !p2answer.equals("B") && !p2answer.equals("c") && !p2answer.equals("C") && !p2answer.equals("d") && !p2answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerTwo + " Choose the corresponding alpahbet:");
									//prompt user again
									p2answer=in.next();
									//gets input from user again
								}
								if (p2answer.equals("c") || p2answer.equals("C")) {
									//runs if the answer inputed by the user is c or C
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p2points= p2points+p2c_points;
									//calculates the points
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p2c_category][2]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}

			//Points 600
						else if(p2c_points==600) {
							//runs if the points inputed by the user is 600
							while(points[p2c_category][3]!=0) {
								//keeps running until the points selected is equal to 0
								int k=7;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k); 
								//prints the answer
								System.out.println(playerTwo + " Choose the corresponding alpahbet:");
								//prompt user
								p2answer=in.next();
								//gets input from user
								while(!p2answer.equals("a") && !p2answer.equals("A") && !p2answer.equals("b") && !p2answer.equals("B") && !p2answer.equals("c") && !p2answer.equals("C") && !p2answer.equals("d") && !p2answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerTwo + " Choose the corresponding alpahbet:");
									//prompt user again
									p2answer=in.next();
									//gets input from user again
								}
								if (p2answer.equals("d") || p2answer.equals("D")) {
									//runs if the answer inputed by the user is d or D
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p2points= p2points+p2c_points;
									//calculates the points
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p2c_category][3]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}

		//Points 800
						else if(p2c_points==800) {	
							//runs if the points inputed by the user is 800
							while(points[p2c_category][4]!=0) {
								//keeps running until the points selected is equal to 0
								int k=8;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k); 
								//prints the answer
								System.out.println(playerTwo + " Choose the corresponding alpahbet:");
								//prompt user
								p2answer=in.next();
								//gets input from user
								while(!p2answer.equals("a") && !p2answer.equals("A") && !p2answer.equals("b") && !p2answer.equals("B") && !p2answer.equals("c") && !p2answer.equals("C") && !p2answer.equals("d") && !p2answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerTwo + " Choose the corresponding alpahbet:");
									//prompt user again
									p2answer=in.next();
									//gets input from user again
								}
								if (p2answer.equals("b") || p2answer.equals("B")) {
									//runs if the answer inputed by the user is b or B
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p2points= p2points+p2c_points;
									//calculates the points
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p2c_category][4]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}

		//Points 1000
						else if(p2c_points==1000) {
							//runs if the points inputed by the user is 1000
							while(points[p2c_category][5]!=0) {
								//keeps running until the points selected is equal to 0
								int k=9;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k); 
								//prints the answer
								System.out.println(playerTwo + " Choose the corresponding alpahbet:");
								//prompt user
								p2answer=in.next();
								//gets input from user
								while(!p2answer.equals("a") && !p2answer.equals("A") && !p2answer.equals("b") && !p2answer.equals("B") && !p2answer.equals("c") && !p2answer.equals("C") && !p2answer.equals("d") && !p2answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerTwo + " Choose the corresponding alpahbet:");
									//prompt user again
									p2answer=in.next();
									//gets input from user again
								}
								if (p2answer.equals("b") || p2answer.equals("B")) {
									//runs if the answer inputed by the user is b or B
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p2points= p2points+p2c_points;
									//calculates the points
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p2c_category][5]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}			
					}

	//Category 2 Math(3) For Player Two	
					if(p2c_category==2) {
						//runs if the category inputed by the user is Math(3)
		//Points 200
						if(p2c_points==200) {	
							//runs if the points inputed by the user is 200
							while(points[p2c_category][1]!=0) {
								//keeps running until the points selected is equal to 0
								int k=10;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k); 
								//prints the answer
								System.out.println(playerTwo + " Choose the corresponding alpahbet:");
								//prompt user
								p2answer=in.next();
								//gets input from user
								while(!p2answer.equals("a") && !p2answer.equals("A") && !p2answer.equals("b") && !p2answer.equals("B") && !p2answer.equals("c") && !p2answer.equals("C") && !p2answer.equals("d") && !p2answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerTwo + " Choose the corresponding alpahbet:");
									//prompt user again
									p2answer=in.next();
									//gets input from user again
								}
								if (p2answer.equals("a") || p2answer.equals("A")) {
									//runs if the answer inputed by the user is a or A
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p2points= p2points+p2c_points;
									//calculates the points
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p2c_category][1]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}

			//Points 400
						else if(p2c_points==400) {
							//runs if the points inputed by the user is 400
							while(points[p2c_category][2]!=0) {
								//keeps running until the points selected is equal to 0
								int k=11;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k); 
								//prints the answer
								System.out.println(playerTwo + " Choose the corresponding alpahbet:");
								//prompt user
								p2answer=in.next();
								//gets input from user
								while(!p2answer.equals("a") && !p2answer.equals("A") && !p2answer.equals("b") && !p2answer.equals("B") && !p2answer.equals("c") && !p2answer.equals("C") && !p2answer.equals("d") && !p2answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerTwo + " Choose the corresponding alpahbet:");
									//prompt user again
									p2answer=in.next();
									//gets input from user again
								}
								if (p2answer.equals("b") || p2answer.equals("B")) {
									//runs if the answer inputed by the user is b or B
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p2points= p2points+p2c_points;
									//calculates the points
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p2c_category][2]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}

		//Points 600
						else if(p2c_points==600) {
							//runs if the points inputed by the user is 600
							while(points[p2c_category][3]!=0) {
								//keeps running until the points selected is equal to 0
								int k=12;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k); 
								//prints the answer
								System.out.println(playerTwo + " Choose the corresponding alpahbet:");
								//prompt user
								p2answer=in.next();
								//gets input from user
								while(!p2answer.equals("a") && !p2answer.equals("A") && !p2answer.equals("b") && !p2answer.equals("B") && !p2answer.equals("c") && !p2answer.equals("C") && !p2answer.equals("d") && !p2answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerTwo + " Choose the corresponding alpahbet:");
									//prompt user again
									p2answer=in.next();
									//gets input from user again
								}
								if (p2answer.equals("a") || p2answer.equals("A")) {
									//runs if the answer inputed by the user is a or A
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p2points= p2points+p2c_points;
									//calculates the points
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p2c_category][3]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}

		//Points 800
						else if(p2c_points==800) {
							//runs if the points inputed by the user is 800
							while(points[p2c_category][4]!=0) {
								//keeps running until the points selected is equal to 0
								int k=13;
								questions(k);
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k); 
								//prints the answer
								System.out.println(playerTwo + " Choose the corresponding alpahbet:");
								//prompt user
								p2answer=in.next();
								//gets input from user
								while(!p2answer.equals("a") && !p2answer.equals("A") && !p2answer.equals("b") && !p2answer.equals("B") && !p2answer.equals("c") && !p2answer.equals("C") && !p2answer.equals("d") && !p2answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerTwo + " Choose the corresponding alpahbet:");
									//prompt user again
									p2answer=in.next();
									//gets input from user again
								}
								if (p2answer.equals("d") || p2answer.equals("D")) {
									//runs if the answer inputed by the user is d or D
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p2points= p2points+p2c_points;
									//calculates the points
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p2c_category][4]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}

		//Points 1000
						else if(p2c_points==1000) {
							//runs if the points inputed by the user is 1000
							while(points[p2c_category][5]!=0) {
								//keeps running until the points selected is equal to 0
								int k=14;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k); 
								//prints the answer
								System.out.println(playerTwo + " Choose the corresponding alpahbet:");
								//prompt user
								p2answer=in.next();
								//gets input from user
								while(!p2answer.equals("a") && !p2answer.equals("A") && !p2answer.equals("b") && !p2answer.equals("B") && !p2answer.equals("c") && !p2answer.equals("C") && !p2answer.equals("d") && !p2answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerTwo + " Choose the corresponding alpahbet:");
									//prompt user again
									p2answer=in.next();
									//gets input from user again
								}
								if (p2answer.equals("c") || p2answer.equals("C")) {
									//runs if the answer inputed by the user is c or C
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p2points= p2points+p2c_points;
									//calculates the points
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p2c_category][5]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}				
					}

	//Category 3 Science(4) For Player Two				
					if(p2c_category==3) {
						//runs if the category inputed by the user is Science(4)
		//Points 200
						if(p2c_points==200) {
							//runs if the points inputed by the user is 200
							while(points[p2c_category][1]!=0) {
								//keeps running until the points selected is equal to 0
								int k=15;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k); 
								//prints the answer
								System.out.println(playerTwo + " Choose the corresponding alpahbet:");
								//prompt user
								p2answer=in.next();
								//gets input from user
								while(!p2answer.equals("a") && !p2answer.equals("A") && !p2answer.equals("b") && !p2answer.equals("B") && !p2answer.equals("c") && !p2answer.equals("C") && !p2answer.equals("d") && !p2answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerTwo + " Choose the corresponding alpahbet:");
									//prompt user again
									p2answer=in.next();
									//gets input from user again
								}
								if (p2answer.equals("b") || p2answer.equals("B")) {
									//runs if the answer inputed by the user is b or B
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p2points= p2points+p2c_points;
									//calculates the points
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p2c_category][1]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}

		//Points 400
						else if(p2c_points==400) {	
							//runs if the points inputed by the user is 400
							while(points[p2c_category][2]!=0) {
								//keeps running until the points selected is equal to 0
								int k=16;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k); 
								//prints the answer
								System.out.println(playerTwo + " Choose the corresponding alpahbet:");
								//prompt user
								p2answer=in.next();
								//gets input from user
								while(!p2answer.equals("a") && !p2answer.equals("A") && !p2answer.equals("b") && !p2answer.equals("B") && !p2answer.equals("c") && !p2answer.equals("C") && !p2answer.equals("d") && !p2answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerTwo + " Choose the corresponding alpahbet:");
									//prompt user again
									p2answer=in.next();
									//gets input from user again
								}
								if (p2answer.equals("d") || p2answer.equals("D")) {
									//runs if the answer inputed by the user is d or D
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p2points= p2points+p2c_points;
									//calculates the points
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p2c_category][2]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}

		//Points 600
						else if(p2c_points==600) {	
							//runs if the points inputed by the user is 600
							while(points[p2c_category][3]!=0) {
								//keeps running until the points selected is equal to 0
								int k=17;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k); 
								//prints the answer
								System.out.println(playerTwo + " Choose the corresponding alpahbet:");
								//prompt user
								p2answer=in.next();
								//gets input from user
								while(!p2answer.equals("a") && !p2answer.equals("A") && !p2answer.equals("b") && !p2answer.equals("B") && !p2answer.equals("c") && !p2answer.equals("C") && !p2answer.equals("d") && !p2answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerTwo + " Choose the corresponding alpahbet:");
									//prompt user again
									p2answer=in.next();
									//gets input from user again
								}
								if (p2answer.equals("d") || p2answer.equals("D")) {
									//runs if the answer inputed by the user is d or D
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p2points= p2points+p2c_points;
									//calculates the points
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p2c_category][3]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}
						
		//Points 800
						else if(p2c_points==800) {
							//runs if the points inputed by the user is 800
							while(points[p2c_category][4]!=0) {
								//keeps running until the points selected is equal to 0
								int k=18;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k); 
								//prints the answer
								System.out.println(playerTwo + " Choose the corresponding alpahbet:");
								//prompt user
								p2answer=in.next();
								//gets input from user
								while(!p2answer.equals("a") && !p2answer.equals("A") && !p2answer.equals("b") && !p2answer.equals("B") && !p2answer.equals("c") && !p2answer.equals("C") && !p2answer.equals("d") && !p2answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerTwo + " Choose the corresponding alpahbet:");
									//prompt user again
									p2answer=in.next();
									//gets input from user again
								}
								if (p2answer.equals("c") || p2answer.equals("C")) {
									//runs if the answer inputed by the user is c or C
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p2points= p2points+p2c_points;
									//calculates the points
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p2c_category][4]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}
						
		//Points 1000
						else if(p2c_points==1000) {
							//runs if the points inputed by the user is 1000
							while(points[p2c_category][5]!=0) {
								//keeps running until the points selected is equal to 0
								int k=19;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k); 
								//prints the answer
								System.out.println(playerTwo + " Choose the corresponding alpahbet:");
								//prompt user
								p2answer=in.next();
								//gets input from user
								while(!p2answer.equals("a") && !p2answer.equals("A") && !p2answer.equals("b") && !p2answer.equals("B") && !p2answer.equals("c") && !p2answer.equals("C") && !p2answer.equals("d") && !p2answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerTwo + " Choose the corresponding alpahbet:");
									//prompt user again
									p2answer=in.next();
									//gets input from user again
								}
								if (p2answer.equals("a") || p2answer.equals("A")) {
									//runs if the answer inputed by the user is a or A
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p2points= p2points+p2c_points;
									//calculates the points
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p2c_category][5]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}

					}

	//Category 4 Computer(5) For Player Two	
					if(p2c_category==4) {
						//runs if the category inputed by the user is Computer(5)
		//Points 200
						if(p2c_points==200) {
							//runs if the points inputed by the user is 200
							while(points[p2c_category][1]!=0) {
								//keeps running until the points selected is equal to 0
								int k=20;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k); 
								//prints the answer
								System.out.println(playerTwo + " Choose the corresponding alpahbet:");
								//prompt user
								p2answer=in.next();
								//gets input from user
								while(!p2answer.equals("a") && !p2answer.equals("A") && !p2answer.equals("b") && !p2answer.equals("B") && !p2answer.equals("c") && !p2answer.equals("C") && !p2answer.equals("d") && !p2answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerTwo + " Choose the corresponding alpahbet:");
									//prompt user again
									p2answer=in.next();
									//gets input from user again
								}
								if (p2answer.equals("c") || p2answer.equals("C")) {
									//runs if the answer inputed by the user is c or C
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p2points= p2points+p2c_points;
									//calculates the points
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p2c_category][1]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}
						
		//Points 400
						else if(p2c_points==400) {
							//runs if the points inputed by the user is 400
							while(points[p2c_category][2]!=0) {
								//keeps running until the points selected is equal to 0
								int k=21;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k); 
								//prints the answer
								System.out.println(playerTwo + " Choose the corresponding alpahbet:");
								//prompt user
								p2answer=in.next();
								//gets input from user
								while(!p2answer.equals("a") && !p2answer.equals("A") && !p2answer.equals("b") && !p2answer.equals("B") && !p2answer.equals("c") && !p2answer.equals("C") && !p2answer.equals("d") && !p2answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerTwo + " Choose the corresponding alpahbet:");
									//prompt user again
									p2answer=in.next();
									//gets input from user again
								}
								if (p2answer.equals("b") || p2answer.equals("B")) {
									//runs if the answer inputed by the user is b or B
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p2points= p2points+p2c_points;
									//calculates the points
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p2c_category][2]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}
						
		//Points 600
						else if(p2c_points==600) {
							//runs if the points inputed by the user is 600
							while(points[p2c_category][3]!=0) {
								//keeps running until the points selected is equal to 0
								int k=22;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k); 
								//prints the answer
								System.out.println(playerTwo + " Choose the corresponding alpahbet:");
								//prompt user
								p2answer=in.next();
								//gets input from user
								while(!p2answer.equals("a") && !p2answer.equals("A") && !p2answer.equals("b") && !p2answer.equals("B") && !p2answer.equals("c") && !p2answer.equals("C") && !p2answer.equals("d") && !p2answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerTwo + " Choose the corresponding alpahbet:");
									//prompt user again
									p2answer=in.next();
									//gets input from user again
								}
								if (p2answer.equals("a") || p2answer.equals("A")) {
									//runs if the answer inputed by the user is a or A
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p2points= p2points+p2c_points;
									//calculates the points
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p2c_category][3]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}
						
		//Points 800
						else if(p2c_points==800) {
							//runs if the points inputed by the user is 800
							while(points[p2c_category][4]!=0) {
								//keeps running until the points selected is equal to 0
								int k=23;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k); 
								//prints the answer
								System.out.println(playerTwo + " Choose the corresponding alpahbet:");
								//prompt user
								p2answer=in.next();
								//gets input from user
								while(!p2answer.equals("a") && !p2answer.equals("A") && !p2answer.equals("b") && !p2answer.equals("B") && !p2answer.equals("c") && !p2answer.equals("C") && !p2answer.equals("d") && !p2answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerTwo + " Choose the corresponding alpahbet:");
									//prompt user again
									p2answer=in.next();
									//gets input from user again
								}
								if (p2answer.equals("d") || p2answer.equals("D")) {
									//runs if the answer inputed by the user is d or D
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p2points= p2points+p2c_points;
									//calculates the points
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p2c_category][4]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}
						
		//Points 1000
						else if(p2c_points==1000) {
							//runs if the points inputed by the user is 1000
							while(points[p2c_category][5]!=0) {
								//keeps running until the points selected is equal to 0
								int k=24;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k); 
								//prints the answer
								System.out.println(playerTwo + " Choose the corresponding alpahbet:");
								//prompt user
								p2answer=in.next();
								//gets input from user
								while(!p2answer.equals("a") && !p2answer.equals("A") && !p2answer.equals("b") && !p2answer.equals("B") && !p2answer.equals("c") && !p2answer.equals("C") && !p2answer.equals("d") && !p2answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerTwo + " Choose the corresponding alpahbet:");
									//prompt user again
									p2answer=in.next();
									//gets input from user again
								}
								if (p2answer.equals("a") || p2answer.equals("A")) {
									//runs if the answer inputed by the user is a or A
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p2points= p2points+p2c_points;
									//calculates the points
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p2c_category][5]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}
					}

	//Category 5 Sports(6) For Player Two	
					if(p2c_category==5) {
						//runs if the category inputed by the user is Sports(6)
		//Points 200
						if(p2c_points==200) {
							//runs if the points inputed by the user is 200
							while(points[p2c_category][1]!=0) {
								//keeps running until the points selected is equal to 0
								int k=25;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k); 
								//prints the answer
								System.out.println(playerTwo + " Choose the corresponding alpahbet:");
								//prompt user
								p2answer=in.next();
								//gets input from user
								while(!p2answer.equals("a") && !p2answer.equals("A") && !p2answer.equals("b") && !p2answer.equals("B") && !p2answer.equals("c") && !p2answer.equals("C") && !p2answer.equals("d") && !p2answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerTwo + " Choose the corresponding alpahbet:");
									//prompt user again
									p2answer=in.next();
									//gets input from user again
								}
								if (p2answer.equals("d") || p2answer.equals("D")) {
									//runs if the answer inputed by the user is d or D
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p2points= p2points+p2c_points;
									//calculates the points
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p2c_category][1]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}
						
		//Points 400
						else if(p2c_points==400) {
							//runs if the points inputed by the user is 400
							while(points[p2c_category][2]!=0) {
								//keeps running until the points selected is equal to 0
								int k=26;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k); 
								//prints the answer
								System.out.println(playerTwo + " Choose the corresponding alpahbet:");
								//prompt user
								p2answer=in.next();
								//gets input from user
								while(!p2answer.equals("a") && !p2answer.equals("A") && !p2answer.equals("b") && !p2answer.equals("B") && !p2answer.equals("c") && !p2answer.equals("C") && !p2answer.equals("d") && !p2answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerTwo + " Choose the corresponding alpahbet:");
									//prompt user again
									p2answer=in.next();
									//gets input from user again
								}
								if (p2answer.equals("c") || p2answer.equals("C")) {
									//runs if the answer inputed by the user is c or C
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p2points= p2points+p2c_points;
									//calculates the points
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p2c_category][2]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}
						
		//Points 600
						else if(p2c_points==600) {
							//runs if the points inputed by the user is 600
							while(points[p2c_category][3]!=0) {
								//keeps running until the points selected is equal to 0
								int k=27;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k); 
								//prints the answer
								System.out.println(playerTwo + " Choose the corresponding alpahbet:");
								//prompt user
								p2answer=in.next();
								//gets input from user
								while(!p2answer.equals("a") && !p2answer.equals("A") && !p2answer.equals("b") && !p2answer.equals("B") && !p2answer.equals("c") && !p2answer.equals("C") && !p2answer.equals("d") && !p2answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerTwo + " Choose the corresponding alpahbet:");
									//prompt user again
									p2answer=in.next();
									//gets input from user again
								}
								if (p2answer.equals("c") || p2answer.equals("C")) {
									//runs if the answer inputed by the user is c or C
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p2points= p2points+p2c_points;
									//calculates the points
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p2c_category][3]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}
						
		//Points 800
						else if(p2c_points==800) {
							//runs if the points inputed by the user is 800
							while(points[p2c_category][4]!=0) {
								//keeps running until the points selected is equal to 0
								int k=28;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k); 
								//prints the answer
								System.out.println(playerTwo + " Choose the corresponding alpahbet:");
								//prompt user
								p2answer=in.next();
								//gets input from user
								while(!p2answer.equals("a") && !p2answer.equals("A") && !p2answer.equals("b") && !p2answer.equals("B") && !p2answer.equals("c") && !p2answer.equals("C") && !p2answer.equals("d") && !p2answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerTwo + " Choose the corresponding alpahbet:");
									//prompt user again
									p2answer=in.next();
									//gets input from user again
								}
								if (p2answer.equals("b") || p2answer.equals("B")) {
									//runs if the answer inputed by the user is b or B
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p2points= p2points+p2c_points;
									//calculates the points
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p2c_category][4]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}
						
		//Points 1000
						else if(p2c_points==1000) {
							//runs if the points inputed by the user is 1000
							while(points[p2c_category][5]!=0) {
								//keeps running until the points selected is equal to 0
								int k=29;
								//Initializes the variable
								questions(k);
								//prints the question
								answers(k); 
								//prints the answer
								System.out.println(playerTwo + " Choose the corresponding alpahbet:");
								//prompt user
								p2answer=in.next();
								//gets input from user
								while(!p2answer.equals("a") && !p2answer.equals("A") && !p2answer.equals("b") && !p2answer.equals("B") && !p2answer.equals("c") && !p2answer.equals("C") && !p2answer.equals("d") && !p2answer.equals("D")) {
									//keeps running until a valid input for the answer is not placed
									System.out.println("--------------------------------------------------");
									System.out.println("There is an Error put the corresponding alpahbet.");
									//shows an error
									System.out.println(playerTwo + " Choose the corresponding alpahbet:");
									//prompt user again
									p2answer=in.next();
									//gets input from user again
								}
								if (p2answer.equals("b") || p2answer.equals("B")) {
									//runs if the answer inputed by the user is b or B
									System.out.println("_____________________________________");
									System.out.println("You are correct! :)");
									System.out.println("-------------------------------------");
									p2points= p2points+p2c_points;
									//calculates the points
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								else {
									System.out.println("_____________________________________");
									System.out.println("You are wrong :(");
									System.out.println("-------------------------------------");
									System.out.print("The correct answer was: ");
									correctanswer(k);
									//prints the correct answer
									System.out.println("-------------------------------------");
									System.out.println("Your points are: " + p2points);
									//prints the points
									System.out.println("_____________________________________");
								}
								points[p2c_category][5]=0;
								//makes the points selected to 0 so it can't be chosen again
							}
						}
					}
				}
			}
		}
		System.out.println("_____________________________________");
		System.out.println("_____________________________________");
		System.out.println("The Game is Over");
		System.out.println("_____________________________________");
		System.out.println("_____________________________________");
		System.out.println();
		if(p1points>p2points) {
			//runs if playerOne points is greater than playerTwo points
			System.out.println("_____________________________________");
			System.out.println(playerOne + " has won the game by " + (p1points-p2points) + " points.");
			System.out.println("_____________________________________");
		}
		else if(p1points==p2points){
			//runs if playerOne points same as playerTwo points
			System.out.println("_____________________________________");
			System.out.println(" The game was tie with " + p1points + " points.");
			System.out.println("_____________________________________");
		}
		else {
			//runs if playerOne points is less than playerTwo points
			System.out.println("_____________________________________");
			System.out.println(playerTwo + " has won the game by " + (p2points-p1points) + " points.");
			System.out.println("_____________________________________");
		}
		System.out.println();
		//adds a line
		System.out.println("_____________________________________");
		System.out.println("Thank you for playing the game. Hope you enjoyed it!");
		System.out.println("Made by: Virendra Jethra");
		System.out.println("_____________________________________");
	}

}
