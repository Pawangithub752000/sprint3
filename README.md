#Problem Statement
Create the following App using the Provided Boilerplate
Note: Make sure you start json-server on 8080 port with provided db.json file, then only you will be able to see data on this website.

You can also take a look at this video : https://drive.google.com/file/d/184D4GJKONn1SMmWNRWC5Br7ELrz_ZedQ/view

Getting Started
Fork this repository https://github.com/abduljabbarpeer/sprint3.git
Clone the Forked repository. Note: This Clone repository should be on your github account.
navigate to the folder cd sprint3
npm install
npm start
Make sure your json-server is running on port 8080, db.json file is provided.
Note: Libraries are not installed, you need to install react-router-dom and any other additional library yourself.

You can also take a look at this video : https://drive.google.com/file/d/184D4GJKONn1SMmWNRWC5Br7ELrz_ZedQ/view

Components Structure :
├── App.js
   ├── Navbar.jsx
   ├── Home.jsx // Protected/Private Route - Only access when user logs in
   |   |── Products.jsx
   |        ├── ProductItem.jsx
   |
   └── Login.jsx // Public Route
Note : Make sure you use only the given components and don't create new files and folders. It is really important.

Understanding Data Structure
db.json
Initial Products should be fetched using json-server only after user logs in.
cartItems has following operations, accessible post login
Add
Delete
Update Count
Note - Make sure you use only the given data and don't create new data.

What needs to be done from your end ?
Navbar :
In Login Page : It should contain HOME and LOGIN Link. Number of items in the cart should not be visible

In Home Page : It should contain HOME link and count of all items in the cart and a logout button. logout button logs user out ( Remember this can be done by modifying the authentication status )

Login Page:
App should redirect to /login : Login page as soon as he visits the / : Home Url.
User will enter his email and password. There should be two input boxes for email and password entry and a button which will make login request. You will be using reqres.in api for this. Refer Docs ( https://reqres.in/ ). Upon successful login; user will be redirected to Home Page /.
Authentication status should be maintained in AuthContext (context provider). whenever component needs the authentication status; it should be sent from context api and that component should be able to receive it and if required modify it. ( for example : authentication status gets modified post successful login )
Home Page :
products and cartItems should be fetched and populated at required places;

List all the products.

Each Individual product card should contain the product name, product description and

Add to Cart button : User Should be able to Add product to cart, if that product is not already existing in /cartItems. Disable the button if item already exists in cart.
Increment button: increment Cart Item Count by Matching Product ID. disable if item does not exists in cart yet
Decrement button: decrement Cart Item Count by Matching Product ID. disable if item does not exists in cart yet. if the count is 1 and decrement is clicked. the item should be completely removed from cart.
There should be a text section which would tell the quantity of that particular item in the cart. if that item does not exist in cart showcase message stating Not Added to Cart
Remove button : disable if item does not exists in cart yet. Clicking on this would delete the item from the cartItems altogether.
cartItems should be maintained in cartContext context API and whenever component needs the cart items info; it should be sent from context api and that component should be able to receive it. Also changes like increment, decrement and removal done here should be reflected in db.json( i.e., POST, GET, PUT/PATCH, DELETE ) requests should also be made accordingly.
General Instructions :
Use styled components for styling purposes ( do not use inline styling or global css )
Make sure you use only the given components and don't create new files and folders. This is really important
Use the given data and do not create new /product data. or change it.
You'll have to deploy the app to netlify and submit us the link ( there is a prob given for this to submit netlify link ). so make sure that you have an account with netlify. (as netlify takes down your app in few days if your account does not exist)






- fork the repository

- clone the forked repository

```
git clone <git_url>
```

```
cd sprint3
```

```
npm install
```

only core ( whatever cra offers ) libraries have been installed. If you want to use any other library. You'll have to install it.

Example : If you need `react-router-dom` library; please install it.

---
