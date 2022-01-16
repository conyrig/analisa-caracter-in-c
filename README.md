# analisa-caracter-em-c
Programa em C que analisa caractéres

#include <stdio.h>

void analisa_caracter (char ch) {
    
    if(ch>='0' && ch<='9'){
        printf ("Um numero\n");
    }   
    if(ch>='a' && ch<='z'){
        if(ch=='a' || ch=='e' || ch=='i' || ch=='o' || ch=='u'){
            printf ("Uma vogal minuscula\n");
        } else{
        printf ("Uma letra minuscula\n");
        }
    }
    if(ch>='A' && ch<='Z'){
        printf ("Uma letra maiuscula\n");
    }
}


void main () {
   
    char    ch;
    
    while (1) {
        printf ("Escreva um caracter %% para sair: ");
        scanf (" %c", &ch);
        if (ch == '%')
            return;
        analisa_caracter (ch);  
    }
}
