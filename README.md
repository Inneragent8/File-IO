processCSV
Input: string filename (name of the CSV file)
Output: None (but prints processed data)
Algorithm:
Open the CSV file.
If the file fails to open, print an error message and exit.
Read each line from the file.
For each line:
Declare num1, num2, and word.
Call parseLine(line, num1, num2, word) to extract values.
Compute total = num1 + num2.
Call printWordMultipleTimes(total, word).
Close the file and print a completion message.

parseLine
Input: string line, int& num1, int& num2, string& word (variables to store data)
Output: Modifies num1, num2, and word
Algorithm:
Create a stringstream from line.
Extract the first integer (num1) by reading until the first comma.
Extract the second integer (num2) by reading until the second comma.
Extract the remaining word (word).
Store extracted values in num1, num2, and word.

printWordMultipleTimes
Input: int count (number of times to print), string word (word to print)
Output: Prints word count times, separated by spaces
Algorithm:
Use a loop from 0 to count-1:
Print word followed by a space.
Print a newline at the end.n
