# -Quiz07-q2.cpp-
#include stdio.h>

#include string.h>


int main()

{
    char palabra[20];
    
    int i, j;
    
    int isPalindromo = 1;
    
    printf("Escribe una cadena: ");
    
    fflush(stdout);
    
    gets(palabra);
    
    j=strlen(palabra)-1;
    
    for(i=0; i<strlen(palabra)/2; i++, j--) {
    
        printf("Comprobando %c==%c\n", *(palabra+i), *(palabra+j));
        
        if (*(palabra+i)!=*(palabra+j)) {
        
            isPalindromo = 0;
            
            break;
            
        }
    }
    if (isPalindromo)
    
        printf("\nEs un palíndrimo.\n");
        
    else
    
        printf("\nNo es un palíndrimo.\n");
        

    return (0);
}

    
    
