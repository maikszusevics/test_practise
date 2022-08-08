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



