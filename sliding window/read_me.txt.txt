There are 4 patterns for sliding window problems 
1) Constant window - 
we have a constant window size of k and we initialize left or right pointers for this .

2) longest subarray / substring with given condition k 

Pattern for this - 

r=right pointer l=left pointer , n = no of elements 
while(r<n)
{

//condition broken shrink window
while(condition)
{
--l;
}
//expand window 
r++;

}

3) no of subarray where condition 
This asks for a count to be returned we use pattern 2 here 

For example Q is -> no of subarray where sum = k  

The solution is 
count  = (number of subarray where sum <=k) - (number of subarray where sum <=k-1)

4) shortest or minimum window with condition 
rare case 
we use l and r 
 if the window is valid we try to shrink until window becomes unvalid
