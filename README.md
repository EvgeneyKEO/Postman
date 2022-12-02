# :large_orange_diamond: [Postman_HW_1](https://github.com/EvgeneyKEO/Postman/blob/9d4ab651c2b9739fea00c9e1ffc1bf2bb84599f2/Home%20work%20%231.postman_collection.json)
Создать запросы в Postman.
```
Protocol: http
IP: 162.55.220.72
Port: 5005
```
____________________

### :small_orange_diamond: [EP_1](https://github.com/EvgeneyKEO/Postman/blob/main/Home%20work%20%231.postman_collection.json#:~:text=name%22%3A%20%22-,EP_1,-%22%2C)
```
Method: GET
EndPoint: /get_method
request url params: 
 name: str
 age: int
```
```
response: 
[
    “Str”,
    “Str”
]
```
____________________

### :small_orange_diamond: [EP_2](https://github.com/EvgeneyKEO/Postman/blob/main/Home%20work%20%231.postman_collection.json#:~:text=name%22%3A%20%22-,EP_2,-%22%2C)
```
Method: POST
EndPoint: /user_info_3
request form data: 
 name: str
 age: int
 salary: int
```
```
response: 
{'name': name,
          'age': age,
          'salary': salary,
          'family': {'children': [['Alex', 24], ['Kate', 12]],
                     'u_salary_1_5_year': salary * 4}}
```
____________________

### :small_orange_diamond: [EP_3](https://github.com/EvgeneyKEO/Postman/blob/main/Home%20work%20%231.postman_collection.json#:~:text=name%22%3A%20%22-,EP_3,-%22%2C)
```
Method: GET
EndPoint: /object_info_1
request url params: 
 name: str
 age: int
 weight: int
```
```
response: 
{'name': name,
          'age': age,
          'daily_food': weight * 0.012,
          'daily_sleep': weight * 2.5}
```
____________________

### :small_orange_diamond: [EP_4](https://github.com/EvgeneyKEO/Postman/blob/main/Home%20work%20%231.postman_collection.json#:~:text=name%22%3A%20%22-,EP_4,-%22%2C)
```
Method: GET
EndPoint: /object_info_2
request url params: 
 name: str
 age: int
 salary: int
```
```
response: 
{'start_qa_salary': salary,
          'qa_salary_after_6_months': salary * 2,
          'qa_salary_after_12_months': salary * 2.7,
          'qa_salary_after_1.5_year': salary * 3.3,
          'qa_salary_after_3.5_years': salary * 3.8,
          'person': {'u_name': [user_name, salary, age],
                     'u_age': age,
                     'u_salary_5_years': salary * 4.2}
          }
```
____________________

### :small_orange_diamond: [EP_5](https://github.com/EvgeneyKEO/Postman/blob/main/Home%20work%20%231.postman_collection.json#:~:text=name%22%3A%20%22-,EP_5,-%22%2C)
```
Method: GET
EndPoint: /object_info_3
request url params: 
 name: str
 age: int
 salary: int
```
```
response: 
{'name': name,
          'age': age,
          'salary': salary,
          'family': {'children': [['Alex', 24], ['Kate', 12]],
                     'pets': {'cat':{'name':'Sunny',
                                     'age': 3},
                              'dog':{'name':'Luky',
                                     'age': 4}},
                     'u_salary_1_5_year': salary * 4}
          }
```
____________________

### :small_orange_diamond: [EP_6](https://github.com/EvgeneyKEO/Postman/blob/main/Home%20work%20%231.postman_collection.json#:~:text=name%22%3A%20%22-,EP_6,-%22%2C)
```
Method: GET
EndPoint: /object_info_4
request url params: 
 name: str
 age: int
 salary: int
```
```
response: 
{'name': name,
          'age': int(age),
          'salary': [salary, str(salary * 2), str(salary * 3)]}
```
____________________

### :small_orange_diamond: [EP_7](https://github.com/EvgeneyKEO/Postman/blob/main/Home%20work%20%231.postman_collection.json#:~:text=name%22%3A%20%22-,EP_7,-%22%2C)
```
Method: POST
EndPoint: /user_info_2
request form data: 
 name: str
 age: int
 salary: int
```
```
response: 
{'start_qa_salary': salary,
          'qa_salary_after_6_months': salary * 2,
          'qa_salary_after_12_months': salary * 2.7,
          'qa_salary_after_1.5_year': salary * 3.3,
          'qa_salary_after_3.5_years': salary * 3.8,
          'person': {'u_name': [user_name, salary, age],
                     'u_age': age,
                     'u_salary_5_years': salary * 4.2}
          }
```
          
