# Body-Adiposity-Index-BAI-Calculator
BAI Calculator

name = "collins"                                                               
hip_circumference = 102
height_m  = 1.8
bai = hip_circumference / (height_m ** 1.5) - 18

if bai <= 11:
    print(name)
    print("bai:")
    print(bai)
    print("is underweight")
    
elif bai <= 23:
    print(name)
    print("bai:")
    print(bai)
    print("is healthy")
    
elif bai <= 28:
    print(name)
    print("bai:")
    print(bai)
    print("is overweight")
    
else:
    print(name)
    print("bai:")
    print(bai)
    print("obessed")
    
