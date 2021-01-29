1. at line 11, the i is printed to the console. This is because i is declared as var,
thus having global scope. 
2. at line 12, the value of discounted price is printed to the console. This is 
because discountedPrice is declared as var, thus having global scope. 
3. at line 13, the value of finalPrice is printed to the console. This is because
finalPrice is declared as var, thus having global scope.
4. discountPrices([100, 200, 300], .5) will return [50, 100, 150]. The function
calculates the discounted price for each price in the array passed in.
5. an error will occur because i has block scope.
6. an error will occur because discountedPrice has block scope.
7. the value of finalPrice will be printed becuase finalPrice is declared outside
of the forloop, thus in the scope of the console log statement.
8. discountPrices([100, 200, 300], .5) will return [50, 100, 150] because every
price is discounted as 50% off.
9. an error will occur because i has block scope.
10. an error will occur because discountedPrice has block scope.
11.  the value of finalPrice will be printed becuase finalPrice is declared outside
of the forloop, thus in the scope of the console log statement.
12. The function will terminated by an error because finalPrice is declared as
const, thus cannot be reassigned.
13.     
        a. student.name

        b. student["Grad Year"]

        c. student.greet()

        d. student["Favorite Teacher"].name

        e. student.courseLoad[0]
14.     
        a. 5 because JavaScript automatically convert '3' to number, then perform the
        arithmetic operation 
        b. 1 because JavaScript automatically convert '3' to number, then perform the
        arithmetic operation 
        c. 3 because null is treated as 0 in JavaScript.
        d. '3null' because null is treated as an empty string in JavaScript.
        e. 4 because true is treated as 1 in JavaScript.
        f. 0 because false and null are treated as 0 in JavaScript.
        g. '3undefined' because undefined will be treated as string in this case.
        h. NaN because there is no string operation involving -, so undefined is
        a number here and '3' becomes 3. 3 + NaN is not a number as the result
        shows.
15. 
        a. true because '2' becomes number 2 here
        b. false because when both are string, they are compared by lexicographical
        order, and '1' comes before '2'
        c. true because == is not checking for strict equality, so '2' is treated
        as 2 here
        d. false becayse === is checking for strict equality. Since one is string
        and one is number, they are not strictly equal
        e. false because true becomes 1 and 1 does not equal 2
        f. true because Boolean(2) converts 2 to true.
16. == and === differs in that === checks for strict equality. In other words, it
checks the equality without type conversion. if a and b are of different types, then a
=== b immediately returns false without an attempt to convert them.
17. This code snippet will log "How are you?" to the console because 2 == true
evaluates to false but 2 by itself evaluates to true due to type conversion.
19. The forloop in modifyArray will run 3 times. 
The first time, it will compute doSomething(1, x*2) => function(1+2) => 6. 
The second time, it will compute doSomething(2, x*2) => function(2+2) => 8.
The third time, it will compute doSomething(3, x*2) => function(3+2) => 10. 
So the output of modifyArray([1,2,3], doSomething) is [6, 8, 10]
21. The output will be 1 4 3 2, each on a seperate line. The first line will print
1 to the console. Since JavaScript is single-threaded, asynchronous callbacks are
assigned to a message placed in a message queue. When no code is currently executing
the event loop polls the message queue, requesting the next message in line to be
processed (executed). Here, log 2 to the console with delay of 1000 millisecond
will be added to the message queue. Next line will add log 3 to the console with
0 millisecond delay to the message queue. Then, the next line will print 4 to the
console. When there is no code executing, JavaScript will look into the message
queue to pull out the logging messages. The first printed is 3 because it has 0
delay. Then 2 will be logged to the console.