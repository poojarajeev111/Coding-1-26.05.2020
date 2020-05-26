
#include <bits/stdc++.h> 

using namespace std; 

void cntArray(int A[], int N) 
{ 


    int result = 0; 

  

    for (int i = 0; i < N; i++) { 

 
        result++; 

        int current_value = A[i]; 

  

        for (int j = i + 1; j < N; j++) {

     

            if (A[j] == current_value) { 

                result++; 

            } 

        } 

    } 

    cout << result << endl; 
}  

int main() 
{ 

    int A[] = { 1, 5, 6, 1, 9, 

                5, 8, 10, 8, 9 }; 

    int N = sizeof(A) / sizeof(int); 

  

    cntArray(A, N); 

  

    return 0; 
} 
