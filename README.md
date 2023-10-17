// Predict the output
#include <bits/stdc++.h>
using namespace std;
int main() {
while ('1' < '2')
cout << "In while loop" << endl;
}
OUTPUT : infinite loop

// Predict the output
#include <bits/stdc++.h>
using namespace std;
int main( ) {
int t = 10;
while (t /= 2) {
cout << "Hello" << endl;
}
}
OUTPUT : Hello
Hello
Hello

// Predict the output
#include <bits/stdc++.h>
using namespace std;
int main( ) {
for (int x = 1; x * x <= 10; x++)
cout << "In for loop" << endl;
}
OUTPUT : In for loop
In for loop
In for loop

// Predict the output
#include <bits/stdc++.h>
using namespace std;
int main( ) {
int x = 10, y = 0 ;
while ( x >= y ) {
x-- ;
y++ ;
cout << x << " " << y << endl ;
}
}
OUTPUT : 
9 1
8 2
7 3
6 4
5 5
4 6

// Sum of Even Digits 
#include<iostream>
using namespace std;
int main(){
    int n;
    cout<<"Enter the value of n : ";
    cin>>n;
    int sum=0;
    int lastdigit=0;
    while(n>0){
        lastdigit=n%10;
        if(lastdigit%2==0) sum += lastdigit;
        n /= 10;
    }cout<<sum;
}

// WAP to print the sum of a given number and its reverse.
#include<iostream>
using namespace std;
int main(){
    int n;
    cout<<"Enter a Number : ";
    cin>>n;
    int a=n; // Because the value of n change in loop
    int lastdigit=0;
    int rev=0;
    int sum=0;
    while(n>0){
        rev=rev*10;
        lastdigit=n%10;
        rev=rev+lastdigit;
        n=n/10;
    }
    sum=rev+a;
    cout<<sum;
}

// Print the factorials of first ‘n’ numbers
#include<iostream>
using namespace std;
int main(){
    int n;
    cout<<"Enter the value of n : ";
    cin>>n;
    int product=1;
    for(int i=1;i<=n;i++){
        product *= i;
        cout<<product<<endl;
    }
}

// Print first ‘n’ fibonacci numbers.
#include<iostream>
using namespace std;
int main(){
    int n;
    cout<<"Enter the value of n : ";
    cin>>n;
    int a=1,b=1,sum=0;
    for(int i=1;i<=n-2;i++){
        sum= a+b;
        a=b;
        b=sum;
        cout<<b<<" ";
    }
} 

// Write a program to print out all Armstrong numbers between 1 and 500. If the sum of cubes of each digit of the number is equal to //the number itself, then the number is called an Armstrong number.
#include<iostream>
using namespace std;
int main(){
    for(int i=1;i<=500;i++){
        int x=i;
        int cubeSum=0;
        while(x>0){
            int ld =x%10;
            cubeSum += (ld*ld*ld);
            x /= 10;
        }
        if(i==cubeSum) cout<<cubeSum<<endl;
    }
}
