# homey-backend
Homey BackEnd API with PHP &amp; MySQL

**API**

| URL | Pre-requirments | Request | URL Parameters | Header Parameters | onsuccess | onerror | Description |
| :------------ | :------------ | :------------  | :------------  | :------------  | :------------ | :------------ | :------------ |
| **Authentication** |  |  |   |  |  |  |  |
| `/login` |  | POST | | Username, Password | `data: { login: true, token: GENERATED_TOKEN, message: MESSAGE }` | `data: { login: false, message: MESSAGE}` | Log a user into system |
| `/signup/` |  | POST | user | Firstname, Lastname, Email, Password | `data: { signup: true, message: MESSAGE }` | `data: { signup: false, message: MESSAGE}` | Sign up a User |
| `/signup/` |  | POST | admin | Firstname, Lastname, Email, Nic,  Password | `data: { signup: true, message: MESSAGE }` | `data: { signup: false, message: MESSAGE}` | Sign up an Admin |
| **Info** |  |  |  |  |  |  |
| `/property-type` |  | GET |  |  | `data : array [ { property_type_id : ID, property_type_name : NAME } ] ` | `data : { error : true, message : MESSAGE }` | Get all property types |
|  |  |  |  |  |  |
