# React Meals Project Documentation

## Overview
The React Meals project is a dynamic web application that allows users to:
- Browse a selection of meals.
- View detailed descriptions.
- Add items to a cart.
- It demonstrates core React features such as component-based development, state management, and interaction handling.

## Features
- Meal Listings: Displays a list of available meals with descriptions and prices.
- Add to Cart: Allows users to add items to the cart.
- Cart Management: Provides an interface for viewing and managing the items in the cart.
- Responsive Design: Optimized for both desktop and mobile devices.

## Project Setup
Prerequisites
Ensure you have the following installed:
 - Node.js (v14 or higher)
 - npm (v6 or higher) or Yarn

## Installation

## Clone the repository:
git clone git@github.com:KundanDG52/React-meals.git

## Navigate to the project directory:
cd React-meals

## Install dependencies:
- npm install

## Start the development server:
- npm start

## File Structure 
src/
│
├── components/
- Components related to the shopping cart

│   ├── Cart/
    
- Components displaying the list of meals

│   ├── Meals/

- Generic UI components like Card, Modal

│   ├── UI/

- Main layout components like Header

│   └── Layout/

- Context API for managing global state

├── store/    

│
- Main application component

├── App.js

- Entry point for React

├── index.js

- Global styles

├── App.css

- Default React index styles

└── index.css

## Key Components
#### 1. MealItem
- Location: src/components/Meals/MealItem.js
- Description: Displays individual meal information, including name, description, and price.

#### 2. Props:
 - name (string): The meal's name.
 - description (string): The meal's description.
 - price (number): The meal's price.

#### 3. Cart
 - Location: src/components/Cart/Cart.js
 - Description: Handles cart items and total price calculations.

#### 4. Features:
 - Displays added items with quantity and total cost.
 - Allows users to remove items or adjust quantities.

#### 5. Header
 - Location: src/components/Layout/Header.js
 - Description: The main navigation bar with a cart button.
 - State Management
 - The project uses React Context API to manage the cart's state, ensuring that the cart's data is accessible across the application.

CartProvider: Wraps the application and provides cart-related state and actions.
#### 1. Actions:
 - addItem: Adds an item to the cart.
 - removeItem: Removes an item from the cart.

#### 2. Styling:
 - CSS modules are used for scoped styling.
 - Global styles are applied via App.css.

## Running Tests
To run unit tests (if included):
npm test

## Build for Production
To create a production build: 
npm run build
This will generate an optimized build in the /build folder.

## Deployment
You can deploy the app using services like Netlify, Vercel, or GitHub Pages.

## Steps for GitHub Pages Deployment
Install the GitHub Pages package: 
npm install gh-pages

Add the following to your package.json: 
"homepage": "https://<username>.github.io/<repository-name>",
"scripts": {
  "predeploy": "npm run build",
  "deploy": "gh-pages -d build"
}

## Deploy:
npm run deploy

## Potential Enhancements:
 - Add user authentication for personalized cart management.
 - Implement backend integration for fetching meals and managing orders.
 - Add a search and filter feature to browse meals easily.
