# Optimizing React code for speed can involve several techniques, here are a few that you can consider:

Reduce the number of renders: Each time a component is re-rendered, it takes some processing time. Make sure you are not re-rendering unnecessarily. You can use React.memo() or shouldComponentUpdate() to optimize this.

Use React's built-in Profiler: React's profiler can help you identify performance bottlenecks in your application. It can tell you which components are taking the most time to render and how many times they're being rendered. You can use this information to optimize your code.

Use a virtualized list: If you're rendering a long list of items, consider using a virtualized list. A virtualized list only renders the items that are currently visible on the screen, which can greatly improve performance.

Use lazy loading: If your application has a lot of components, consider using lazy loading. Lazy loading only loads the components that are needed, which can improve the initial load time of your application.

Optimize images: Large images can take a long time to load and slow down your application. Consider optimizing your images by compressing them or using lazy loading techniques.

Use useMemo() or useCallback(): If you have expensive calculations or functions that are used in your components, consider using useMemo() or useCallback() to memoize the results. This can greatly improve performance by preventing unnecessary re-calculations.

Avoid unnecessary DOM manipulation: Manipulating the DOM can be expensive. Try to avoid making unnecessary DOM manipulations by using React's state and props to update your components.

Use the production build: When you're ready to deploy your application, make sure you're using the production build of React. The production build is optimized for performance and has fewer warnings and debugging features.

Use Web Workers: If you have long-running processes that are blocking the main thread, consider using Web Workers to move that processing to a separate thread. This can greatly improve performance by preventing the UI from freezing.

Use Code Splitting: If your application has a lot of code, consider using code splitting to split your code into smaller chunks. This can improve the initial load time of your application by only loading the code that's needed.

Use a CDN: If you're serving your assets from your own server, consider using a CDN (Content Delivery Network) to serve your assets. A CDN can improve the load time of your application by caching your assets and serving them from a server closer to the user.

Use CSS Transitions and Animations: If you're animating elements on your page, consider using CSS transitions and animations instead of JavaScript. CSS animations are often more performant than JavaScript animations.

Minimize the number of HTTP requests: Each HTTP request takes time to process and can slow down your application. Minimize the number of HTTP requests by combining your CSS and JavaScript files, and by using image sprites instead of individual images.

Use memoized selectors: If you're using a state management library like Redux, consider using memoized selectors to optimize your selectors. Memoized selectors can prevent unnecessary re-renders by only re-calculating the results when the input data changes.

# Course Code & Materials

This repository contains the course source code and other extra materials like slides.

## How to use

The code snapshots are organized in multiple **branches** where every branch **represents a course section**.

For example, the branch [01-getting-started](https://github.com/academind/react-complete-guide-code/tree/01-getting-started) holds all code snapshots and extra materials for section 1 of the course ("Getting Started").

You can switch branches via the branch dropdown above the directory explorer.

![Click on the branch dropdown and then select the appropriate branch for the course section you're looking for](./selecting-a-branch.jpg)

In most branches, you'll find multiple folders which organize the section-specific content further:

- Often, you'll find a `/code` subfolder which contains any relevent code snapshots for the given course section
- You also often find `/slides` folders which - guess what - contain the slides for the module
- `/extra-files` typically contains extra files like `.css` files that might be attached to individual lectures in that course module

The folder names should generally be self-explanatory but also feel free to simply click around and see which materials are available.

## Using code snapshots

Code snapshots (which you find in `/code`) are there for you to compare your code to mine and find + fix errors you might have in your code.

You can either view my code directly here on Github (you can open + view code files without issues here) or you download the snapshots.

The subfolders in the `/code` folder are named such that mapping them to the course lectures is straightforward.

### Downloading code snapshots

You can download all the content of a branch via the "Code" button here on Github. You can then either [clone](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository) the repository or simply download the selected branch content as a ZIP file.

**Important:** You always download the **entire branch content!**

You can then dive into the interesting folders (e.g. the individual code snapshots) locally on your hard drive.

### Running the attached code

You can use the attached code simply to compare it to yours. But you can also run it.

To run my code, navigate into a specific code snapshot folder via the `cd` command in your command prompt or terminal first.

Then run `npm install` to install all required dependencies (this will create a `/node_modules` folder).

**Important:** If you're using the code for a module that requires API keys or a backend (e.g. the module about sending Http requests), you'll have to use **your backend URLs** or API keys. Mine won't work (I disabled my projects).
