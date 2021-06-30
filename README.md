import requests 
with open('C:\\Users\\Cheslav\\Downloads\\dataset_3378_3.txt', 'r') as file_1:
    y=file_1.readline().strip()
    print(y)
    print(type(y))
    r=requests.get(y)
    r=r.text
    print(r.count('\n')) 
