Download link :https://programming.engineering/product/netflix/

# Netflix
Netflix
Write a program that can be used to gather statistical data about the number of hours college students spend watching streaming videos on Netflix in one month.

Assignment Instructions:

MAIN FUNCTION:

Ask the user how many students were surveyed.

Call a function called makeArray to define an array of integers with the number of elements equal to the number of students surveyed.

Call a function called getStudentData to allow the user to enter the number of hours each student spent watching Netflix into the array.

Call a function called getAverage to calculate and display the average of the hours entered.

Call a function called selectionSort to sort the hours in ascending order. This function is provided for you.

Call a function called printArray to print out the hours in the array.

Print out the Average

makeArray Function

Define an array of integers with the number of elements equal to the number of students surveyed. The function will accept as arguments the following: An integer that indicates the number of elements in the array.

The array should be dynamically allocated.
Use pointer notation instead of array notation in this function.


getStudentData Function

Allow the user to enter the number of hours each student watched Netflix into the array. The function will accept as arguments the following:

An array of integers

An integer that indicates the number of elements in the array.

Input Validation: Do not accept negative numbers for input.
Use pointer notation instead of array notation in this function.

printArray Function

This function should print out the text “Number of hours each student watched Netflix in ascending order: “. Then, the function should print out each element in the array with a space between each element. The function will accept as arguments the following:

An array of integers

An integer that indicates the number of elements in the array.

Use pointer notation instead of array notation in this function.

getAverage Function

The average of a set of values is calculated by adding all the values and then dividing the sum by the number of values in the set. Write a function that accepts as arguments the following:

An array of integers

An integer that indicates the number of elements in the array.

The function should determine the average of the array. The average is the value the function should return.
Use pointer notation instead of array notation in this function.

selectionSort Function:

/**************************************************

* Function selectionSort *

* This function performs the selection sort *

* algorithm on array, sorting it into ascending *

* order. The parameter size holds the number of *

* elements in the array. *

**************************************************/

void selectionSort(int *array, int size)

{

int startScan, minIndex, minValue;

for (startScan = 0; startScan < (size – 1); startScan++)

{

minIndex = startScan;

minValue = *(array+startScan);

for(int index = startScan + 1; index < size; index++)

{

if (*(array+index) < minValue)

{

minValue = *(array+index);

minIndex = index;

}

}

*(array+minIndex) = *(array+startScan);

*(array+startScan) = minValue;

}

}
