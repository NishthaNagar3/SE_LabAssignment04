# SE_LabAssignment04
# NEW LINE


# CODE
import pandas as pd

data = {
  "Employee ID ": ["161E90","161F91","161F99","171E20","171G30"],
  "Name": ["Raman","Himadri","Jaya","Tejas","Ajay"],
  "Age": [41,38,51,30,45],
  "Salary(PM)": [56000,67500,82100,55000,44000]
}

df = pd.DataFrame(data)
print(df)

while True:

    print("NISHTHA NAGAR --------- E22CSEU0642 --------- LabAssignment 4")
    print("------------------------Menu-----------------------")
    print("- 1. Ascending Sort with respect to Name")
    print("- 2. Ascending Sort with respect to Age")
    print("- 3. Ascending Sort with respect to Salary")
    print("- 4. Descending Sort with respect to Name")
    print("- 5. Descending Sort with respect to Age")
    print("- 6. Descending Sort with respect to Salary")
    print("- 7 (or more). Exit the perogram")
    
    choice = int(input("Enter choice: "))
    
    if choice == 1:
        df.sort_values("Name",ascending=True)
        print("Ascending sort with respect to Name: \n",df)
        
    elif choice == 2:
        df.sort_values("Age",ascending=True)
        print("Ascending sort with respect to Age: \n",df)
        
    elif choice == 3:
        df.sort_values("Salary",ascending=True)
        print("Ascending sort with respect to Salary(PM): \n",df)

    elif choice == 4:
        df.sort_values("Name",ascending=False)
        print("Descending sort with respect to Name: \n",df)

    elif choice == 5:
        df.sort_values("Age",ascending=False)
        print("Descending sort with respect to Age: \n",df)
    
    elif choice == 6:
        df.sort_values("Salary",ascending=False)
        print("Descending sort with respect to Salary(PM): \n",df)
        
    elif choice >6:
        print("EXITED!!!")
        break
        
    else:
        break