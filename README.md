# D3.js Pizza Visualization

This project is an interactive pizza maker built with D3.js. Users can create their own custom pizza by adding a base of sauce and cheese, a variety of toppings, and some finishing touches. Once the pizza is complete, the user can "cook" the pizza to view a detailed breakdown of its nutritional information and a bar chart showing the distribution of the added toppings.

## Live Demo

You can try it out here: [https://sjessicameyer.github.io/a1-ghd3/](https://sjessicameyer.github.io/a1-ghd3/)

## Screenshots

![Screenshot of the Pizza Visualization](./Screenshot%202026-01-17%20at%204.44.16%E2%80%AFPM.png)

![Screenshot of the Nutritional Visualization](./Screenshot%202026-01-17%20at%204.47.12%E2%80%AFPM.png)

## Technical Achievements

*   **Interactive D3.js Visualization:** The entire pizza and its toppings are dynamically generated and rendered as SVG elements using D3.js.
*   **Data-Driven Elements:** Toppings are added based on user interaction, with their positions and rotations randomized to create a unique and organic-looking pizza every time.
*   **DOM Manipulation:** D3 is used for all major DOM manipulations, including event handling, managing UI state (switching between pizza-making and stats screens), and clearing/resetting the visualization.
*   **Dynamic Stats Calculation:** Nutritional information is calculated in real-time based on the number and type of toppings added by the user.
*   **D3 Charting:** A bar chart is generated using D3 scales (`scaleBand`, `scaleLinear`) and axes (`axisBottom`, `axisLeft`) to visualize the distribution of toppings on the final stats screen.
*   **Performance Optimization:** Button clicks are throttled using a custom `throttle` function to prevent users from overwhelming the DOM with too many elements at once, ensuring a smooth experience.

## Design Achievements

*   **Intuitive UI/UX:** The interface is clean, simple, and organized into logical steps (Base, Toppings, Finish). Bootstrap is used for a responsive layout.
*   **Engaging Visuals:** Emojis and custom image icons are used for the controls, making the experience more fun and visually appealing. The classic red-and-white checkerboard background evokes a pizzeria aesthetic.
*   **Clear User Feedback:** Interactive elements have hover effects, and buttons are temporarily disabled after a click to provide clear feedback to the user.
*   **Two-Phase Experience:** The application is split into two distinct phases: a creative "building" phase and an informative "summary" phase, which provides a satisfying conclusion to the user's interaction.
*   **Informative Summary:** The final stats screen presents data in two effective ways: a numerical list for precise nutritional facts and a bar chart for an at-a-glance comparison of topping quantities.
