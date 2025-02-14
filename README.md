# File-IO
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
