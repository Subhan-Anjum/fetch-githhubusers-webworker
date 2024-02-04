# Fetching Data in a Worker

This project demonstrates fetching data from GitHub using Web Workers in JavaScript. It allows users to input a GitHub username and fetch information about their profile, followers, and repositories.

## Live Preview

You can view a live preview of this project [here](https://fetch-githhubusers-webworker.netlify.app/).

## How to Run

To run this project locally, follow these steps:

1. Clone this repository to your local machine:

    ```bash
    git clone https://github.com/Subhan-Anjum/fetch-githhubusers-webworker.git
    ```

2. Navigate to the project directory:

    ```bash
    cd fetch-githhubusers-webworker
    ```

3. Open the `index.html` file in a web browser.

## Usage

- Enter a GitHub username in the input box.
- Click the "Run with Worker" button to fetch data using a Web Worker.
- Click the "Run without Worker" button to fetch data without using a Web Worker.

## File Structure

- `index.html`: HTML file containing the structure and interface of the project.
- `style.css`: CSS file containing styles for the HTML elements.
- `worker.js`: JavaScript file containing the Web Worker code for fetching data.

## Technologies Used

- HTML
- CSS
- JavaScript

## Performance Improvements with Web Workers

Using Web Workers for fetching data can provide significant performance improvements by offloading tasks to separate threads, thus preventing UI blocking. This allows for smoother user experience, especially when dealing with heavy computational tasks or asynchronous operations like network requests.

## Challenges Faced and Solutions
1. Managing Worker Communication:
   One challenge was managing communication between the main thread and the Web Worker. This was overcome by using the postMessage API to send and receive messages between threads.

2. Handling CORS Issues:
    Another challenge was dealing with Cross-Origin Resource Sharing (CORS) issues when fetching data from external APIs. This was addressed by either configuring the server to allow CORS or using a proxy server to bypass CORS restrictions.

## References and Resources
MDN Web Docs - Web Workers
Web Workers API: Speed Up Your Web Apps with Web Workers
Using Web Workers to Speed Up Your JavaScript Applications
Handling CORS Issues: A Complete Guide

## Contributors

- [Subhan Anjum](https://github.com/Subhan-Anjum)

