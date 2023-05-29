  <h1>Project Structure</h1>
<h2>
Table of Contents</h2>
<li><a href="#src">/src</a></li>
  <ul>
    <li><a href="#assets">/assets</a></li>
    <li><a href="#components">/components</a></li>
    <li><a href="#constants">/constants</a></li>
    <li><a href="#services">/services</a></li>
    <li><a href="#pages">/pages</a></li>
    <li><a href="#store">/store</a>
    <ul>
        <li><a href="#actions">/actions</a></li>
        <li><a href="#reducers">/reducers</a></li>
        <li><a href="#selectors">/selectors</a></li>
        <li><a href="#middlewares">/middlewares</a></li>
    </ul>
    </li>
    <li><a href="#styles">/styles</a></li>
    <li><a href="#utils">/utils</a></li>
    <li><a href="#tests">/tests</a></li>
    <li><a href="#performance">/performance</a>
    <ul>
        <li><a href="#metrics">/metrics</a></li>
        <li><a href="#reports">/reports</a></li>
        <li><a href="#middlewares">/middlewares</a></li>
    </ul>
    </li>
    <li><a href="#app">app.jsx</a></li>
    <li><a href="#index">index.jsx</a></li>
  </ul>

<hr/>
<br/>

<h1>Description:</h1>

<h2 id="src"><Strong>/src :</strong></h2>
    <p>The /src directory is the main directory of the project, housing all the source code for the application. It serves as the root directory for organizing and managing various files and directories.</p>
    <ul>
        <h2 id="assets">/assets :</h2>
            <p>The <strong>'/assets'</strong> directory is used to store images, fonts, and other static assets required by the application. It provides a central location for managing and accessing these assets. For example, you can store <strong>'logo.png'</strong>, <strong>'font.ttf'</strong>, or <strong>'background.jpg'</strong> files in this directory and use them throughout your application.</p>
        <h2 id="components">/components :</h2>
            <p> The <strong>'/components'</strong> directory contains reusable UI components that can be utilized across different parts of the application. It promotes code reusability, reduces redundancy, and ensures consistent user interface elements. For instance, you might have a Button component that can be used in multiple places like forms, headers, or navigation bars.</p>
        <h2 id="constants">/constants :</h2>
            <p> The <strong>'/constants'</strong> directory is used to store constant values that are utilized throughout the application. It helps centralize the management of these values and provides a single source of truth. For example, you can define constants such as API endpoints, error messages, or configuration settings in separate files like <strong>'apiEndpoints.js'</strong>, <strong>'errorMessages.js'</strong>, or <strong>'config.js'</strong>.</p>
        <h2 id="services">/services :</h2>
            <p>The <strong>'/services'</strong> directory contains API services and utility functions that handle API calls and perform other related tasks. It provides a structured approach to encapsulate API-related logic and keeps it separate from the components. For example, you might have a <strong>'userService.js'</strong> file that encapsulates functions like <strong>'getUser()'</strong> or <strong>'updateUser()'</strong> which handle API calls related to user data.</p>
        <h2 id="pages">/pages :</h2>
            <p>The <strong>'/pages'</strong> directory houses the top-level pages of the application. Each page represents a distinct view or route in the application. It helps organize the codebase by separating different pages and their associated components and logic. For example, you can have files like <strong>'HomePage.js'</strong>, <strong>'AboutPage.js'</strong>, or <strong>'ContactPage.js'</strong> representing different pages of your application, each with their own unique functionality and UI components.</p>
        <h2 id="store">/store :</h2>
            <p>The <strong>'/store'</strong> directory is responsible for setting up and configuring the Redux store, which manages the application state. It follows the Redux architecture pattern, separating actions, reducers, selectors, and middlewares into their respective subdirectories. This structure promotes maintainability, scalability, and separation of concerns.</p>
            <ul>
            <h3 id="actions">/actions :</h3>
                <p>The <strong>'/actions'</strong> directory contains Redux action creators, which are functions that create actions to update the Redux store. For example, you might have an <strong>'userActions.js'</strong> file that defines actions like <strong>'fetchUser()'</strong> or <strong>'updateUser()'</strong>.</p>
            <h3 id="reducers">/reducers :</h3>
                <p> The <strong>'/reducers'</strong> directory contains Redux reducers, which specify how the state should change in response to actions. They handle updating the state based on the dispatched actions. For example, you might have a <strong>'userReducer.js'</strong> file that handles state changes related to user data.</p>
            <h3 id="selectors">/selectors :</h3>
                <p> The <strong>'/selectors'</strong> directory includes Redux selectors, which are functions that extract specific pieces of state from the Redux store. They help in accessing and deriving derived state from the store. For example, you might have a <strong>'userSelectors.js'</strong> file that extracts user-related data, such as the current user or user list, from the state.</p>
            <h3 id="middlewares">/middlewares :</h3>
                <p> The <strong>'/middlewares'</strong> directory contains custom Redux middlewares, which intercept actions before they reach the reducers. Middlewares provide a way to add custom logic or side effects to the Redux flow. For example, you might have a middleware that logs actions or handles asynchronous API calls.</p>
            </ul>
        <h2 id="styles">/styles :</h2>
            <p>The <strong>'/styles'</strong> directory is used for managing global styles and CSS modules used in the application. It provides a central location to define and organize styles, ensuring consistency and ease of maintenance. For example, you can have a <strong>'global.css'</strong> file for global styles and separate CSS modules for each component.</p>
        <h2 id="utils">/utils :</h2>
            <p> The <strong>'/utils'</strong> directory includes utility functions and helpers that are used throughout the application. These functions provide common functionality, reusable code snippets, and help avoid code duplication. For example, you might have utility functions for date formatting, string manipulation, or data validation that can be used across multiple components and modules.</p>
        <h2 id="tests">/tests :</h2>
            <p> The <strong>'/tests'</strong> directory is dedicated to unit tests and integration tests for the application. It helps ensure the correctness and reliability of the codebase by automating testing processes. For example, you can have test files like <strong>'userActions.test.js'</strong> or <strong>'HomePage.test.js'</strong> to test the functionality of specific modules or components.</p>
        <h2 id="performance">/performance :</h2>
            <p>The <strong>'/performance'</strong> directory contains files related to performance monitoring. It focuses on measuring and optimizing the application's performance.</p>
            <ul>
            <h3 id="metrics">/metrics :</h3>
                <p>The <strong>'/metrics'</strong> directory includes setup and configuration files for performance monitoring metrics. It helps track and measure various performance-related metrics, such as response times or memory usage. For example, you might have a configuration file for a tool like Google Analytics or New Relic to collect performance metrics.</p>
            <h3 id="reports">/reports :</h3>
                <p>The <strong>'/reports'</strong> directory is used to store generated performance reports. These reports provide insights into the application's performance, identifying areas for improvement and optimization. For example, you might have reports that analyze the loading times of different pages or the efficiency of certain API calls.</p>
            <h3 id="performance-middlewares">/middlewares :</h3>
                <p> The <strong>'/middlewares'</strong> directory contains middleware specifically designed for performance monitoring. These middlewares can intercept and analyze performance-related data during runtime. For example, you might have a middleware that measures API response times and logs them for analysis and optimization.</p>
            </ul>
        <h2>Other Files</h2>
            <ul>
                <li><strong>App.js</strong> - App.js typically contains the main component that represents the root of the application, defining the overall structure and layout.</li>
                <li><strong>index.js</strong> - index.js is responsible for rendering the application into the DOM, initializing the app and its dependencies. These files are essential for the proper functioning and rendering of the application.</li>
            </ul>
