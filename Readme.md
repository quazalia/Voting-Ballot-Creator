Voting Ballot Management System
Description:
The Voting Ballot Management System is a console-based application designed to manage a list of candidates and their votes in a ballot. It allows users to add, modify, and remove candidates, display the list of candidates, and save/load the ballot data from a file. This application is useful for small organizations or groups conducting informal elections or polls.
Objectives:
Candidate Management: Provide functions to add, update, and remove candidates from the ballot.
Vote Tracking: Allow tracking of votes for each candidate.
Data Persistence: Enable saving the ballot data to a file and loading it from a file.
User-Friendly Interface: Offer a simple console-based interface for easy interaction.
Sorting and Display: Display candidates sorted by the number of votes.

Design Decisions:
Data Storage: Candidates are stored in a vector to allow dynamic resizing and efficient iteration.
Candidate Representation: A struct is used for the Candidate entity to group related attributes (name and votes) together.
File I/O: Candidates can be saved to and loaded from a file using standard file stream operations (ifstream and ofstream).
User Interface: A simple command-line interface is provided for user interaction.

Data Structures and Algorithms
Data Structures
Vector: Used to store the collection of candidates.
Struct Candidate: Defines the attributes of a candidate (name and votes).
Algorithms
Add Candidate: Appends a new candidate to the candidates vector.
Update Candidate: Iterates through the candidates vector to find a candidate by their name and updates their details.
Remove Candidate: Iterates through the candidates vector to find a candidate by their name and removes them.
Display Candidates: Iterates through the candidates vector, sorts by votes, and prints each candidate's details.
Save to File: Writes each candidate's details to a file, one candidate per line.
Load from File: Reads each line from a file, parses the candidate details, and adds the candidate to the candidates vector.
Screenshots:
1.Main Menu
![Снимок экрана (28)](https://github.com/quazalia/Voting-Ballot-Creator/assets/148089170/5e2111c1-3860-4752-a54a-2508cbdc822f)
How to Use the Software
Installation and Setup:
Ensure you have a C++ compiler installed.
Save the provided code into a file, e.g., voting_ballot.cpp.
Compilation
Open a terminal or command prompt.
Navigate to the directory containing voting_ballot.cpp.
Compile the code using a C++ compiler, e.g., g++ -o voting_ballot voting_ballot.cpp
Execution:
Run the compiled program, e.g.,/voting_ballot
Follow the on-screen instructions to interact with the Voting Ballot Management System.
Ensure that ballot.txt exists in the same directory to load the ballot data on start. The file will also be used to save the ballot data.
