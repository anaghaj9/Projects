# Project 1
CSE 231 Project SS23
#write your code in this window
"""
Computer Project #1

Program asks for input of a floating-point value in distance of rods, reprints value,
and converts said value to meters, feet, miles, furlongs, and time in 
minutes to walk the distance

"""

rods = input("Input rods: ") #input from user asking for a rods value
rodsFloat = float(rods) #converted given rods to a float-point value
print("\nYou input", rodsFloat, "rods.") #printed rods value after converted to decimal as a float-point value


meters = (5.0292 * rodsFloat) #meters conversions
feet = (meters / 0.3048) #feet conversions
miles = (meters / 1609.34) #miles conversions
furlongs = (rodsFloat / 40) #furlongs conversions
minutes = ((60/3.1) * miles) #minutes conversions

#print statements
print("\nConversions")
print("Meters:", round(meters, 3)) #meters value after rounded
print("Feet:", round(feet, 3)) #feet value after rounded
print("Miles:", round(miles, 3)) #miles value after rounded
print("Furlongs:", round(furlongs, 3)) #furlongs value after rounded
print("Minutes to walk",rodsFloat, "rods:", round(minutes, 3)) #minutes to walk value after rounded
