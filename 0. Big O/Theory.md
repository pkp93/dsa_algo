What is Big O ?
1. Basically how good a solution is, gives a vocabulary to talk about how our code performs. 
2. Useful to discuss trade-offs between diff approaches
3. Good for debugging as helps in identifying pain points

Compare the below code for counting the sum of n numbers. The second one is obviously faster.

Algo 1

function count(n) {
    let total = 0;
    for(let i = 1; i <= n; i++) {
        total+= i
    } 
    return total
}

Algo 2

function countWithFormula(n) {
    return (n*(n+1)/2)
}

But, how do we quantify the speed of the two algo, especially considering that they will take diff time on even same machine ?

Here Big O comes in picture. Simply how many operations a computer performs on an algo

![](2022-01-18-11-47-11.png)

Definition of time complexity : Big O notation is a way to formalize worst case fuzzy counting. It allows us to talk formally about how the runtime of an algo grows as the i/p grows 

![](2022-01-18-14-01-42.png)

Definition of space complexity : How much memory an algo is consuming. 