---
title: 28th October Daily Recap
draft: false
tags:
  - school
  - study
  - java
  - arrays
---
 
# Arrays and Methods
okay so lets say you have a massive fucking array
to pass it to the method we can use ...
like thins 
public static int max(intx, inty, int.... a){} -> here I craeted a method max and stated that you can put as much as values you want as long as they r integer type

lets say we pass array (1,2,3,4,5,6) ok cool
the 1 and 2 (aka first and second values ) will be passed to x and y and the remaining will go as an arrray to a. We can pass more 

RULES:
YOU CAN ONLY HAVE 1 a.... or shit like that

REMEMBER THAT IT STILL CAN RETURN THE EMPTY LIST (FROM METHOD), with 0 length

Note: if you decide to print an erray it will just give the reference of an arrray (aka just point out where to go)
# ARRAYS CLASS IN JAVA (import)
ok so there is binary search, for this to work the list must be sorted! why?
binary search just divides the interval in half and compares, when the array is too long
why sorted because binary saerch assumes that the lsit is sorted as it will check if the value is less or greater than the vlaue it found, so if its not sorted then it will take too long

ok so 
## import java.util.Arrays; class commands
|Method|Description|Example|
|---|---|---|
|`Arrays.toString(arr)`|Converts an array into a readable string|`System.out.println(Arrays.toString(arr));`|
|`Arrays.sort(arr)`|Sorts the array in ascending order|`Arrays.sort(numbers);`|
|`Arrays.sort(arr, from, to)`|Sorts only part of the array|`Arrays.sort(nums, 2, 5);`|
|`Arrays.binarySearch(arr, key)`|Returns the index of `key` (must be sorted first)|`int i = Arrays.binarySearch(nums, 10);`|
|`Arrays.equals(arr1, arr2)`|Checks if two arrays are equal|`Arrays.equals(a, b);`|
|`Arrays.copyOf(arr, newLength)`|Copies elements into a new array of given size|`int[] copy = Arrays.copyOf(nums, 5);`|
|`Arrays.copyOfRange(arr, start, end)`|Copies part of an array|`int[] part = Arrays.copyOfRange(nums, 1, 4);`|
|`Arrays.fill(arr, value)`|Fills every element with a given value|`Arrays.fill(arr, 0);`|
|`Arrays.deepToString(arr2D)`|Prints multidimensional arrays nicely|`System.out.println(Arrays.deepToString(matrix));`|
|`Arrays.deepEquals(a, b)`|Compares nested arrays (2D/3D arrays)|`Arrays.deepEquals(arr1, arr2);`|
|`Arrays.stream(arr)`|Creates a Stream (for filtering, sum, etc.)|`int sum = Arrays.stream(nums).sum();`|
|`Arrays.hashCode(arr)`|Generates a hash for an array|`int h = Arrays.hashCode(nums);`|
|`System.arraycopy(src, start1, dest, start2, length)`|Fast copy of one array to another|`System.arraycopy(a, 0, b, 0, 3);`|


## import java.util.ArrayList; class commands
| Method               | Description                        | Example                            |
| -------------------- | ---------------------------------- | ---------------------------------- |
| `add(value)`         | Adds element to end                | `list.add("Hi");`                  |
| `add(index, value)`  | Inserts element at position        | `list.add(2, "Wow");`              |
| `get(index)`         | Returns element at position        | `System.out.println(list.get(0));` |
| `set(index, value)`  | Replaces element                   | `list.set(1, "New");`              |
| `remove(index)`      | Removes element at position        | `list.remove(2);`                  |
| `remove(Object)`     | Removes first occurrence of object | `list.remove("Hi");`               |
| `size()`             | Returns number of elements         | `System.out.println(list.size());` |
| `clear()`            | Removes all elements               | `list.clear();`                    |
| `contains(value)`    | Checks if list has a value         | `list.contains("Hi");`             |
| `isEmpty()`          | True if list has no elements       | `list.isEmpty();`                  |
| `indexOf(value)`     | Returns first index of element     | `list.indexOf("Hi");`              |
| `lastIndexOf(value)` | Returns last index of element      | `list.lastIndexOf("Hi");`          |
| `toArray()`          | Converts list → array              | `Object[] arr = list.toArray();`   |
| `equals(list2)`      | Compares lists                     | `list1.equals(list2);`             |