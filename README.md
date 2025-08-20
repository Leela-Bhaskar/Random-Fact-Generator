# Vue Random Fact Generator

A simple and clean web application built with Vue.js that fetches and displays a random useless fact from a public API.

![Screenshot of the Vue Random Fact Generator](https://placehold.co/600x400/6366f1/ffffff?text=Random+Fact+App+UI)

---

## 🚀 Features

-   **Fetch Random Facts:** Click a button to get a new random fact.
-   **Loading State:** A spinner indicates when a fact is being fetched from the API.
-   **Error Handling:** Displays a user-friendly message if the API call fails.
-   **Responsive Design:** The layout is fully responsive and looks great on desktops, tablets, and mobile devices.
-   **Dark Mode:** Styled for both light and dark mode based on your system preference.

---

## 🛠️ Technologies Used

-   **HTML5:** The core structure of the web page.
-   **Vue.js (v3):** A progressive JavaScript framework for building the user interface.
-   **Tailwind CSS:** A utility-first CSS framework for rapid and responsive styling.
-   **Useless Facts API:** The public API used to source the random facts.

---

## 🏁 Getting Started

This project is a single, self-contained HTML file, so there's no need for a complex setup or build process.

1.  **Clone the repository (optional):**
    ```bash
    git clone [https://github.com/your-username/vue-fact-generator.git](https://github.com/your-username/vue-fact-generator.git)
    ```
2.  **Navigate to the project directory:**
    ```bash
    cd vue-fact-generator
    ```
3.  **Open the `index.html` file:**
    Simply open the `index.html` file in your favorite web browser (like Chrome, Firefox, or Safari) to run the application.

---

## ⚙️ How It Works

The application is initialized using the global Vue 3 build.

-   **`data()`:** The component's state is managed by three properties:
    -   `fact`: Stores the fact text fetched from the API.
    -   `isLoading`: A boolean that controls the visibility of the loading spinner.
    -   `error`: Stores any error messages if the API call fails.
-   **`getFact()` method:** This `async` method is triggered when the "Get New Fact" button is clicked. It handles:
    1.  Setting `isLoading` to `true`.
    2.  Making a `fetch` request to the Useless Facts API.
    3.  Parsing the JSON response and updating the `fact` data property.
    4.  Catching any potential errors and updating the `error` property.
    5.  Setting `isLoading` back to `false` once the request is complete.

---


This project is powered by the [Useless Facts API](https://uselessfacts.jsph.pl/).
