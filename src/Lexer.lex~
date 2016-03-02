import java_cup.runtime.*;

%%
%class Lexer
%unicode
%cup
%line
%column

%{
   private Symbol symbol(int type){
       return new Symbol(type, yyline, yycolumn);
   }
   
   private Symbol symbol(int type, Object value){
       return new Symbol(type, yyline, yycolumn, value);
   }
%}


Letter = [a-zA-Z]
Digit = [0-9]
IdChar = {Letter} | {Digit} | "_"
Identifier = {Letter}{IdChar}*

