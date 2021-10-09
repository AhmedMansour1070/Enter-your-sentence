#include <iostream>
using namespace std;
#include <string.h>
#include <string>
#include <ctype.h>



string shuffle(string sentence);
string reverse(string sentence);
string strcpy1(string The_sentence);
string strcpy2(string sentance);
string middle(string sentence);
int add(string sentence);
void order(string sentence);
string UPPER(string sentence);

int main() {
   string sentence;
   cout<<"Enter your sentence"<<endl;
   getline(cin,sentence);
   if(strcpy1(sentence)=="print"||strcpy1(sentence)=="Print")
   cout<<strcpy2(sentence);
   else if(strcpy1(sentence)=="reverse"||strcpy1(sentence)=="Reverse")
   cout<<reverse(sentence);
   else if(strcpy1(sentence)=="shuffle"||strcpy1(sentence)=="Shuffle")
   cout<<shuffle(sentence);
   else if(strcpy1(sentence)=="add"||strcpy1(sentence)=="Add")
   cout<<add(sentence);
   else if(strcpy1(sentence)=="order"||strcpy1(sentence)=="Order")
   order(sentence);
   else if(strcpy1(sentence)=="upper"||strcpy1(sentence)=="upper")
   cout<<UPPER(sentence);
    return 0;
}


string strcpy1(string sentence){
    int i;
    string command;
    for(i = 0;sentence[i] != ' '; i++)
    {
        command = command + sentence[i];
    }
    return command;
}


string strcpy2(string sentence){
    int k, l ,i;
    string rest_of_the_sentence;
    for(l = 0;sentence[l] != '\0'; l++);
    //l = sentence.length();
    for(i = 0;sentence[i] != ' '; i++);
    for(k = i+1; k <= l; k++)
    {
        rest_of_the_sentence = rest_of_the_sentence + sentence[k];
    }
    return rest_of_the_sentence;
}


string reverse(string sentence){
    strcpy2(sentence);
    int k, l ,i;
    string rest_of_the_sentence;
    for(l = 0;sentence[l] != '\0'; l++);
    //l = sentence.length();
    for(i = 0;sentence[i] != ' '; i++);
    for(k = l; k >= i+1; k--)
    {
        rest_of_the_sentence = rest_of_the_sentence + sentence[k];
    }
    return rest_of_the_sentence;
}


string shuffle(string sentence){
    strcpy2(sentence);
    string shuffled_sentence;
    int i,l,k;
    for(l = 0;sentence[l] != '\0'; l++);
    for(i = 0;sentence[i] != ' '; i++);
    for(k = i+1; k <= l;k += 2)
    {
        shuffled_sentence =shuffled_sentence + sentence[k+1] + sentence[k];
    }
    return shuffled_sentence;
}




int add(string sentence){
    string the_two_num,firtst_num;
    the_two_num = strcpy2(sentence);
    int i, int_n1;
    for(i = 0;the_two_num[i] != ' '; i++){
        firtst_num = firtst_num + the_two_num[i];
    }
    int_n1 = stoi(firtst_num);
    int v,k,l;
    int int_n2;
    string second_num;
    for(l = 0;the_two_num[l] != '\0'; l++);
    for(v = 0;the_two_num[v] != ' '; v++);
    for(k = v+1; k <= l; k++)
    {
        second_num = second_num + the_two_num[k];
    }
    int_n2 = stoi(second_num);
    return int_n1+int_n2;
}


void order(string sentence){
    
    string two_words,first_word;
    two_words = strcpy2(sentence);
    int i;
    for(i = 0;two_words[i] != ' '; i++){
        first_word = first_word + two_words[i];
    }
    int v,k,l;
    string second_word;
    for(l = 0;two_words[l] != '\0'; l++);
    for(v = 0;two_words[v] != ' '; v++);
    for(k = v+1; k <= l; k++)
    {
        second_word = second_word + two_words[k];
    }
    if(first_word<second_word)
    cout<<first_word<<" "<<second_word;
    else
    cout<<second_word<<" "<<first_word;
}


string UPPER(string sentence){ 
    string sentence_new;
    string s;
    sentence_new = strcpy2(sentence);
    for(int i = 0 ; i+1 <= sentence_new.length();i++){
        s += toupper(sentence_new[i]);
    }
    return s;
}
