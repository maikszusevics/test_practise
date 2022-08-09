# test practise:
<img width="352" alt="5" src="https://user-images.githubusercontent.com/110176257/183426304-71ebe318-a23a-4ac4-9be6-d5f6f0b86049.png">

#### Time taken: less than 3 minutes
```
def find_largest(numbers):
    numbers.sort(reverse = True)
    return numbers[0]
```
tested using:
```
print(find_largest([34,54,1,3,65,2365,346,1243,]))
```


<img width="341" alt="9" src="https://user-images.githubusercontent.com/110176257/183428165-239cf14a-51f3-4769-8537-e2b013f2e448.png">

#### Time taken: really long with help from sam (will do again by myself with timer)

```
def find_smallest_interval(numbers):
    numbers.sort(reverse = True)
    differences = []
    if len(numbers)>100000 or len(numbers) < 2:
        pass
    else:
        for i in range(len(numbers)-1):
            try:
                differences.append(((numbers[i]-numbers[i+1])))
            except OverflowError:
                pass
        return(sorted(differences)[0])
```


![image](https://user-images.githubusercontent.com/110176257/183448472-c696e67b-4eff-46ae-84c7-24969d5ca2bc.png)

#### time taken: less than 6 minutes:

```
def oddevencounter(number):
    lst = [0,0]
    for i in range(number+1):
        if i % 2 == 0:
            lst[0] += i
        else:
            lst[1] += i
    return lst
print(oddevencounter(5))
```

1700 update: On call explaining exam questions and codewars with fatima

1800 update: on call with fetima helping with codewars

#### Codewars code:
```
# This code returns initials of a name
def abbrev_name(name):

    name = name.split(" ")

    return f"{name[0].capitalize()[0]}.{name[-1].capitalize()[0]}"

return(abbrev_name("patrick feenan"))
```
```
# this code removes vowels from a string:
def disemvowel(string_):
    vowe = ["a", "e", "i", "o", "u", "A", "E", "I", "O", "U"]
    for i in string_:
        if i in vowe:
            string_ = string_.replace(i, "")

    return string_
```
```
# This code returns string backwards:
def solution(string):
    return(string[::-1])

return(solution("Hello"))
```
```
# this code takes input of seconds and converts it to HH:MM:SS format
import math
def make_readable(seconds):
    hh = 0
    mm = 0
    ss = 0
    if seconds < 60:
        ss += seconds
    elif seconds >= 60 and seconds < (60 * 60):
        mm += int(seconds/60)
        ss += seconds%60
    elif seconds >= (60 * 60):
        hh += math.floor(seconds/(60*60))
        mm += math.floor((seconds%(60*60))/60)
        ss += seconds%60

    if hh<10:
        hh = f"0{str(hh)}"
    if mm<10:
        mm = f"0{str(mm)}"
    if ss<10:
        ss = f"0{str(ss)}"
    return ''.join(f"{str(hh)}" + f":{str(mm)}:{str(ss)}")
```
```
# this code takes a list of numbers and makes it into a phone number
def create_phone_number(n):
    lst = []
    for i in n:
        i = str(i)
        lst.append(i)

    return ''.join("(" + f"{''.join(lst[0:3])}" + ")" + " " + f"{''.join(lst[3:6])}" + "-" + f"{''.join(lst[6:])}")


print(create_phone_number([1, 2, 3, 4, 5, 6, 7, 8, 9, 0]))
```
```
# This code takes a year and returns which century it is inL
import math
def century(year):

    if str(year)[-2] == "00":
        print (math.floor((year/100)))
    else:
        print (math.floor((year/100 +1)))

century(1160)
```
```
# This code counts how many positives in a string and adds the negatives
def count_positives_sum_negatives(arr):
    x = 0
    y = 0
    for v in arr:
        if v > 0:
            x += 1
        elif v < 0:
            y += v
    result = [x, y]
  
    return (result)

count_positives_sum_negatives([1, 2, 3, 4, 5, 6, 7, 8, 9, 10, -11, -12, -13, -14, -15])
```
```
# this code returns biggest and smallest numbers in a list:
list = [4,6,2,1,9,63,-134,566]

def sorter(x):
    x.sort(reverse=True)
    return(f"max = {list[0]}, min = {list[-1]}")

sorter(list)


```

