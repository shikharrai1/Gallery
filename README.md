# PicGallery - React Pagination App

A dynamic image gallery built with **React** that fetches data from the [Lorum Picsum API](https://picsum.photos/). This project demonstrates efficient state management, API handling with Axios, and a custom pagination system.

##  Features

* **Asynchronous Data Fetching:** Uses `Axios` and `async/await` to retrieve image data.
* **Dynamic Pagination:** Navigate through hundreds of images using "Next" and "Prev" buttons.
* **Conditional Rendering:** Includes a "Loading..." state while fetching new data.
* **Responsive Design:** Built with **Tailwind CSS** for a clean, mobile-friendly grid layout.
* **Interactive Components:** Individual `Card` components that link directly to the source image.

## Tech Stack

* **Frontend:** React.js
* **Styling:** Tailwind CSS
* **Data Fetching:** Axios
* **API:** Picsum Photos API

## Key Concepts Implemented

### 1. Hooks (useState & useEffect)

The app manages two primary states: `userData` for storing the API response and `index` for tracking the current page. The `useEffect` hook is configured with `[index]` as a dependency to trigger a fresh API call whenever the page changes.

### 2. Component Communication (Props)

Data is passed from the main `App` component to the `Card` component using **Props**. This keeps the code modular and reusable.

### 3. Virtual DOM Updates

By updating state, React triggers the reconciliation process to update only the parts of the DOM that changed (the gallery grid and page number), ensuring a smooth user experience.

##  Installation & Setup

1. **Clone the repository:**
```bash
git clone < url from github >

```


2. **Install dependencies:**
```bash
npm install

```


3. **Start the development server:**
```bash
npm run dev

```



## Component Structure

```text
src/
├── components/
│   └── Card.jsx    # Displays individual image, author, and link
├── App.jsx         # Main logic, state management, and pagination
└── main.jsx        # Entry point

```
