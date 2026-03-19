# C-23
#include<iostream.h>
#include<conio.h>

void main()
{
    char str[100];
    int i, vowels = 0, consonants = 0;

    clrscr();

    cout<<"Enter a string: ";
    cin.getline(str, 100);

    for(i = 0; str[i] != '\0'; i++)
    {
        char ch = tolower(str[i]);

        if(ch >= 'a' && ch <= 'z')
        {
            if(ch=='a'||ch=='e'||ch=='i'||ch=='o'||ch=='u')
                vowels++;
            else
                consonants++;
        }
    }

    cout<<"Vowels: "<<vowels<<endl;
    cout<<"Consonants: "<<consonants;

    getch();
}
