**Third commit**


A code to convert a string to Morse code:
string toMorseCode(string text) {
    map<char, string> morseCode = initializeMorseCodeMap();
    string morseText = "";


for loop :
        for (char& c : text) {
        char upperChar = toupper(c);
        
//Converting letters to uppercase for simplicity
        if (morseCode.find(upperChar) != morseCode.end()) {
            morseText += morseCode[upperChar] + " ";
        }
    }
