# <u>Assignment - 2</u>

Q \ Separate the **"Even" & "Odd"** numbers between 1-20 in this List 

myNumbers = [1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20];

 if "Even" add it to list called "myEven". if "Odd" add it to list called "myOdd". 

And print the three lists in final(myNumbers & myEven & myOdd) ?

1-) Method One :

```dart
main() {
  var myNumbers = [1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20];
  var myOdd = [];
  var myEven = [];

  for (var i = 0; i < myNumbers.length; i++) {
    if (myNumbers[i] % 2 == 0) {
      myEven.add(myNumbers[i]);
    } else {
      myOdd.add(myNumbers[i]);
    }
  }

  print("Main Numbers => $myNumbers");
  print("#"*50);
  print("Even => $myEven");
  print("#"*50);
  print("Odd => $myOdd");
}
```

****

2-) Method Two :

```dart
main() {
  var myNumbers = [1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20];
  var myOdd = [];
  var myEven = [];
  
  var i = 0;
  while (i < myNumbers.length) {
    if (myNumbers[i] % 2 == 0) {
      myEven.add(myNumbers[i]);
    } else {
      myOdd.add(myNumbers[i]);
    }
    i++;
  }
  
  print("Main Numbers => $myNumbers");
  print("#"*50);
  print("Even => $myEven");
  print("#"*50);
  print("Odd => $myOdd");
}
```

****

3-) Method Three :

```dart
main() {
  var myNumbers = [1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20];
  var myOdd = [];
  var myEven = [];
  
  var i = 0;
  do {
    if (myNumbers[i] % 2 == 0) {
      myEven.add(myNumbers[i]);
    } else {
      myOdd.add(myNumbers[i]);
    }
    i++;
  } while (i < myNumbers.length);

  print("Main Numbers => $myNumbers");
  print("#"*50);
  print("Even => $myEven");
  print("#"*50);
  print("Odd => $myOdd");
}
```

****

4-) Method Four :

```dart
main() {
  var myNumbers = [1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20];
  var myOdd = [];
  var myEven = [];

  myNumbers.forEach((i){
    if (i % 2 == 0) {
      myEven.add(i);
    } else {
      myOdd.add(i);
    }
  });

  print("Main Numbers => $myNumbers");
  print("#"*50);
  print("Even => $myEven");
  print("#"*50);
  print("Odd => $myOdd");
}
```

***

Output :

```
Main Numbers => [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20]
##################################################
Even => [2, 4, 6, 8, 10, 12, 14, 16, 18, 20]
##################################################
Odd => [1, 3, 5, 7, 9, 11, 13, 15, 17, 19]
```

