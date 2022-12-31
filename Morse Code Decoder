// Author: Muhammad Asad Naveed
// U.No.: 3035957848
// Assignment 2 Question 3
// Description : In this problem, you are asked to write a C++ program that takes in a sequence of morse code and decodes it to text characters.

#include <iostream>
#include <string>

/**
 * A s code decoder.
 */

using namespace std;

// IMPORTANT:  Do NOT change any of the function headers
//             It means that you will need to use the function headers as is
//             You may add other functions wherever appropriate


/**
 * Decode the s code `s` and return the text character
 */



string Morsetoletter(string morse)    //keys for all the possible decoding
{

        if(morse == "._")
        {return "A";}
        else if(morse == "_...")
        {return "B";}
        else if(morse == "_._.")
        {return "C";}
        else if(morse == "_..")
        {return "D";}
        else if(morse == ".")
        {return "E";}
        else if(morse == ".._.")
        {return "F";}
        else if(morse == "__.")
        {return "G";}
        else if(morse == "....")
        {return "H";}
        else if(morse == "..")
        {return "I";}
        else if(morse == ".___")
        {return "J";}
        else if(morse == "_._")
        {return "K";}
        else if(morse == "._..")
        {return "L";}
        else if(morse == "__")
        {return "M";}
        else if(morse == "_.")
        {return "N";}
        else if(morse == "___")
        {return "O";}
        else if(morse == ".__.")
        {return "P";}
        else if(morse == "__._")
        {return "Q";}
        else if(morse == "._.")
        {return "R";}
        else if(morse == "...")
        {return "S";}
        else if(morse == "_")
        {return "T";}
        else if(morse == ".._")
        {return "U";}
        else if(morse == "..._")
        {return "V";}
        else if(morse == ".__")
        {return "W";}
        else if(morse == "_.._")
        {return "X";}
        else if(morse == "_.__")
        {return "Y";}
        else if(morse == "__..")
        {return "Z";}

        else
        {
            return " ";
        }

    return 0;    


}  
/**
 * Decode the morse code `s` and return the text character
 */      
string morseCodeToText(string s)              // iterates through the input and call the morse to letter function accordingly
{
	int node = 0;
	string temp;
    string see;
    string text="";
    for(int i = 0;i<=s.length();i++)
    {
        if(s[i]=='|')                         //if | is found is looks the characters behind it
        {

            see = s.substr(node,i-node);
            text+=Morsetoletter(see);
            node = i+1;
        
        }
        if(i==s.length()-1)
        {
            see = s.substr(node,i+1-node);
            text+=Morsetoletter(see);
            node = i+1;
        }

    }

	

	return text;

	
}

///////////////////////////////////////////////////////Main Function//////////////////////////////////////////////////////////
int main()                             
{
	string s;
	cin >> s;
	cout << morseCodeToText(s) << '\n';      //displays the output
    return 0;
}

