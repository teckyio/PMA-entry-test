# Tecky's Professional Mobile App(PMA) Entry Test

## Motivation
[This course](https://tecky.io/courses/PMA) is designed for students with experience in software development. It is assumed that students joining this course already know basic Javascript or other programming languages. If you don’t have any programming experience, we recommend you to join our [Micromaster in AI and Programming](https://tecky.io/courses/MAP) to learn how to build a full stack software.

## Requirement
You need to build a Restful API that has the following structure:

|API| Sample Input | Sample Output|
|---|---|---|
|GET /students |`{}` | `[{name:"Ann",year:1,averageGPA:2.7},{name:"Peter",year:4,averageGPA:3.4}]` |
|POST /students| `{name:'John',year:2}` | `{updated:1}`|
|PUT /students/:id| `{id:2,name:'Ben',year:1}` | `{updated:1}`|
|DELETE /students/:id| `{id:2}` | `{updated:1}` |

On your server side, you can use the following as your 
sample data. Therefore there is no need for database.
Also it is not necessary to maintain a json file as the file
storage.

```json
{
    "students":[
        {
            "id": 1,
            "name": "Ann",
            "year": 1,
            "averageGPA": 2.7
        },
        {
            "id": 2,
            "name": "Benn",
            "year": 2,
            "averageGPA" : 3.4
        },
        {
            "id": 3,
            "name": "Peter",
            "year": 4,
            "averageGPA" : 3.4
        }
    ]
}
```

A [Postman](https://www.getpostman.com/) file is also attached for clarification.

### Technology
The implemented should be done by NodeJS. It does not matter
which framework you make use of.

### Submission
We advise you to use [`CodeSandBox`](https://codesandbox.io/dashboard) to build your RESTful
API since it is the easiest way to share 
with us.Codesandbox allows you to build 
node right inside the browser.
