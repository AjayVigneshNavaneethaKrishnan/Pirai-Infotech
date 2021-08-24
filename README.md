# Pirai-Infotech
n=input("Number of Applications:")
if n.isdigit() == True:
    n=int(n)
    list_app=[]
    for i in range(n):
        print("Enter the application detail"+str(i+1))
        an = input("Enter Application name:")
        au = input("Enter Application author name:")
        vr = input("Enter Application version:")
        yr = input("Enter Application year:")
        pr = input("Enter Application price:")
        list_app.append([an,au,vr,yr,pr])

#Display the author name to check

    aut = input("Enter the author name to check:")
    for i in range(n):
        if(list_app[i][1]) == aut:
            print(list_app[i])

#Sort the price in increasing order
    
prr = [list_app]     
temp = 0   
for i in range(0, len(list_app)):    
    print(list_app[i])
    #Sort the price in ascending order    
for i in range(0, len(list_app)):    
    for j in range(i+1,len(list_app)): 
         if(list_app[i] > list_app[j]) ==True:
            temp = list_app[i];   
            list_app[i] = list_app[j];    
            list_app[j] = temp;    
            print();    

#Displaying enter the price  after sorting    
    
print("Enter the price sorted in ascending order: ");    
for i in range(0, len(list_app)):    
    print(list_app[i]) 

#Display the publishing year

year = input("Enter the year to check:")
for i in range(n):
    if(list_app[i][1]) == year:
        print(list_app[i])

#Sort the two fields in increasing order
#Display the author name to check
    aut = input("Enter the author name to check:")
    for i in range(n):
        if(list_app[i][1]) == aut:
            print(list_app[i])
            
#Display the publishing year
year = input("Enter the year to check:")
for i in range(n):
    if(list_app[i][1]) == year:
        print(list_app[i])
      
else:
    print("Enter valid number for Number of Application")

    
