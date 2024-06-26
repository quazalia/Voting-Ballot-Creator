[Presentation's link](https://docs.google.com/presentation/d/1mf7WAnRDQ06oL0pFJbInKFJ5Givn7sVeHwWlM3w-LbU/edit?usp=sharing)
# Voting Ballot Creator

## Description
The Voting Ballot Creator is a console-based application designed to manage a list of candidates and their votes in a ballot. It allows users to add, modify, and remove candidates, display the list of candidates, and save/load the ballot data from a file. This application is useful for small organizations or groups conducting informal elections or polls.

## Objectives
- **Candidate Management**: Provide functions to add, update, and remove candidates from the ballot.
- **Vote Tracking**: Allow tracking of votes for each candidate.
- **Data Persistence**: Enable saving the ballot data to a file and loading it from a file.
- **User-Friendly Interface**: Offer a simple console-based interface for easy interaction.
- **Sorting and Display**: Display candidates sorted by the number of votes.

## Design Decisions

### Data Storage
- **Candidates**: Stored in a `vector` to allow dynamic resizing and efficient iteration.

### Candidate Representation
- **Struct**: A `struct` is used for the Candidate entity to group related attributes (`name` and `votes`) together.

### File I/O
- **File Streams**: Candidates can be saved to and loaded from a file using standard file stream operations (`ifstream` and `ofstream`).

### User Interface
- **Command-Line Interface**: A simple command-line interface is provided for user interaction.

## Data Structures and Algorithms

### Data Structures
- **Vector**: Used to store the collection of candidates.
- **Struct Candidate**: Defines the attributes of a candidate (`name` and `votes`).

### Functions
- **Add Candidate**: Appends a new candidate to the candidates vector.
- **Update Candidate**: Iterates through the candidates vector to find a candidate by their name and updates their details.
- **Remove Candidate**: Iterates through the candidates vector to find a candidate by their name and removes them.
- **Display Candidates**: Iterates through the candidates vector, sorts by votes, and prints each candidate's details.
- **Save to File**: Writes each candidate's details to a file, one candidate per line.
- **Load from File**: Reads each line from a file, parses the candidate details, and adds the candidate to the candidates vector.

## Screenshots
1. Main Menu <br>
  ![main menu](https://github.com/quazalia/Voting-Ballot-Creator/assets/148089170/c245254f-236b-450c-be67-1110b1b282e9)<br>
***
## How to Use the Software

### Installation and Setup
1. Ensure you have a C++ compiler installed.
2. Save the provided code into a file, e.g., `voting_ballot.cpp`.

### Compilation
1. Open a terminal or command prompt.
2. Navigate to the directory containing `voting_ballot.cpp`.
3. Compile the code using a C++ compiler, e.g., 
   ```sh
   `g++ -o voting_ballot voting_ballot.cpp`.
   
### Execution
   Run the compiled program, e.g.,/voting_ballot
Follow the on-screen instructions to interact with the Voting Ballot Management System.Ensure that ballot.txt exists in the same directory to load the ballot data on start. The file will also be used to save the ballot data.

### Features

**1. Add Candidate:**  
   Allows the user to input the details of a new candidate and add them to the ballot.

**2. Update Candidate:**  
   Enables the user to update the details (name and votes) of an existing candidate by providing the candidate's name and the new details.

**3. Remove Candidate:**  
   Provides the functionality to remove a candidate from the ballot by specifying the candidate's name.

**4. Display Candidates:**  
   Displays the list of all candidates in the ballot, sorted by the number of votes received.

**5. Save Ballot to File:**  
   Saves the current state of the ballot, including all candidates and their respective votes, to a file named "ballot.txt".

**6. Load Ballot from File:**  
   Loads the previously saved ballot from the "ballot.txt" file if it exists. This feature clears any existing candidates in memory and replaces them with the ones loaded from the file.

