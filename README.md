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

#CODE10

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

#Delete and Insert Data in Pandas
	Insert

#CODE11

var=pd.DataFrame({"A":[1,2,3,4],"B":[1,2,3,4]})
print(var)
print()
var.insert(1,"new",var["A"])
print(var)



#CODE12
var=pd.DataFrame({"A":[1,2,3,4,5],"B":[1,2,3,4,5]})
var["pyhton"]=var["A"][:3]
print(var)


	DELETE
Pop function

	#CODE13
	var=pd.DataFrame({"A":[111,2,113,114,115],"B":[11,21,31,41,51],"C":[13,14,1,5,16]})
	
	print(var)
	print()
	var=var.pop("B")
	print(var)


	DELETE FUNCTION

#CODE14
var=pd.DataFrame({"A":[111,2,113,114,115],"B":[11,21,31,41,51],"C":[13,14,1,5,16]})

print(var)
print()
del var["B"]
print(var)



Python Pandas CSV Files
  Difference between CSV and XLS (excel) file formats:
	CSV format is a plain text format in which values are separated by commas (Comma separated values).
	XLS file is an excel sheets binary file format which ho9lds information about all the worksheets in a file, including both content and formatting.
**Write CSV
Syntax to create a csv file:
var.to_csv(“file_name”)
to remove indexing and header
var.to_csv(“file_name”,index=False,header=[1,2,3])

#CODE15

dis={"A":[11,22,33,44,55],"B":[66,77,88,99,98],"C":[14,15,16,17,18]}
d=pd.DataFrame(dis)
print(d)
print()
d.to_csv("test_new1.csv",index=False,header=[1,2,3])






