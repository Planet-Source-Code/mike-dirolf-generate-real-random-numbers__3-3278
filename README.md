<div align="center">

## Generate REAL Random Numbers


</div>

### Description

//If you havent yet realized it the

//function 'rand()' will not produce

//an actual random number because it

//uses the same seed every time, the

//way to fix this is to use time as

//a seed for the rand function. If

//this helps, rate it please.
 
### More Info
 
random number


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Mike Dirolf](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/mike-dirolf.md)
**Level**          |Beginner
**User Rating**    |5.0 (20 globes from 4 users)
**Compatibility**  |C\+\+ \(general\), Microsoft Visual C\+\+, Borland C\+\+, UNIX C\+\+
**Category**       |[Miscellaneous](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/miscellaneous__3-1.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/mike-dirolf-generate-real-random-numbers__3-3278/archive/master.zip)

### API Declarations

```
#include <iostream.h>
#include <stdlib.h>
#include <time.h>
```


### Source Code

```
//Real Random Numbers
#include <iostream.h> //for the output
#include <stdlib.h> //for 'rand', 'srand'
#include <time.h> //for 'time'
int main()
 {
 //use time as seed for 'rand'
 srand(time(0));
 //create an actually random number
 int a=rand();
 cout<<a<<endl;
 system('pause');
 return 0;
 }
//if you compile and run this program
//you will see that every time you
//run it there will be a new, random
//number. if you want a number in a
//given range(lets say 0-8) replace
//the call 'rand();' with 'rand()%9'
//(notice we use 9, not 8.
//P.S. try running the same program
//I used without setting srand to time
// if you run it several times you will
//notice your output is the same every
//time!!!
```

