bed_count = 0
kit_count = 0
bath_count = 0
gard_count = 0
entra_count = 0
drive_way = 0
pool = 0
back = 0

for i in dict_list:
    if ("bedroom") in list(i.keys()):
        bed_count+=1
    if ("bed") in list(i.keys()):
        bed_count+=1
    if  "stove" in list(i.keys()):
        kit_count+=1
    if "bathtub" in list(i.keys()):
        bath_count+=1
    if "garden" in list(i.keys()):
        gard_count += 1
    if "entrance" in list(i.keys()):
        entra_count += 1
    if "driveway" in list(i.keys()):
        drive_way += 1
    if "pool" in list(i.keys()):
        pool += 1
    if "backyard" in list(i.keys()):
        back += 1    
    

print("*****House Summary***** ")
print("Bedrooms: " +  str(bed_count))
print("Kitchen: " + str(kit_count))
print("Bathrooms: " + str(bath_count))
if gard_count > 0:
    print("Lawn: Yes")
else:
    print("Lawn: No")
    
if (entra_count > 0) or (drive_way > 0):
    print("Parking: Yes")
else:
    print("Parking: No")

if (back > 0):
    print("Backyard: Yes")
else:
    print("Backyard: No")
    
if (pool > 0):
    print("Swimming Pool: Yes")
else:
    print("Swimming Pool: No")
    
print("\n")
print("Test Complete!")
print("\n")
    
        
        
