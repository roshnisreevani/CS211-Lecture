Name: Angela Natividad
Major: Computer Science
Favorite CS Topic: Strings
Challenging Topic: Pointers

int nthFibonacci(int n) {
    if(n <=1){
        return n;
    }
    int current = 0;
    int previous1 = 1;
    int previous2 = 0;
    
    for(int i = 2; i <=n; i++){
        current = previous1 + previous2;
        
        previous2 = previous1;
        previous1 = current;
    }
    return current;
}

//line 12 error no semicolon. add semicolon after return
//wrong output. return call to function
