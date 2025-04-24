# Fibonacci Series - First n Terms

def fibonacci(n):
    fib_series = [0, 1]
    for i in range(2, n):
        fib_series.append(fib_series[i-1] + fib_series[i-2])
    return fib_series[:n]

# Example usage
n = int(input("Enter the number of terms: "))
print("Fibonacci Series:", fibonacci(n))



# Factorial using recursion

def factorial(n):
    if n == 0 or n == 1:
        return 1
    return n * factorial(n - 1)

# Example usage
num = int(input("Enter a number to find factorial: "))
print("Factorial of", num, "is", factorial(num))

# Find Greatest of Three Numbers

def greatest_of_three(a, b, c):
    return max(a, b, c)

# Example usage
a = int(input("Enter first number: "))
b = int(input("Enter second number: "))
c = int(input("Enter third number: "))
print("Greatest number is:", greatest_of_three(a, b, c))


# Bubble Sort

def bubble_sort(arr):
    n = len(arr)
    for i in range(n):
        for j in range(n - i - 1):
            if arr[j] > arr[j + 1]:
                arr[j], arr[j + 1] = arr[j + 1], arr[j]
    return arr

# Example usage
arr = list(map(int, input("Enter numbers separated by space: ").split()))
sorted_arr = bubble_sort(arr)
print("Sorted array:", sorted_arr)


