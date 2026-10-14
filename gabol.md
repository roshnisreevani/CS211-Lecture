Name: Gloria Abolade
Major: Computer Science
Favorite CS Topics: Turtle
Challenging Topic: Everything else
int nthFibonacci(int n) {
	// code here
	if (n <= 1) {
		return n;
	}
	int curr = 0; // stores currnet fibonacci
	// stores past two fibaonnaci sequence
	
	int prev1 = 1;
	int prev2 = 0;
	
	for (int i = 2; i <= n; i++) {
		curr = prev1 + prev2;
		
		// Update previous two Fibonacci
		// numbers for next number
		prev2 = prev1;
		prev1 = curr;
	}
	
	return curr;
	
}