# Next.js Data Fetching Error: Invalid JSON Return

This repository demonstrates a common error in Next.js applications involving the `getStaticProps` or `getServerSideProps` functions.  The issue arises when these functions return data that is not correctly formatted as a JSON object, causing unexpected errors during the build or runtime.

## Bug
The `bug.js` file shows an example where the function returns a primitive value (a string) instead of a JSON object. This leads to a failure in the Next.js build process.

## Solution
The `bugSolution.js` file provides a corrected version where the data is properly wrapped within a JSON object, ensuring successful data fetching and rendering.

## How to Reproduce
1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm run dev` to start the development server.
4. Observe the error in the console (for `bug.js`) and the successful rendering (for `bugSolution.js`).

This example highlights the importance of carefully structuring the data returned from `getStaticProps` and `getServerSideProps` to avoid common errors in Next.js development.