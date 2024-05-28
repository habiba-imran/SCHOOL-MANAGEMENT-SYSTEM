SCHOOL MANAGEMENT PROGRAM

This is a simple school management program written in C++. The program allows users to perform various operations on student data, including entering new records, searching, updating, deleting, and displaying all student records. The data is stored in a text file to ensure persistence between sessions.

FEATURES

1. Enter Data: Add new student records to the system.
2. Search Data: Search for a student record by roll number.
3. Update Data: Update the details of an existing student.
4. Delete Data: Delete a student record by roll number or delete all records.
5. Display All Data: Display all student records.

FILE STRUCTURE

- `main.cpp`: Contains the main code for the program.
- `students.txt`: The file where student records are stored.


PREREQUISITES

To compile and run this program, you need:
- A C++ compiler (e.g., g++, clang++)
- An IDE or text editor (e.g., Visual Studio, VS Code, Code::Blocks)
- Basic understanding of C++ and file I/O

INSTALLATION

1. CLONE THE REPOSITORY

    ```bash
    git clone https://github.com/yourusername/school-management-program.git
    cd school-management-program
    ```

2. OPEN THE PROJECT IN VISUAL STUDIO

    - Open Visual Studio.
    - Go to `File` > `Open` > `Project/Solution`.
    - Navigate to the cloned directory and select `main.cpp`.

3. COMPILE AND RUN

    - Press `Ctrl + F5` to compile and run the program in Visual Studio.

USAGE

1. RUNNING THE PROGRAM

    Run the program using your preferred IDE or compile it manually using the terminal:

    ```bash
    g++ main.cpp -o school_management
    ./school_management
    ```

2. INTERACTING WITH THE PROGRAM

    The program will display a menu with the following options:

    - Press `1` to enter new student data.
    - Press `2` to search for a student by roll number.
    - Press `3` to update an existing student's data.
    - Press `4` to delete a student record or all records.
    - Press `5` to display all student records.
    - Press `6` to exit the program.

3. ADDING STUDENT DATA

    When you select the option to add student data, you will be prompted to enter details such as first name, roll number, department, semester, and contact number.

4. SEARCHING FOR A STUDENT

    Enter the roll number of the student you want to search for. If the student is found, their details will be displayed.

5. UPDATING STUDENT DATA

    Enter the roll number of the student whose data you want to update. The program will display the current data and prompt you to enter new details.

6. DELETING RECORDS

    You can delete all records or delete a specific record by entering the student's roll number.

7. DISPLAYING ALL RECORDS

    This option displays the details of all students stored in the system.

 CODE OVERVIEW

DATA STRUCTURE

- `struct Student`: Defines the structure of a student record with attributes like first name, roll number, department, semester, and contact number.
- `students`: An array of `Student` structures to hold all student records.
- `totalStudents`: Keeps track of the number of student records.

FUNCTIONS

- `void saveToFile()`: Saves all student records to `students.txt`.
- `void loadFromFile()`: Loads student records from `students.txt` at the start of the program.
- `void enter()`: Prompts the user to enter new student data.
- `void search()`: Searches for a student by roll number.
- `void update()`: Updates the details of an existing student.
- `void delete_record()`: Deletes a student record or all records.
- `void displayAll()`: Displays all student records.

MAIN FUNCTION

The `main()` function initializes the program, loads existing records from the file, and presents a menu to the user for various operations.

LICENSE

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

 ACKNOWLEDGMENTS

This program is a basic example of file I/O and struct usage in C++. It can be expanded with additional features such as input validation, error handling, and a more user-friendly interface.
