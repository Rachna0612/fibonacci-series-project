projects
def search_fibo(x):
    n1 = 0
    n2 = 1
    
    while(n1<=x):
        if(n1 == x):
            return 1
        nn = n1+n2
        n1 = n2
        n2 = nn  
    return 0


test_cases = int(input("No. of inputs: "))

li = [None for x in range(test_cases)]

for i in range(0,test_cases):
    li[i] = int(input(f"{i+1}: "))
    if(search_fibo(li[i])):
        print(f"{li[i]} is a valid fibonacci number")
    else:
        print(f"{li[i]} is not a valid fibonacci number")
