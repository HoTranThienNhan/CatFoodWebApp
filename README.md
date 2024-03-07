# CAT FOOD WEB APPLICATION

<div align="center">
  <img src="https://github.com/HoTranThienNhan/CatFoodWebApp/assets/122293496/fed28be9-b43f-4814-9947-723ffe8df4f6" width="60%"/>
  <h2 align=center>This repository contains three submodules of the project which is a cat food web application using MEVN Stack 😼🥫</h2>
</div>
<div>
  <b>Cat food web application</b> is the project regarding building and developing a website system to manage the purchase and sale activities for cat food. </br></br>
  In this project, I decided to examine and analyze the e-commerce as well as the situation of cat ownership in Viet Nam. Since then, I commenced creating the cat food website system 
  which consists of sufficient basic functions of an e-commerce website system, such as reviewing products, adding products to cart, checking out and ordering, managing order history,... 
  Besides, I also built a website management for the storekeeper in order to manage all products, all orders,... 
</div>
</br></br>

> **Three submodules of this project includes:**<br/>
> i) A front-end for customers which allows them to review and purchase products.<br/>
> ii) A front-end for administrators (storekeeper and staffs) which allows them to manage purchase and sale activities of the system.<br/>
> iii) A back-end.<br/></br>

---

## Documentation
### Project Structure 
</br>
<div align="center">
  <img src="https://github.com/HoTranThienNhan/CatFoodWebApp/assets/122293496/724ef29e-1b0d-4920-82cd-d27846cb0cc8" width="70%"/>
</div>


### CDM
</br>
<div align="center">
  <img src="https://github.com/HoTranThienNhan/CatFoodWebApp/assets/122293496/51294447-1deb-437d-9f6c-4ca827126287" width="70%"/>
</div>

### Project Figures
<details open>
  </br>
  <summary><b>Customer Side</b></summary>
  
  <div align="center">
    <img src="https://github.com/HoTranThienNhan/CatFoodWebApp/assets/122293496/8f6f0b18-cf0b-49ba-a53a-0be413f1ff06" width="70%"/>
    <div>
      <em><b>Feature 1.</b> Home page</em>
    </div>
  </div>
  </br>
  
  <div align="center">
    <img src="https://github.com/HoTranThienNhan/CatFoodWebApp/assets/122293496/b8f464e5-0b86-4600-8830-3762fe4cdcf1" width="70%"/>
    <div>
      <em><b>Feature 2.</b> Product detail page</em>
    </div>
  </div>
  </br>
  
  <div align="center">
    <img src="https://github.com/HoTranThienNhan/CatFoodWebApp/assets/122293496/88692ca9-edb5-4245-bfe0-3bc0356b0bb5" width="70%"/>
    <div>
      <em><b>Feature 3.</b> Cart page</em>
    </div>
  </div>
  </br>
  
  <div align="center">
    <img src="https://github.com/HoTranThienNhan/CatFoodWebApp/assets/122293496/58fd6931-6abd-4ca8-b954-dcac844a364e" width="70%"/>
    <div>
      <em><b>Feature 4.</b> Order history page</em>
    </div>
  </div>
  </br>
</details>

<details open>
  </br>
  <summary><b>Admin Side</b></summary>

  <div align="center">
    <img src="https://github.com/HoTranThienNhan/CatFoodWebApp/assets/122293496/3a10e7a6-16a4-47db-bcd2-f423694f5f51" width="70%"/>
    <div>
      <em><b>Feature 5.</b> Product management page</em>
    </div>
  </div>
  </br>

  <div align="center">
    <img src="https://github.com/HoTranThienNhan/CatFoodWebApp/assets/122293496/b4731277-40f8-4bdc-bb3e-31a7c852e910" width="70%"/>
    <div>
      <em><b>Feature 6.</b> Order management page</em>
    </div>
  </div>
  </br>

  <div align="center">
    <img src="https://github.com/HoTranThienNhan/CatFoodWebApp/assets/122293496/6e4e4113-bef4-4c7c-a116-9fc7820fad0c" width="70%"/>
    <div>
      <em><b>Feature 7.</b> Order detail modal popup</em>
    </div>
  </div>
  </br>
</details>

### Members
<table>
  <tr>
    <td align="center">
        <a href="https://github.com/HoTranThienNhan">
            <img src="https://github.com/HoTranThienNhan/CatFoodWebApp/assets/122293496/e4c09ea2-8172-4ba9-9ac9-c3b3fb122d08" width="100px;" alt=""/>
            <br /><sub><b>Thien Nhan</b></sub>
          </a>
        </a>
      </td>
  </tr>
</table>

---

## Setup And Usage
### Installation and setup 
```bash
### Cloning this repository:
$ git clone --recurse-submodules https://github.com/HoTranThienNhan/CatFoodWebApp.git
$ cd CatFoodWebApp

### Installing all dependencies of each submodule:
# cat-food-front-end:
$ cd cat-food-front-end
$ npm install

# cat-food-front-end-admin:
$ cd cat-food-front-end-admin
$ npm install

# cat-food-back-end:
$ cd cat-food-back-end
$ npm install
```

### Database
``` bash
### In MongoDB Compass (localhost: 27017) shell, preparing for database and its collections:
# creating 'catfood' database if not exists
> use catfood

# creating 4 collections: products, users, orders, reviews
> db.createCollection("products")
> db.createCollection("users")
> db.createCollection("orders")
> db.createCollection("reviews")
```
To access admin website system, importing [this json file](https://github.com/HoTranThienNhan/CatFoodWebApp/files/14522468/admin-account.json) to <em>'users'</em> collection of <em>'catfood'</em> database which has already created:

```
{
  "_id": {
    "$oid": "653b49d4cbc3883700898ca2"
  },
  "name": "Admin",
  "email": "admin@gmail.com",
  "address": "Your Address",
  "phone": "0987654321",
  "password": "$2b$10$Xi7dWI4Ijn9T.yFK6ZONO.nT19XW8lnmgDZoTT9OiUoo94ZXNbtt.",
  "createdAt": {
    "$date": "2023-11-17T16:43:39.434Z"
  },
  "role": "General Manager",
  "favoriteProducts": [],
  "active": true
}
```
<details>
  <summary><b>Testing admin account infomation (for accessing admin web), click to show details</b></summary>
  <div>
    <b>Email:</b> admin@gmail.com
  </div>
  <div>
    <b>Password:</b> admin123
  </div>
  
</details>

### Run
``` bash
### Running each submodule:
# cat-food-front-end (running on localhost:3001):
$ cd cat-food-front-end
$ npm run dev

# cat-food-front-end-admin (running on localhost:3002):
$ cd cat-food-front-end-admin
$ npm run dev

# cat-food-back-end (running on port 3000):
$ cd cat-food-back-end
$ node server.js
```

