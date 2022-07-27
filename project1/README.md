### Project Developed By : 
	Bharath Kumar Raju Bairraju
	Sharvari Sanjiv Babhale
	Manukonda Harika

---------------------- Shop4Home ----------------------

Shop For Home is a popular store in the  market for shopping the home decor stuff. Due  to Covid 19 all the offline shopping stopped. So,  the store wants to move to the online platforms  and wants their own web application.

To do the above web applications there are two users:-
1.User
2.Admin

### How to run this Shop4Home project 
 1. 
	-cd ShopForHome
	-npm install

	-cd client
	-npm install  
	-( if you get any error while installing this use the following command 
	npm install react-bootstrap bootstrap --force )

 2. cd ..
 3. npm run dev
	note: both backend, frontend server and microservices will start at once with the above command.

 4. Above commands will run 
 	- project 		- port no. 3000
	- backend 		- port no. 5000
	- microsevices 	- port no. 7789

#### Database Structure: (Table: columns)

    1. categories:
			_id
			namecreatedAt
			updtaedAt 

    2. orders:  
			_id 
			status 
			products (Array) 
			transaction_id 
			amount 
			address 
			user (Object) 
			createdAt
			 updatedAt

    3. products: 
			_id 
			photo (Object) 
			sold 
			name 
			description 
			price 
			category 
			shipping 
			quantity 
			createdAt
			updatedAt

    4. users: 
			_id 
			role 
			history (Array) 
			name 
			email 
			salt
			hashed_password 
			createdAt 
			updatedAt

### App Description:
    1. user can register & sign in
    2. user can view all products
    3. user can view single product
    4. user can search products and sort products by category
    5. user can add any product to cart, checkout products by applying discount(if any) and entering delivery address
    
    6. admin can register and sign in
    7. admin can create, edit, update & delete products
    8. admin can create categories
    9. admin can view ordere history
    10.admin can view product stocks
    11. admin can give discount to any user
    12. admin can perform update, delete operations on user as well
    13. admin can use bulk upload feature by uploading a csv file
        Products can be created one by one(create product feature) or in bulk
    14. admin is able to receive an email when any product stock is less than 10.

### Tech Stack used

- Frontend-> React JS

- Backend-> Node JS & Express JS

- Database-> MongoDB

## Note
- While performing manual upload product operation try to download the image so that it will be visible on app. 
  If the images are not able to visible on app during bulkupload that means the images are not there in the folder.i.e,(public -> images)
- The mail functionality will only work if the products are less than 10 , If you use buy operation in user , then  login as admin to recieve the mail because when the admin is loged in only then he will receive mail of stocks which are less than 10.
- User and Admin validation is done,so while performing sign uo operation enter proper details 

