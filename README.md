#Control flow with if, elif and else conditions


## An example of an if loop
```
weather = "Rainy"

if weather == "Rainy":
    print("Take an umbrella!")

if weather != "Rainy":
   print("Well it isn't raining..... ENJOY")
else:
    print ("Who knows what the weather is going to do....")
```

###  Ticket age example:

age = 18
```
if age <= 18:
    print(" You are not eligible to watch this movie ")
```

### For Loops and While Loops                                                        
- Loops help us iterate through our data, such as lists, dict., and sets etc.

- This loop will stop at before "bread" and will not continue the loop
```
                                                                               
shopping_list = ["eggs", "apples","milk","bread","butter"]            
for items in shopping_list:           
    if items == "bread":     
        break # Stops the loop 
    print(items)
```    


#### Loops with dict.                                                                     
```
student_data = {                                                                            
    "student_name" : "Niki",                                                                
    "course" : "DevOps",                                                                    
    "course_topics" : 4,                                                                    
    "topic_names" : ["Business week", "Python", "virtualisation with Vagrant","AWS cloud"]  
}                                                                                           
print(student_data)                                                                        

```

- Iterate through our dictionary                                                          

```
for data in student_data.values():                                                          
    if data == "Niki":                                                                      
        print(data)                                                                         
                                                                                            
```                                                                                            
    

#### While Loops is essentially used to monitor the data                                        
- Simple iteration of while loop, prints numbers from 0-9                                       
 ```                                                                                                 
num = 0                                                                                           
while num < 10:                                                                                   
    print(f"it's working-> {num}")   # f = formats the                                            
    num +=1                                                                                       
 ```                                                                                                 
                                                                                                  
- Prints until number 5 then breaks                                                             
```                                                                                                  
num =0                                                                                            
while num <10:                                                                                    
    print(f"It's working -> {num}")                                                               
    if num == 5:                                                                                  
        break                                                                                     
    num += 1                                                                                      
```

 **TASK**                                                                                        
 - Prompt with user to input age and restrict to enter in only digits                            
 - Check if data is in digits, display back to user                                              
 - If not in digits, prompt the user with message to enter in digits                             
``` 
                                                                                                 
user_age = input("Please enter your age as a digit: ")                                            
digit_check = user_age.isdigit()                                                                  
                                                                                                  
if digit_check == True:                                                                           
    print(f"Good job, this is a digit: {user_age}")                                               
else:                                                                                             
    print("Nop not a digit, try again")                                                           
                                                                                                                                                                       
```


 **TASK**                                                                    
 - Prompt with user to input age and restrict to enter in only digits        
 - Check if data is in digits, display back to user                          
 - If not in digits, prompt the user with message to enter in digits         
                                                                              
 ```                                                                             
while True:                                                                   
    user_age = input("Please enter your age as a digit: ")                    
    digit_check = user_age.isdigit()                                          
                                                                              
    if digit_check == True:                                                   
        print(f"Good job, this is a digit: {user_age}")                       
        break                                                                 
    else:                                                                     
        print("Nop not a digit, try again")                                   
                                                                              
```                                                                              
 - Teachers Example                                                            
 ```                                                                             
user_prompt = True                                                            
                                                                              
while user_prompt:                                                            
    age= input("Please enter your age: ")                                     
    if age.isdigit() and int(age) >0:                                         
        user_prompt = False                                                   
    else:                                                                     
        print("Please provide your answer in a digit")                        
print(f"Your age is {age}")                                                   
                                                                              
 ```                                                                                           