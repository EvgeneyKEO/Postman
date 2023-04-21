### _CONTENT_
__________________
### [:arrow_forward: Postman_HW_1](https://github.com/EvgeneyKEO/Postman#large_orange_diamond-postman_hw_1)
> [:one: EP_1](https://github.com/EvgeneyKEO/Postman/blob/main/README.md#small_orange_diamond-ep_1)
[:two: EP_2](https://github.com/EvgeneyKEO/Postman/blob/main/README.md#small_orange_diamond-ep_2)
[:three: EP_3](https://github.com/EvgeneyKEO/Postman/blob/main/README.md#small_orange_diamond-ep_3)
[:four: EP_4](https://github.com/EvgeneyKEO/Postman/blob/main/README.md#small_orange_diamond-ep_4)
[:five: EP_5](https://github.com/EvgeneyKEO/Postman/blob/main/README.md#small_orange_diamond-ep_5)
[:six: EP_6](https://github.com/EvgeneyKEO/Postman/blob/main/README.md#small_orange_diamond-ep_6)
[:seven: EP_7](https://github.com/EvgeneyKEO/Postman/blob/main/README.md#small_orange_diamond-ep_7)


### [:arrow_forward: Postman_HW_2](https://github.com/EvgeneyKEO/Postman#large_orange_diamond-postman_hw_2)
> [:one: №_1](https://github.com/EvgeneyKEO/Postman/blob/main/README.md#small_orange_diamond-1)
[:two: №_2](https://github.com/EvgeneyKEO/Postman/blob/main/README.md#small_orange_diamond-2)
[:three: №_3](https://github.com/EvgeneyKEO/Postman/blob/main/README.md#small_orange_diamond-3)
[:four: №_4](https://github.com/EvgeneyKEO/Postman/blob/main/README.md#small_orange_diamond-4)
[:five: №_5](https://github.com/EvgeneyKEO/Postman/blob/main/README.md#small_orange_diamond-5)
___________________
# :large_orange_diamond: [Postman_HW_1](https://github.com/EvgeneyKEO/Postman/blob/4ef821160358bc7d982ca6cd84b4a0f43a9dcf71/Home%20work%20%231.postman_collection.json)
### _Создать запросы в Postman_
```
Protocol: http
IP: 162.55.220.72
Port: 5005
```
____________________

### :small_orange_diamond: [EP_1](https://github.com/EvgeneyKEO/Postman/blob/main/Home%20work%20%231.postman_collection.json#:~:text=name%22%3A%20%22-,EP_1,-%22%2C)
### _Дано_
```
Method: GET
EndPoint: /get_method
request url params: 
 name: str
 age: int
```
### _Решение:_
```
1. Создаем новую коллекцию - переходим в раздел "Collections" --> нажимаем "+" 
2. Создаем новый запрос ПКМ по названию ранее созданной коллекции, выбираем "Add request"
3. Выбираем метод запроса GET, вставляем в URL - http://162.55.220.72:5006/get_method
4. На вкладке "Params" заносим параметры в столбцы "KEY" (ключ) - (name, age),
"VALUE" (значение) - Evgen, 24 соответственно 
5. Нажимаем Send и получаем response: 
[
 “Evgeney”,
 “24”
]
```
____________________

### :small_orange_diamond: [EP_2](https://github.com/EvgeneyKEO/Postman/blob/main/Home%20work%20%231.postman_collection.json#:~:text=name%22%3A%20%22-,EP_2,-%22%2C)
### _Дано_
```
Method: POST
EndPoint: /user_info_3
request form data: 
 name: str
 age: int
 salary: int
```
### _Решение:_
```
1. Создаем новый запрос ПКМ по названию ранее созданной коллекции, выбираем "Add request"
2. Выбираем метод запроса POST, вставляем в URL - http://162.55.220.72:5006/user_info_3
3. Выбираем вкладку "Body" заносим данные в столбцы "KEY" (ключ) - (name, age, salary),
"VALUE" (значение) - Evgen, 24, 1000 соответственно 
4. Нажимаем Send и получаем response: 
{
 "age": "24",
 "family": {"children": [
            ["Alex", 24],
            ["Kate", 12]
          ],
        "u_salary_1_5_year": 4000
    },
    "name": "Evgen",
    "salary": 1000
}
```
____________________

### :small_orange_diamond: [EP_3](https://github.com/EvgeneyKEO/Postman/blob/main/Home%20work%20%231.postman_collection.json#:~:text=name%22%3A%20%22-,EP_3,-%22%2C)
### _Дано_
```
Method: GET
EndPoint: /object_info_1
request url params: 
 name: str
 age: int
 weight: int
```
### _Что должно придти в response:_
```
{
 'name': name,
 'age': age,
 'daily_food': weight * 0.012,
 'daily_sleep': weight * 2.5
}
```
### _Решение:_
```
1. Создаем новый запрос ПКМ по названию ранее созданной коллекции, выбираем "Add request"
2. Выбираем метод запроса GET, вставляем в URL - http://162.55.220.72:5006/object_info_1
3. Выбираем вкладку "Params" заносим данные в столбцы "KEY" (ключ) - (name, age, weight),
"VALUE" (значение) - Evgen, 24, 102 соответственно
4. Нажимаем Send и получаем response:
{
 "age": 24,
 "daily_food": 1.224,
 "daily_sleep": 255.0,
 "name": "Evgen"
}
```
____________________

### :small_orange_diamond: [EP_4](https://github.com/EvgeneyKEO/Postman/blob/main/Home%20work%20%231.postman_collection.json#:~:text=name%22%3A%20%22-,EP_4,-%22%2C)
### _Дано_
```
Method: GET
EndPoint: /object_info_2
request url params: 
 name: str
 age: int
 salary: int
```
### _Что должно придти в response:_
```
{
 'start_qa_salary': salary,
 'qa_salary_after_6_months': salary * 2,
 'qa_salary_after_12_months': salary * 2.7,
 'qa_salary_after_1.5_year': salary * 3.3,
 'qa_salary_after_3.5_years': salary * 3.8,
 'person': {'u_name': [user_name, salary, age],
            'u_age': age,
            'u_salary_5_years': salary * 4.2}
}
```
### _Решение:_
```
1. Создаем новый запрос ПКМ по названию ранее созданной коллекции, выбираем "Add request"
2. Выбираем метод запроса GET, вставляем в URL - http://162.55.220.72:5006/object_info_2
3. Выбираем вкладку "Params" заносим данные в столбцы "KEY" (ключ) - (name, age, salary),
"VALUE" (значение) - Evgen, 24, 1000 соответственно
4. Нажимаем Send и получаем response:
{
    "person": {
        "u_age": 24,
        "u_name": ["Evgen",1000,24],
        "u_salary_5_years": 4200.0
    },
    "qa_salary_after_1.5_year": 3300.0,
    "qa_salary_after_12_months": 2700.0,
    "qa_salary_after_3.5_years": 3800.0,
    "qa_salary_after_6_months": 2000,
    "start_qa_salary": 1000
}
```
____________________

### :small_orange_diamond: [EP_5](https://github.com/EvgeneyKEO/Postman/blob/main/Home%20work%20%231.postman_collection.json#:~:text=name%22%3A%20%22-,EP_5,-%22%2C)
### _Дано_
```
Method: GET
EndPoint: /object_info_3
request url params: 
 name: str
 age: int
 salary: int
```
### _Что должно придти в response:_
```
{
 'name': name,
 'age': age,
 'salary': salary,
 'family': {
             'children': [
                          ['Alex', 24], ['Kate', 12] 
                         ],
             'pets': {
                      'cat':{'name':'Sunny','age': 3},
                      'dog':{'name':'Luky','age': 4}
                     },
  'u_salary_1_5_year': salary * 4}
}
```
### _Решение:_
```
1. Создаем новый запрос ПКМ по названию ранее созданной коллекции, выбираем "Add request"
2. Выбираем метод запроса GET, вставляем в URL - http://162.55.220.72:5006/object_info_3
3. Выбираем вкладку "Params" заносим данные в столбцы "KEY" (ключ) - (name, age, salary),
"VALUE" (значение) - Evgen, 24, 1000 соответственно
4. Нажимаем Send и получаем response:
{
    "age": "24",
    "family": {
        "children": [
            ["Alex", 24],
            ["Kate", 12]
        ],
        "pets": {"cat": {"age": 3,"name": "Sunny"},
                 "dog": {"age": 4, "name": "Luky"}
        },
        "u_salary_1_5_year": 4000
    },
    "name": "Evgen",
    "salary": 1000
}
```
____________________

### :small_orange_diamond: [EP_6](https://github.com/EvgeneyKEO/Postman/blob/main/Home%20work%20%231.postman_collection.json#:~:text=name%22%3A%20%22-,EP_6,-%22%2C)
### _Дано_
```
Method: GET
EndPoint: /object_info_4
request url params: 
 name: str
 age: int
 salary: int
```
### _Что должно придти в response:_
```
{
 'name': name,
 'age': int(age),
 'salary': [salary, str(salary * 2), str(salary * 3)]
}
```
### _Решение:_
```
1. Создаем новый запрос ПКМ по названию ранее созданной коллекции, выбираем "Add request"
2. Выбираем метод запроса GET, вставляем в URL - http://162.55.220.72:5006/object_info_4
3. Выбираем вкладку "Params" заносим данные в столбцы "KEY" (ключ) - (name, age, salary),
"VALUE" (значение) - Evgen, 24, 1000 соответственно
4. Нажимаем Send и получаем response:
{
    "age": 24,
    "name": "Evgen",
    "salary": [1000, "2000", "3000"]
}
```
____________________

### :small_orange_diamond: [EP_7](https://github.com/EvgeneyKEO/Postman/blob/main/Home%20work%20%231.postman_collection.json#:~:text=name%22%3A%20%22-,EP_7,-%22%2C)
### _Дано_
```
Method: POST
EndPoint: /user_info_2
request form data: 
 name: str
 age: int
 salary: int
```
### _Что должно придти в response:_
```
{
 'start_qa_salary': salary,
 'qa_salary_after_6_months': salary * 2,
 'qa_salary_after_12_months': salary * 2.7,
 'qa_salary_after_1.5_year': salary * 3.3,
 'qa_salary_after_3.5_years': salary * 3.8,
 'person': {'u_name': [user_name, salary, age],
            'u_age': age,
            'u_salary_5_years': salary * 4.2}
}
```
### _Решение:_
```
1. Создаем новый запрос ПКМ по названию ранее созданной коллекции, выбираем "Add request"
2. Выбираем метод запроса POST, вставляем в URL - http://162.55.220.72:5006/user_info_2
3. Выбираем вкладку "Body" заносим данные в столбцы "KEY" (ключ) - (name, age, salary),
"VALUE" (значение) - Evgen, 24, 1 соответственно
4. Нажимаем Send и получаем response:
{
    "person": {"u_age": 24, "u_name": ["Evgen", 1, 24],"u_salary_5_years": 4.2},
    "qa_salary_after_1.5_year": 3.3,
    "qa_salary_after_12_months": 2.7,
    "qa_salary_after_3.5_years": 3.8,
    "qa_salary_after_6_months": 2,
    "start_qa_salary": 1
}
```
____________________        

# :large_orange_diamond: [Postman_HW_2](https://github.com/EvgeneyKEO/Postman/blob/75ca19c0fde2b178bd92d5936716a6514791e65c/Home%20work%20%232.postman_collection.json)

### :small_orange_diamond: [№1](https://github.com/EvgeneyKEO/Postman/blob/main/Home%20work%20%232.postman_collection.json#:~:text=name%22%3A%20%22-,/first,-%22%2C)
http://162.55.220.72:5005/first
1. Отправить запрос.
2. Статус код 200
```
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});
```
3. Проверить, что в body приходит правильный string.
```
pm.test("Body is correct", function () {
    pm.response.to.have.body("This is the first responce from server!ss");
});
```
_____________________________________

### :small_orange_diamond: [№2](https://github.com/EvgeneyKEO/Postman/blob/main/Home%20work%20%232.postman_collection.json#:~:text=%3A%20%22/-,user_info_3,-%22%2C)
http://162.55.220.72:5005/user_info_3
1. Отправить запрос.
2. Статус код 200
```
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});
```
3. Спарсить response body в json.
```
let resp = pm.response.json();
```
4. Проверить, что name в ответе равно name s request (name вбить руками.)
```
pm.test("Name in response = name in request", function () {
    pm.expect(resp.name).to.eql("Evgen");
});
```
5. Проверить, что age в ответе равно age s request (age вбить руками.)
```
pm.test("Age in response = Age in request", function () {
    pm.expect(resp.age).to.eql("24");
});
```
6. Проверить, что salary в ответе равно salary s request (salary вбить руками.)
```
pm.test("Salary in response = Salary in request", function () {
    pm.expect(resp.salary).to.eql(3000);
});

```
7. Спарсить request (из POST метода).
```
let req = request.data;
```
8. Проверить, что name в ответе равно name в request (name забрать из request.)
```
pm.test("Name in response = name in request №2", function () {
    pm.expect(resp.name).to.eql(req.name);
});
```
9. Проверить, что age в ответе равно age в request (age забрать из request.)
```
pm.test("Age in response = Age in request №2", function () {
    pm.expect(resp.age).to.eql(req.age);
});
```
10. Проверить, что salary в ответе равно salary s request (salary забрать из request.)
> Сперва поменяем тип данных salary в запросе из строки в число, потом сделаем проверку
```
let req_salary = +req.salary
pm.test("Salary in response = Salary in request №2", function () {
    pm.expect(resp.salary).to.eql(req_salary);
});
```
11. Вывести в консоль параметр family из response.
```
console.log("resp_family = " + typeof resp.family)
```
12. Проверить что u_salary_1_5_year в ответе равно salary*4 (salary забрать из request)
```
let req_salary_1_5 = req_salary * 4
pm.test("resp_salary_1_5 = req_salary * 4", function () {
    pm.expect(resp.family.u_salary_1_5_year).to.eql(req_salary_1_5);
});
```
_______________________________________

### :small_orange_diamond: [№3](https://github.com/EvgeneyKEO/Postman/blob/main/Home%20work%20%232.postman_collection.json#:~:text=%3A%20%22/-,object_info_3,-%22%2C)
http://162.55.220.72:5005/object_info_3
1. Отправить запрос.
2. Статус код 200
```
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});
```
3. Спарсить response body в json.
```
let resp = pm.response.json();
```
4. Спарсить request.
```
let req = pm.request.url.query.toObject();
```
5. Проверить, что name в ответе равно name в request (name забрать из request.)
```
pm.test("Name in response = name in request", function () {
    pm.expect(resp.name).to.eql(req_name);
});
```
6. Проверить, что age в ответе равно age в request (age забрать из request.)
```
let req_age = req.age;
pm.test("Age in response = Age in request", function () {
    pm.expect(resp.age).to.eql(req_age);
});
```
7. Проверить, что salary в ответе равно salary s request (salary забрать из request.)
```
let req_salary = + req.salary;
console.log("req_salary = " + typeof req_salary)
console.log("resp_salary = " + typeof resp.salary)
pm.test("salary in response = salary in request", function () {
    pm.expect(resp.salary).to.eql(req_salary);
});
```
8. Вывести в консоль параметр family из response.
```
console.log("resp_family =" +typeof resp.family)
```
9. Проверить, что у параметра dog есть параметры name.
```
pm.test("Dog has a name", function () {
    pm.expect(resp.family.pets.dog).to.have.property("name")
```
10. Проверить, что у параметра dog есть параметры age.
```
pm.test("Dog has an age", function () {
    pm.expect(resp.family.pets.dog).to.have.property("age")
}); 
```
11. Проверить, что параметр name имеет значение Luky.
```
pm.test("Name has Lucky", function () {
    pm.expect(resp.family.pets.dog.name).to.be.oneOf(["Luky"])
}); 
```
12. Проверить, что параметр age имеет значение 4.
```
pm.test("Age has 4", function () {
    pm.expect(resp.family.pets.dog.age).to.be.oneOf([4])
}); 
```
_______________________________________

### :small_orange_diamond: [№4](https://github.com/EvgeneyKEO/Postman/blob/main/Home%20work%20%232.postman_collection.json#:~:text=%3A%20%22/-,object_info_4,-%22%2C)
http://162.55.220.72:5005/object_info_4
1. Отправить запрос.
2. Статус код 200
```
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});
```
3. Спарсить response body в json.
```
let resp = pm.response.json();
```
4. Спарсить request.(из GET метода)
```
let req = pm.request.url.query.toObject()
```
5. Проверить, что name в ответе равно name в request (name забрать из request.)
```
pm.test("Name in response = name in request", function () {
    pm.expect(resp.name).to.eql(req.name);
});
```
6. Проверить, что age в ответе равно age из request (age забрать из request.)
```
pm.test("age in response = age in request", function () {
    pm.expect(resp.age).to.eql(+req.age);
});
```
7. Вывести в консоль параметр salary из request.
```
console.log ("req_salary = " + typeof req.salary)
```
8. Вывести в консоль параметр salary из response.
```
console.log ("resp_salary = " + typeof resp.salary)
```
9. Вывести в консоль 0-й элемент параметра salary из response.
```
console.log ("resp_salary_element_0 = " + resp.salary[0])
```
10. Вывести в консоль 1-й элемент параметра salary параметр salary из response.
```
console.log ("resp_salary_element_1 = " + resp.salary[1])
```
11. Вывести в консоль 2-й элемент параметра salary параметр salary из response.
```
console.log ("resp_salary_element_2 = " + resp.salary[2])
```
12. Проверить, что 0-й элемент параметра salary равен salary из request (salary забрать из request.)
```
pm.test("salary_element_0 = req_salary", function () {
    pm.expect(+resp.salary[0]).to.eql(+req.salary);
});
```
13. Проверить, что 1-й элемент параметра salary равен salary*2 из request (salary забрать из request.)
```
pm.test("salary_element_1 = req_salary", function () {
    pm.expect(+resp.salary[1]).to.eql(req.salary*2);
});
```
14. Проверить, что 2-й элемент параметра salary равен salary*3 из request (salary забрать из request.)
```
pm.test("salary_element_2 = req_salary", function () {
    pm.expect(+resp.salary[2]).to.eql(req.salary*3);
});
```
15. Создать в окружении переменную name, age, salary
```
environments --> tap '+' ---> add variable
```
16. Передать в окружение переменную name
```
pm.environment.set("name", "Evgen");
```
17. Передать в окружение переменную age
```
pm.environment.set("age", 24);
```
18. Передать в окружение переменную salary
```
pm.environment.set("salary", 1000);
```
19. Написать цикл который выведет в консоль по порядку элементы списка из параметра salary.
```
for (i = 0; i < resp.salary.length; i++){
    console.log ("salary = ", resp.salary[i])
}
```
_______________________________________

### :small_orange_diamond: [№5](https://github.com/EvgeneyKEO/Postman/blob/main/Home%20work%20%232.postman_collection.json#:~:text=%3A%20%22/-,user_info_2,-%22%2C)
http://162.55.220.72:5005/user_info_2
1. Вставить параметр salary из окружения в request
2. Вставить параметр age из окружения в age
3. Вставить параметр name из окружения в name
4. Отправить запрос.
5. Статус код 200
```
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});
```
6. Спарсить response body в json.
```
let resp = pm.response.json();
```
7. Спарсить request.
```
let req = request.data;
```
8. Проверить, что json response имеет параметр start_qa_salary
```
pm.test("json response имеет параметр start_qa_salary", function () {
    pm.expect(resp).to.have.property("start_qa_salary");
});
```
9. Проверить, что json response имеет параметр qa_salary_after_6_months
```
pm.test("json response имеет параметр qa_salary_after_6_months", function () {
    pm.expect(resp).to.have.property("qa_salary_after_6_months");
});
```
10. Проверить, что json response имеет параметр qa_salary_after_12_months
```
pm.test("json response имеет параметр qa_salary_after_12_months", function () {
    pm.expect(resp).to.have.property("qa_salary_after_12_months");
});
```
11. Проверить, что json response имеет параметр qa_salary_after_1.5_year
```
pm.test("json response имеет параметр qa_salary_after_1.5_year", function () {
    pm.expect(resp).to.have.property("qa_salary_after_1.5_year");
});
```
12. Проверить, что json response имеет параметр qa_salary_after_3.5_years
```
pm.test("json response имеет параметр qa_salary_after_3.5_years", function () {
    pm.expect(resp).to.have.property("qa_salary_after_3.5_years");
});
```
13. Проверить, что json response имеет параметр person
```
pm.test("json response имеет параметр person", function () {
    pm.expect(resp).to.have.property("person");
});
```
14. Проверить, что параметр start_qa_salary равен salary из request (salary забрать из request.)
> сделал с объявлением переменной
```
let req_salary = +req.salary 
pm.test("start_qa_salary = salary из request", function () {
    pm.expect(resp.start_qa_salary).to.eql(req_salary);
});
```
15. Проверить, что параметр qa_salary_after_6_months равен salary*2 из request (salary забрать из request.)
> не объявлял переменную, умножение переводит текстовое значение в цифру
```
pm.test("qa_salary_after_6_months = salary*2 из request", function () {
    pm.expect(resp.qa_salary_after_6_months).to.eql(req.salary*2);
});
```
16. Проверить, что параметр qa_salary_after_12_months равен salary*2.7 из request (salary забрать из request.)
```
pm.test("qa_salary_after_12_months = salary*2.7 из request", function () {
    pm.expect(resp.qa_salary_after_12_months).to.eql(req.salary*2.7);
});
```
17. Проверить, что параметр qa_salary_after_1.5_year равен salary*3.3 из request (salary забрать из request.)
```
pm.test("qa_salary_after_1.5_year = salary*3.3 из request", function () {
    pm.expect(resp["qa_salary_after_1.5_year"]).to.eql(req.salary*3.3);
});
```
18. Проверить, что параметр qa_salary_after_3.5_years равен salary*3.8 из request (salary забрать из request.)
```
pm.test("qa_salary_after_3.5_year = salary*3.8 из request", function () {
    pm.expect(resp["qa_salary_after_3.5_years"]).to.eql(req.salary*3.8);
});
```
19. Проверить, что в параметре person, 1-й элемент из u_name равен salary из request (salary забрать из request.)
```
pm.test("в параметре person, 1-й элемент из u_name = salary из request", function () {
    pm.expect(resp.person.u_name[1]).to.eql(+req.salary);
});
```
20. Проверить, что что параметр u_age равен age из request (age забрать из request.)
> не объявлял переменную, добавил + к req.age - формат поменялся на number
```
pm.test("параметр u_age = age из request ", function () {
    pm.expect(resp.person.u_age).to.eql(+req.age);
});
```
21. Проверить, что параметр u_salary_5_years равен salary*4.2 из request (salary забрать из request.)
```
pm.test("параметр u_salary_5_years = salary*4.2", function () {
    pm.expect(resp.person.u_salary_5_years).to.eql(req.salary*4.2);
});
```
22. ***Написать цикл который выведет в консоль по порядку элементы списка из параметра person.
```
for (let i in resp.person){
    console.log("Property:", i, "property value:", resp.person[i])
}
