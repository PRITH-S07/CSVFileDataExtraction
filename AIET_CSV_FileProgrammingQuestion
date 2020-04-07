datasalM=[]
datasalF=[]
datasalmech=[]
import csv
sum=0
summech=0
nmalhy=0
with open("StudentData.csv","r") as std:
  ab=csv.reader(std)
  next(ab)
  for row in ab:
    sum+=int(row[4])
    if row[5]=="Male":
      datasalM.append(int(row[4]))
      if row[3]=="Hyd":
        nmalhy+=1
    else:
      datasalF.append(int(row[4]))
    if row[1]=="Mech":
      datasalmech.append(row[4])
      summech+=int(row[4])
  print("Total sum of package:",sum)
  minm=datasalM[0]
  for i in datasalM:
    if minm>i:
      minm=i
  print("Minimum Package from Male Gender group:",minm)
  print("Maximum Package from the Female Gender group:",max(datasalF))
  print("Avg Package received by Mech branch:",summech/len(datasalmech))
  print("No. of Male people selected from City Hyd:",nmalhy)
