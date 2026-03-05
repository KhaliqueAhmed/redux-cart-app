# Redux Cart App

A simple shopping cart application built with **React** and **Redux Toolkit**.

## Features

- View a static product list
- Add products to cart
- Remove products from cart
- Live total price calculation
- Global state management with Redux Toolkit

## Tech Stack

- React
- Redux Toolkit
- React Redux
- Create React App (react-scripts)

## Project Structure

```
redux-cart-app/
├─ public/
├─ src/
│  ├─ app/
│  │  └─ store.js
│  ├─ components/
│  │  ├─ Cart.js
│  │  └─ ProductList.js
│  ├─ features/
│  │  └─ cart/
│  │     └─ cartSlice.js
│  ├─ App.js
│  └─ index.js
├─ package.json
└─ README.md
```

## Getting Started

### Prerequisites

- Node.js (v18+ recommended)
- npm

### Installation

```bash
npm install
```

### Run Development Server

```bash
npm start
```

App runs at: `http://localhost:3000`

## Available Scripts

- `npm start` — start development server
- `npm test` — run tests in watch mode
- `npm run build` — create production build
- `npm run eject` — eject CRA config (one-way operation)

## How It Works

- `ProductList` dispatches `addItem(product)`
- `Cart` reads state using `useSelector`
- `Cart` dispatches `removeItem(id)`
- Total is calculated using `reduce()` over cart items

## Future Improvements

- Prevent duplicate cart entries or add quantity support
- Persist cart data in `localStorage`
- Add product API integration
- Improve UI styling and responsiveness
