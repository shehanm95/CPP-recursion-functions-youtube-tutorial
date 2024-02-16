you can get all the c++ recursion questions and answers in here,

my tutorial vedio >> https://www.youtube.com/watch?v=P129tsrdWSI


========C++ Recursion functions.=====



1. Write a c++ program to find factorial of first 5 numbers without using loops;
   
#include <iostream>
using namespace std;
int factorial(int num){
 if(num == 0){
 return 1;
 }
 return num * factorial(num-1);
}
int main() {
 cout << factorial(5);
 return 0;
}
2==================================//===========================
write 5 times hello world without loop


#include <iostream>
using namespace std;
int hello(int num){
 if(num == 0){
 return 0;
 }
 cout << "hello" << endl;
 return hello(num-1);
}
int main() {
 hello(5);
 return 0;
}
3==================================//===========================
print 1 to N number without loop;
#include <iostream>
using namespace std;
int rec(int num){
 if(num == 0){
 return 0;
 }
 cout << 1 + rec(num-1);
 return num;
}
int main() {
 rec(7);
 return 0;
}
4==================================//===========================
print N to 1 number without loop;



#include <iostream>
using namespace std;
int rec(int num){
 if(num == 0){
 return 0;
 }
 cout << num;
 return rec(num -1);
 
}
int main() {
 rec(7);
 return 0;
}



5==================================//===========================
reverse of a word;
#include <iostream>
using namespace std;
int rec(string word , int index){
 if(index == 1){
 cout << word[0];
 return 1;
 }
 
 cout << word[index-1];
 return rec(word , index-1);
}
int main() {
 string word = "OLLLOO";
 int size = word.length();
 rec(word, size);
 return 0;
}
6==================================//===========================
avarage of array
#include <iostream>
using namespace std;
float avarage(float nums[] ,int index, int size){
 int sum;
 if(index == 1){
 return nums[0];
 }
 sum = nums[index - 1] + avarage(nums ,index - 1,size);
 if(index == size){
 return sum / size;
 }
 return sum;
}
int main() {
 float nums[4] = {2,3,5,2};
 int size = sizeof(nums)/sizeof(nums[0]);
 cout << avarage(nums ,size , size );
 return 0;
}



7==================================//============================



fibonaci number calculation with recursion;
#include <iostream>
using namespace std;
int fib(int n){
 if(n == 1){
 return 1;
 }
 else if(n == 0){
 return 0;
 }
 return fib(n-1) + fib(n-2);
}
int main() {
 for(int i =0; i < 10 ; i++)
 cout << "fib(" << i << ") = " << fib(i) << endl;
 return 0;
}
