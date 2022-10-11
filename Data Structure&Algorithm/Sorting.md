# 🔢Sorting

## What to study - resources I find helpful📚



## My Implementation🧰



## LeetCode✏️



## Study Note ✍️

### Bubble sort

Pairs of adjacent elements are compared, and the elements swapped if they are not in order

```
for i:=0 to size(list)
	for j:=0 to size(list)-i-j:
		if(list[j]>list(j+1)):
			swap element
```

Complexity: O(n^2)

### Selection sort

Search through an array and keep track of the minimum value during each iteration. At the end of each iteration, we swap variables.

```
for i:=0 to size(list):
	min-value := list[i]
	min_index := i
	for j:= i to size(list):
		if list[j]<min_value:
			min_value = list[j]
			min_index = j
	swap list[i] and list[min-index]
```

Complexity: O(n^2)

### Insertion sort

```
for i:= 1 to size 
	value:= list[i]
	j:=i
	while j > 0 and list[j-1] >value
		list[j] = list[j-1]
		j = j-1
	list[j] = value
```

Complexity: O(n^2)
