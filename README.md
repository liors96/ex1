# ex1

def twoNumberSum(array, targetSum):
    for i in range(len(array) - 1):
        for j in range(i + 1, len(array)):
            if array[i] + array[j] == targetSum:
                return [array[i], array[j]]

    return []


arr = []
how_many_ints = int(input("enter number of integers in the array: "))
print("enter an array: ")
for i in range(how_many_ints):
    user_input = int(input())
    arr.append(user_input)
print(arr)
t_sum = int(input("enter the target sum: "))
print(twoNumberSum(arr, t_sum))

