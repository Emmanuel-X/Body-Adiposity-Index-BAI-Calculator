# Interactive Body-Adiposity-Index-BAI-Calculator
# Created with Python

"""This function is basically for the user's age, which checks if the age of the user is within a certain range, since BAI is age and gender dependent."""
def male_age():
    if age <= 39:
        return male_bai1()
    elif age <= 59:
        return male_bai2()
    else:
        return male_bai3()
    
def female_age():
    if age <= 39:
        return female_bai1()
    elif age <= 59:
        return female_bai2()
    else:
        return female_bai3()
      

def male_bai1():                                                       # BAI for Men from 20 - 39
    if bai <= 8:                               
        print(user_name)
        print("bai:")
        print("{0} %".format(bai))
        print("status: ")
        print("underweight")
    
    elif bai <= 21:
        print(user_name)
        print("bai:")
        print("{0} %".format(bai))
        print("status: ")
        print("healthy")
    
    elif bai <= 25:
        print(user_name)
        print("bai:")
        print("{0} %".format(bai))
        print("status: ")
        print("overweight")
    
    else:
        print(user_name)
        print("bai:")
        print("{0} %".format(bai))
        print("status: ")
        print("obese")
        
def male_bai2():                                                             # BAI for Men from 40 - 59  
    if bai <= 11:
        print(user_name)
        print("bai:")
        print("{0} %".format(bai))
        print("status: ")
        print("underweight")
    
    elif bai <= 23:
        print(user_name)
        print("bai:")
        print("{0} %".format(bai))
        print("status: ")
        print("healthy")
    
    elif bai <= 28:
        print(user_name)
        print("bai:")
        print("{0} %".format(bai))
        print("status: ")
        print("overweight")
    
    else:
        print("bai:")
        print("bai:")
        print("{0} %".format(bai))
        print("status: ")
        print("obese")
        
        
def male_bai3():                                                               # BAI for Men from 60 - 79    
    if bai <= 13:                                            
        print(user_name)
        print("bai:")
        print("{0} %".format(bai))
        print("status: ")
        print("underweight")
    
    elif bai <= 25:
        print(user_name)
        print("bai:")
        print("{0} %".format(bai))
        print("status: ")
        print("healthy")
    
    elif bai <= 30:
        print(user_name)
        print("bai:")
        print("{0} %".format(bai))
        print("status: ")
        print("overweight")
    
    else:
        print(user_name)
        print("bai:")
        print("{0} %".format(bai))
        print("status: ")
        print("obese")
        
        
def female_bai1():                                                                # BAI for Women from 20 - 39
    if bai <= 21:                                      
        print(user_name)
        print("bai:")
        print("{0} %".format(bai))
        print("status: ")
        print("underweight")
    
    elif bai <= 33:
        print(user_name)
        print("bai:")
        print("{0} %".format(bai))
        print("status: ")
        print("healthy")
    
    elif bai <= 38:
        print(user_name)
        print("bai:")
        print("{0} %".format(bai))
        print("status: ")
        print("overweight")
    
    else:
        print(user_name)
        print("bai:")
        print("{0} %\n".format(bai))
        print("status: ")
        print("obese")
    
    
def female_bai2():                                                               # BAI for Women from 40 - 59
    if bai <= 23:                                       
        print(user_name)
        print("bai:")
        print("{0} %".format(bai))
        print("status: ")
        print("underweight")

    elif bai <= 35:
        print(user_name)
        print("bai:")
        print("{0} %".format(bai))
        print("status: ")
        print("healthy")
    
    elif bai <= 40:
        print(user_name)
        print("bai:")
        print("{0} %".format(bai))
        print("status: ")
        print("overweight")
    
    else:
        print(user_name)
        print("bai:")
        print("{0} %".format(bai))
        print("status: ")
        print("obese")
            
def female_bai3():                                                                  # BAI for Women from 60 - 79
    if bai <= 25:                                      
        print(user_name)
        print("bai:")
        print("{0} %".format(bai))
        print("status: ")
        print("underweight")
    
    elif bai <= 38:
        print(user_name)
        print("bai:")
        print("{0} %".format(bai))
        print("status: ")
        print("healthy")
    
    elif bai <= 42:
        print(user_name)
        print("bai:")
        print("{0} %".format(bai))
        print("status: ")
        print("overweight")
    
    else:
        print(user_name)
        print("bai:")
        print("{0} %".format(bai))
        print("status: ")
        print("obese")
            

user_name = input("Enter your name:\n")                                           # User keyoard input
user_gender = input("Enter your gender (male/female):\n")
user_age = input("Enter your age:\n")
age = int(user_age)
user_height = input("Enter your height (m):\n")
height = float(user_height)
user_hip = input("Enter your hip circumference (cm):\n")
hip = int(user_hip)

bai1 = hip / (height ** 1.5) - 18
bai = round(bai1)

"""This function help determine the user's gender(male/female) and returns the result to the age function for further processing. """
def gender_type(gender):
    if user_gender == "male":
        return male_age()
    else:
        return female_age()
    
gender_type(user_gender)
    


