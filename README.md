%{
#include<stdio.h>
%}
if|else|while|for|switch|return|break|continue {printf("valid keyword. ") ;}
[0-9]+ {printf(" Other than keyword and number "(:}
%%
void () 
{ printf(" Enter the input string:") ;
yylex() :
}
int yywrap() 
{
 return 1;
 }
