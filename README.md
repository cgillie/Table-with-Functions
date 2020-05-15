# Table-with-Functions
Sample table which allows you to edit certain rows and columns

# Flexible 2d array
n=int(input('How many rows? '))
m=int(input('How many columns? '))
print('\r') #newline
rows, cols = (n, m) 
  
arr = [[0]*cols]*rows #set to 0
for row in arr: 
    print(row)

print('\r') #newline

#mass assign value
p=float(input('Mass value= '))
arr = [[p for i in range(cols)] for j in range(rows)]
for row in arr: #print function
    print(row) 

print('\r') #newline

# change the first element of the first row, can be adapted to any element. Note this starts in top left corner (quadrant 4)  
arr[0][0] = 1.0
print('first element change')
for row in arr: #print function
    print(row) 

print('\r') #newline

#change first columnt to 1
print('first column change')
for l in range (n): 
  arr[l][0]=1.0

for row in arr: #print function
    print(row) 

print('\r') #newline

#change last row
print('last row change')
for k in range (m): 
  arr[n-1][k]=1.0
for row in arr: #print function
    print(row) 

print('\r') #newline

#change last columnt to 1
print('last column change')
for l in range (n): 
  arr[l][m-1]=1.0

for row in arr: #print function
    print(row) 
