Name: Krishna Harshini Duggirala
Major: Data Science
Favotite CS topic: Decision trees
Challenging toic: Pointers

//memoization coding problem solution
int nthFibonacci(int n) {
    
    if (n <= 1){
        return n;
    }
    int current = 0; 
    int previous1 = 1;
    int previous2 = 0;
    
    for(int i = 2; i <= n; i++){
        current = previous1 + previous2;
        
        previous2 = previous1;
        previous1 = current;
    }
    
    return current;
    
}