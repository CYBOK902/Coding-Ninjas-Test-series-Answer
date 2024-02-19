# Coding-Ninjas-Test-series-Answer
#Coding Ninjas Test series Answer #CodingNinjas #Test series #answer

Problem statement
A binary array is an array consisting of only 0s and 1s.

You are given a binary array "arr" of size ‘N’. Your task is to sort the given array and return this array after sorting.

Detailed explanation ( Input/output format, Notes, Images )
Sample Input 1 :
2
3 
0 1 0
4
0 0 0 1
Sample Output 1 :
0 0 1
0 0 0 1
Explanation of Sample Input 1 :
Test case 1:
The sorted array is 0 0 1

Test case 2:
The array is already sorted.
Sample Input 2 :
2
1
0
2
1 0
Sample Output 2 :
0
0 1
Explanation of Sample Input 2 :
Test case 1:
The array is already sorted

Test case 2:
The sorted array is 0 1.


>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>////////////Code/////////<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<

#include <vector> 
using namespace std;

vector<int> sortBinaryArray(vector<int> arr, int n) {
	int ind = 0;
	for (int i = 0; i < n; i ++){
		if (arr[i] ==0){
			swap(arr [i], arr[ind]);
			ind++;
		}
	}
	return arr;
}


