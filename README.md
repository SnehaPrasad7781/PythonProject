# PythonProject
differentiating leap years
start = input("Enter the start date(dd/mm/yyyy): ")
end   = input("Enter the end date(dd/mm/yyyy): ")

start_year = int(start.split("/")[2])
end_year   = int(end.split("/")[2])

leap = []
nonleap = []

for year in range(start_year, end_year+1):
    if year%400==0 or year%4==0 and year%100!=0:
        leap.append(str(year))
    else:
        nonleap.append(str(year))


print("Leap years are:\n"," ".join(leap))
print("Non Leap years are:\n"," ".join(nonleap))
