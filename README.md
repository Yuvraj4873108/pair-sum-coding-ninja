# pair-sum-coding-ninja
You have been given an integer array/list(ARR) and a number X. Find and return the total number of pairs in the array/list which sum to X.
int pairSum(int *input, int size, int x)
{
    int count =0;
    for(int i=0;i<size;i++)
    {
        int m=x-*(input+i);
        int j;
        for( j=0;j<size;j++)
        {
            if(m==*(input+j))
            {
                count++;
                
            }
        }
    }
    return count/2;
}
