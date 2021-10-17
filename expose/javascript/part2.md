1. Line 12 will output 2, since the length of *prices* is 3 and *i* iterates as long as it is less than the length of *prices*. It only outputs 2 because it is being printed after the for loop is over.
2. Line 13 will output the discounted price for the last item in the *prices* container, which is 150, because the final iteration of the loop is at i=2 which means *discountedPrice* = prices[2] * (1-*discount*) = 150.
3. Line 14 will output the same thing as line 13. *finalPrice* is meant to round the number in case *discountedPrice* is not a whole number, but since 150 is a whole number, *finalPrice* = *discountedPrice*.
4. This function will return an array of discounted prices that are discounted based on the input. In this case, since the input prices were [100, 200, 300], and the discount specified was 0.5, the function will output [50, 100, 150].
5. I believe that line 12 will still output 2, since *i* is declared with *let* outside the scope of the for loop.
6. This will cause an error. Since *discountedPrice* is declared using *let* inside the scope of the for loop, it won't exist outside of the for loop, which is where it is trying to be printed.
7. Line 14 will still output 150. Since *finalPrice* was declared using *let* at the start of the function, it can be used throughout the entire function.
8. This function will still return the same array of discounted prices, [50, 100, 150]. In this case, changing the variable declarations from *var* to *let* did not affect the functionality of the function, because none of the variables needed to be used outside the scope in which they were declared.
9. An error will occur before we even reach line 11, since we are trying to modify *discounted*, which is *const* inside the for loop.
10. An error will occur before we even reach line 12, since we are trying to modify *discounted*, which is *const* inside the for loop.
11. This code will cause an error because within the for loop, we are trying to modify *discounted* which was declared as *const*.
12. A. student.name
    B. student["Grad Year"]
    C. student.greeting
    D. student["Favorite Teacher"].name
    E. student.courseLoad[1]

13. A. '32', because integers map to their exact string representation
    B. 1, because subtraction will convert '3' to it's integer representation - 3
    C. 3, because null maps to 0 in numeric operations
    D. '3null', because null maps to itself in string operations
    E. 4, because true maps to 1 in numeric operations
    F. 0, because false and null both map to 0 in numeric operations
    G. '3undefined', because undefinded maps to itself in string operations
    H. NaN, because undefined maps to NaN in numeric operations

14. A. True, when JS is comparing values of different types, the values are converted to numbers
    B. False, because dictionary comparison and '2' > '1'
    C. True, when JS is comparing values of different types, the values are converted to numbers
    D. False, because 2 and '2' are different types, and we compared using the strict equality operator
    E. False, when JS is comparing values of different types, the values are converted to numbers, so true = 1 and 1 != 2
    F. True, since Boolean(2) == true

15. == checks equality after type conversion, while === checks equality without type conversion. For example, '2' == 2 is true, but '2' === 2 is false
17. *modifyArray* will return an array in which each element is double what it was inputted as. In this case, since the input was [1, 2, 3], *modifyArray* will return [2, 4, 6]. This is because the for loop pushes the result of the callback function (which returns the input*2) to the return array
19. The output is 1,4,3,2 because 1 and 4 have no delay, then 3 has a 0 second delay, then 2 has a one second delay.
