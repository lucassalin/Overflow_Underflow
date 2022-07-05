# Arithmetic Overflow and Underflow

__Overflow__ occurs when uint reaches its byte size. 
Then the next element added will return the first variable element.  

__Underflow__ happens in the opposite direction.  

Let’s take the example of a *uint8*, which can only have 8 bits.  

The largest number we can store is binary 11111111 (2^8 – 1 = 255)

`uint8 balance = 255;`  
`balance++;`

If we execute the code above, the balance will be 0 because we are adding 1 to binary 11111111 so it will reset back to 00000000.
