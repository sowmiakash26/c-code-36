#include<stdio.h>
#include<stdbool.h>
bool is prime(int num) {
if(num==1) {
return false;
}
if(num=2)
{
 return true;
 }
 if(num%2==0) {
 return false;
 }

 for(int i=3; i<= sqrt(num); i+=2) {
 if(num%2 == 0) {
  return false;
  }
  }
  return true;

  }

bool ispalindrome(int num) {
int org=num;
int rev=0;
while(num>0){
int digit = num%10;
rev = rev*10 + digit;
num/=10;
}
return org == rev;
}
