Role-Based Authentication Module - Frontend
Description
This frontend project is built using React to provide a user interface for the Role-Based Authentication (RBAC) system. It enables users to register, log in, and access different dashboards based on their roles (Admin, User).

Features
User login and registration forms.
Axios for API requests to the backend.
Conditional rendering of components based on user roles.
Admin Dashboard with additional controls.
User Dashboard with standard features.
Proper error handling for restricted access.

# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)

Installation
Prerequisites
Node.js (v14 or later)
npm (Node Package Manager)
npm install is the command to install all the packages
Steps to Set Up
Create a new React application (if not already created):
npx create-react-app rbac-frontend
cd rbac-frontend
Clone the repository:
git clone https://github.com/your-username/OJT_Task1.git
cd OJT_Task1
git checkout frontend
Install Axios for API requests:
npm install axios
Usage:
To start the React application:

npm start
Access the application at http://localhost:3000.
Login: Users can log in using their credentials.
Register: New users can create an account.
Environment Variables:
Update the API base URL in your Axios configuration file to point to your backend server.
For example, in src/authService.js, set: const API_URL = "http://localhost:8080/auth/";
Deployment:
install the gh-pages package
The package allows us to publish build files into a gh-pages
npm install gh-pages --save-dev
configure the package.json file so that we can point our GitHub repository to the location where our React app will be deployed.
add predeploy and deploy scripts to the package.json file.
"predeploy" : "npm run build",
"deploy" : "gh-pages -d build",
git add .
git commit -m "setup gh-pages"
git push
npm run deploy
Contributions:
-Fork the repository.

Create a new branch for your feature or bug fix.
Commit your changes and push to your branch.
Create a pull request.
License:
This project is licensed under the MIT License
