# Productiv

Productiv is a todo app using React. I used this as a project to better understand state and prop-drilling as well as practice with react-bootstrap. 

## Usage

```javascript
# install dependencies in root directory
npm start
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.


```http
  POST v1/users/
```
`userData` = ```json
{
    "first_name",
    "last_name",
    "email",
    "phone_number", 
    "date_of_birth"
}```
| Body | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `id`      | `object` | **Required**. Id of item to fetch |

#### add(num1, num2)

Takes two numbers and returns the sum.

