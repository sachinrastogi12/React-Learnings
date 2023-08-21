# React-Learnings

Just documenting my learnings in a question answer format so that anyone can understand step by step apporach to learn it.

### What is bundlers?
 
In simple terms, bundlers are tools that take all your code files (like JavaScript, CSS, images) and package them together into a smaller number of files that your web browser can easily understand and load.

Let's break it down with an example:

Imagine you're building a React app. You've written multiple JavaScript files, each containing different components and functions. You also have CSS files for styling and images to show. When it comes to actually showing your app in a web browser, it's inefficient to load all these files individually – it could slow down your app's performance.

Here's where a bundler, like Webpack, comes in. It takes all those separate files, processes them, and combines them into a few optimized files. So, instead of the browser having to download many separate files, it only needs to download a couple of bundled files. This speeds up the loading time and makes your app run smoother.

Let's say you have an example React app with three components: `Header`, `Sidebar`, and `MainContent`. You've also written some CSS styles and used a logo image. With a bundler, your files might be organized like this:

1. `index.js` - Your main JavaScript file that imports and renders your components.
2. `Header.js`, `Sidebar.js`, `MainContent.js` - Individual React component files.
3. `styles.css` - File containing your CSS styles.
4. `logo.png` - Your logo image.

The bundler would take these files, process them, and create something like:

- `bundle.js` - A single JavaScript file that includes all your component code.
- `bundle.css` - A single CSS file with your styles.
- `assets/` - A folder with optimized image files.

Then, in your HTML file, you'd only need to link to the `bundle.js` and `bundle.css` files, and the bundler will handle the rest.

This bundling process helps your app load faster and keeps it organized, even if you have many different code and asset files. It's like packing all your belongings into a suitcase for a trip, so you don't have to carry many separate bags.

Remember, there are different bundlers available, and Webpack is just one example. They all serve the purpose of optimizing your code for web delivery.