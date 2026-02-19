# Personal-Finance-Dashboard
Full Stack Personal Finance Web App
This is a personal finance application that allows users to link their bank account via the Plaid API. Current functionality includes basic authentication via JSON Web Token, and the addition, deletion, and refreshing of a bank account. The application will display the user's account balances and transactions. Note that this project is a work in progress - more features are planned to be implemented in the future.

Setup

1) git clone https://github.com/jagodin/personal-finance-app
2) cd personal-finance-app
3) npm install
4) npm run dev to run the development environment.


Obtain your Plaid API keys from here and set up a MongoDB database

Configure ./config/default.json

{
    "mongoURI": "YOUR_MONGO_URI",
    "jwtSecret": "YOUR_SECRET_TOKEN"
}


Technologies

1)Node.js

2)React

3)Redux

4)MongoDB

5)Express.js

6)Material UI

Packages

1)Axios

2)Express Validator

3)JSON Web Token

4)Redux Thunk

5)Bcrypt.js

6)Mongoose

Screenshots
Login/Registration Page
<img width="1035" height="500" alt="Screenshot (126)" src="https://github.com/user-attachments/assets/9114b313-af0d-465a-9d71-95060d736e05" />
Dashboard and Profile Menu
<img width="1824" height="854" alt="Screenshot (132)" src="https://github.com/user-attachments/assets/46f1e8f5-74f7-47b0-9941-adb722fd2112" />
Linked Accounts and Balances 
<img width="1804" height="842" alt="Screenshot (133)" src="https://github.com/user-attachments/assets/e98b1ecc-7066-472d-a436-1a894ce78562" />
Transactions
<img width="1765" height="862" alt="Screenshot (134)" src="https://github.com/user-attachments/assets/aabe79b1-a6d3-4427-9c74-43c6806c93e7" />
Plaid Link 
<img width="1818" height="841" alt="Screenshot (135)" src="https://github.com/user-attachments/assets/ec9041be-0308-46ea-bd4d-f9b3fb051a5f" />
Responsive Dashboard 
<img width="873" height="799" alt="Screenshot (136)" src="https://github.com/user-attachments/assets/69c38682-7b0a-4573-9387-fcc8d7c95b27" />

Future Enhancements

Implement budgets and categorize transactions into appropriate budget.
Add user settings (i.e. UI preferances).
Give users the ability to report application issues via the Support page.
Implement FAQ.
Responsive UI enhancements.
Implement cache to prevent user's from overloading the backend and Plaid API.
Implement Google Firebase Authentication.

Disclaimer
Note that the application exposes the user's access_tokens and item_ids to the client. For production releases, these must be securely persisted to your database and never exposed to the client.

From the Plaid API documentation:
access_tokens and item_ids are the core identifiers that map your end-users to their financial institutions. You should persist these securely and associate them with users of your application. Make sure, however, that these identifiers are never exposed client-side. Keep in mind that one user can create multiple Items if they have accounts with multiple financial institutions.








