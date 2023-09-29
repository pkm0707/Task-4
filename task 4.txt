------------------------------------------------------
| Do the below programs in anonymous function & IIFE |
------------------------------------------------------
1. Print odd numbers in an array ?
      let a = [1,2,3,4,5,6,9];
      function oddNumber(a)
      {
        for (let i = 0; i < a.length; i++) 
        {
          if(a[i] % 2 == 1)
          {
            console.log(a[i]);
          }
        }
      }
      oddNumber(a)

o/p : 
      1
      3
      5
      9
------------------------------------------------------------------------------
2. Convert all the strings to title caps in a string array ?
      let a = [1,2,3,4,5,6,9];
      let sum = 0;
      function add (a)
      {
        for (let i = 0; i < a.length; i++) 
        {
          sum = sum + a[i];
        }
        console.log(sum);
      }
      add (a)

o/p : 
      30
-------------------------------------------------------------------------------
3. Sum of all numbers in an array ?
      let a = ["virat","kohli","the","chase","master"];
      function titlecaps(a)
      {
        for (let i = 0; i < a.length; i++) 
        {
          let b = a[i].toUpperCase();
          console.log(b);
        }
      }
      titlecaps (a)

o/p : 
      VIRAT
      KOHLI
      THE
      CHASE
      MASTER
-------------------------------------------------------------------------------
4. Return all the prime numbers in an array ?
      let a = [10,34,56,78,90,13,17,100,4,5,9,11,371];
      function primenumber(a){
          for (let i=0;i<a.length;i++)
      {
          let p = 0;
          let n = parseInt(a[i]/2);
          let j = 2;
          while(j<=n)
          {
              if(a[i] % j == 0)
              {
                p = 1;
                break;
              }
              j++;
          }
          if (p == 0)
          {
              console.log("It is a prime number",a[i]);
          }
      }
      }
      primenumber(a)

o/p :
      It is a prime number 13
      It is a prime number 17
      It is a prime number 5
      It is a prime number 11
-------------------------------------------------------------------------------
5. Return all the palindromes in an array ?

-------------------------------------------------------------------------------
6. Return median of two sorted arrays of the same size ?
      let arr1 = [15,3,1,7,4,13];
      let arr2 = [12,5,9,22,45,2];
      function addmedian(arr1,arr2)
      {
          let arr3 = arr1.concat(arr2)
          arr3.sort(function(a,b){return a-b});
          // console.log(arr3);
          let len = arr3.length;
          // console.log("length =",len);
          let median = (len/2);
          return arr3[median] += arr3[median-1];
          // console.log(arr3[median] += arr3[median-1]);
      }
      console.log(addmedian(arr1,arr2));
      // addmedian(arr1,arr2)

o/p :
      16
-------------------------------------------------------------------------------
7. Remove duplicates from an array ?
      let arr = [1,1,2,5,6,8,5,7,1,5,6,8,4,5,6,10];
        
      function removeDuplicates(arr) {
          return [...new Set(arr)];
      }
        
      console.log(removeDuplicates(arr));

o/p :
      [ 1, 2, 5,  6,  8, 7, 4, 10] 
-------------------------------------------------------------------------------
8. Rotate an array by k times ?

-------------------------------------------------------------------------------

-------------------------------------------
| Do the below programs in arrow function |
-------------------------------------------

1. Print odd numbers in an array ?
      let a = [1,2,3,4,5,6,9];
      let myFunction = (a) => {
          for (let i = 0; i < a.length; i++) 
        {
          if(a[i] % 2 == 1)
          {
            console.log(a[i]);
          }
        }
      }
      myFunction(a);

o/p : 
      1
      3
      5
      9
-------------------------------------------------------------------------------
2. Convert all the strings to title caps in a string array ?
      let a = [1,2,3,4,5,6,9];
      let sum = 0;
      let myFunction = (a) => 
      {
        for (let i = 0; i < a.length; i++) 
        {
          sum = sum + a[i];
        }
        return sum;
      }
      console.log(myFunction(a))

o/p : 
      30
-------------------------------------------------------------------------------
3. Sum of all numbers in an array ?
      let a = ["virat","kohli","the","chase","master"];
      let myFunction = (a) =>
      {
          for (let i = 0; i < a.length; i++) 
        {
          let b = a[i].toUpperCase();
          console.log(b);
        }
      }
      myFunction(a);

o/p : 
      VIRAT
      KOHLI
      THE
      CHASE
      MASTER
-------------------------------------------------------------------------------
4. Return all the prime numbers in an array ?
      let a = [10,34,56,78,90,13,17,100,4,5,9,11,371];
      let myFunction = (a) =>
      {
          for (let i=0;i<a.length;i++)
      {
          let p = 0;
          let n = parseInt(a[i]/2);
          let j = 2;
          while(j<=n)
          {
              if(a[i] % j == 0)
              {
                p = 1;
                break;
              }
              j++;
          }
          if (p == 0)
          {
              console.log("It is a prime number",a[i]);
          }
      }
      }
      myFunction(a)

o/p :
      It is a prime number 13
      It is a prime number 17
      It is a prime number 5
      It is a prime number 11
-------------------------------------------------------------------------------
5. Return all the palindromes in an array ?

-------------------------------------------------------------------------------
