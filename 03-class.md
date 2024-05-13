# File I/O
## definition:
File I/O is the ability of a program to take a file as input or create a file as output.

File I/O is crucial for developing programs that need to store or retrieve data persistently. It enables applications to interact with files on the filesystem, facilitating tasks such as data storage, configuration management, and data exchange.

**open** is a functionality built into Python that allows you to open a file and utilize it in your program. The open function allows you to open a file such that you can read from it or write to it.  



    name = input("What's your name? ")

    file = open("names.txt", "r")
    file.write(name)
    file.close()

- **"names.txt"** is the name of the file that you want to open
- **"w"** is the mode you want to use, in this case it is write
other modes are also avalible like 
- **"r"** for reading a file
- **"a"** appending to a file, it different from writing by which "a" do not overwrite the 
file content as "w" do, the following example shows the the difference: 


suppose I have a file called **names.txt** that contains the following: 
>> Anas Knbar  
>> Waled Ali  
>> Mohammad Yousef  
>> Rame Hussen  

using the below code with the "w" it's going to overwrite the content file and replace it with the new name.

    

      name = input("What's your name? ")
      file = open("names.txt", "w")
      file.write(name)
      file.close()

resulting with following file. 

>> 'the new name only'

on the other hand using 'a' it will give the following file.

>> Anas Knbar  
>> Waled Ali  
>> Mohammad Yousef  
>> Rame Hussen  
>> 'the new name'

## with 

The keyword **with** allows you to automate the closing of a file.



    name = input("What's your name? ")

    with open("names.txt", "a") as file:
        file.write(f"{name}\n")







