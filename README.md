# Remainder-on-dividing-by-11
java, problem of the day , geeksforgeeks , solution 


class Solution 
{ 
    static int xmod11(String x)
	{    
	    // code here
	      char[] ch = x.toCharArray();
        int even = 0, odd = 0;
        for(int i=0;i<ch.length;i++){
            if(i%2==0)even += ch[i] - '0';
            else odd += ch[i] - '0';
        }
        return ((odd-even)%11 + 11)%11; 
	}
} 

