# Pandas
My cheat codes of Pandas (Python library) without output:




#CODES START


#CODE0:

import numpy as np
import pandas as pd
#CODE1:
x=[3,4,5,6,7,8]
var=pd.Series(x)
print(var,type(var))
print(var[2])

#CODE2

dic={"name":['pyhon','c','c++','java'],"por":[12,13,14,15],"rank":[1,4,3,2]}
var=pd.Series(dic)
print(var)

#CODE3

x=[1,2,3,4]
var=pd.Series(x,index=['a','s','d','f'],dtype="float",name="python")
print(var)

#CODE4:

svar=pd.Series(12,index=[1,2,3,4,5])
print(svar)

#CODE5


l=[1,2,3,4]
var=pd.DataFrame(l)
print(var)
print(type(var))

#CODE6


d={"a":[1,2,3,4,5],"s":[1,2,3,4,5]}
var=pd.DataFrame(d)
print(type(var))
print(var)

#CODE7

d={"a":[1,2,3,4,5],"s":[1,2,3,4,5],"d":[1,2,3,4,5],1:[1,2,3,4,5]}
var=pd.DataFrame(d,columns=["a",1],index=["a","s","d","f","g"])
print(type(var))
print(var)

#CODE8

d={"a":[1,2,3,14,5],"s":[1,2,3,4,5],"d":[1,2,3,4,5],1:[1,2,3,4,5]}
var=pd.DataFrame(d)
print(type(var))
print(var)
print()
print(var["a"][3])

#CODE9

d={"s":pd.Series([1,2,3,4]),"f":pd.Series([1,2,3,4])}
var=pd.DataFrame(d)
print(var)

#CODE10.

var=pd.DataFrame({"A":[1,2,3,4],"B":[5,6,7,8]})
print(var)

var["C"]=var["A"]+var["B"]
print(var)

var["C"]=var["A"] * var["B"]
print(var)

var["Check_A"]=var["A"] <=3
var["Check_B"]=var["B"] >=7
var["Check_C"]=var["C"] >=15
print(var)
