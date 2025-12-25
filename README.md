# Intro to ReactJS

**Definition/Overview:** ReactJS was developed by Facebook (now *Meta*) as a client-side JavaScript (JS) library. It is utilized by developers to build *single-page apps* and customize interactive user interfaces (UIs) via highly reusable and flexible web *components*. The relatively light learning curve (in comparison to a heavier JS framework, such as AngularJS) of ReactJS assists in optimizing UIs and their associated User Experience (UX) potential.
  
ReactJS also utilizes a JavaScription syntax extension known as JavaScript XML, or 'JSX'. It combines JS and HTML scripting within individual files.

#### Table of Contents

1. ['Hello World' Code Example](#hello-world)
2. [Components and Elements Overview](#components-and-elements)
3. [React Component Lifecycle](#component-life-cycle)
4. [Optimization and Pitfalls](#optimization-and-pitfalls)
5. [Next.js](#nextjs)
6. [ReactJS vs. Angular vs. Vue.js](#rav)
7. [Supplemental Resources](#supplemental)
  
<hr />

## <a name="hello-world">1. 'Hello World' Code Example</a>

```
// projects/HelloWorldApp.jsx
import React from 'react';

function HelloWorldApp() {
  return (
    <div>
      <h1>Hello World!</h1>
    </div>
  );
}

export default HelloWorldApp;
```

<hr />

## <a name="components-and-elements">2. Components and Elements Overview</a>
  
**What exactly are 'components'?:** A ReactJS component is a piece of code that can be reused throughout an application. There are many possibilities for what ReactJS components can be--buttons, textboxes, and text headings, for example. This reuse of code slices allows for apps to be developed quicker and perform faster.
  
**What about 'single-page apps'?:** Simply put, these are apps in which clicking on elements, such as navigation menu items and various links, does not result in reloading of the app as a whole. Instead, *the only reloaded content is the body of the freshly requested section*. For an example of this, consider a movie and/or television streaming service, such as Hulu or Netflix. The use of a single-page app system allows for users to watch their streaming media content without reloading entire pages.
  
<hr />
  
## <a name="component-life-cycle">3. React Component Lifecycle</a>
  
React components undergo three core phases from the time of their creation to being discarded from the Document Object Model (the DOM, which is the interface that provides a representation of HTML/XML documents). These phases assist with performance optimization, side effect handling, and controlling component behaviors.

| Phase | Explanation | Class Components | Functional Components |
| :---: | :---: | :---: | :---: |
| **Mounting Phase** | Initiated at the time that a component is created and initially inserted into the DOM. | Rely on methods (e.g., constructor(), render(), componentDidMount()). | Rely on render and useEffect hook for handling mounting. |
| **Updating Phase** | Happens when component states or props update, causing the component to be rendered again. | Rely on methods (e.g., shouldComponentUpdate(), render(), componentDidUpdate()). | Rely on the useEffect hook and various dependencies, in response to updates of component state and props. |
| **Unmounting Phase** | Happens in response to a component being discarded from the DOM. | Rely on the componentWillUnmount() method being called prior to the component being discarded, so that components can be properly cleaned up or reset (e.g., discarding event listeners, resetting timers). | Rely on the useEffect hook for cleaning at the time of the component being unmounted. |

<hr />
  
## <a name="optimization-and-pitfalls">4. Optimization and Pitfalls</a>
  
**How is ReactJS Optimized?:** Some of the ReactJS features and techniques that benefit UI/UX developers include...
  
<br />

| Feature | Explanation |
| :---: | :---: |
| **Debouncing and Throttling** | This limits when functions execute, and how often. |
| **Functional Pattern Adherence** | This assists in handling complex code/logic, potentially reducing errors and increasing performance. |
| **Lazy Loading** | This limits component loading to only when it is needed. |
| **List Virtualization** | This limits the rendering of list items to only when they are available on screen to users. |
| **Memoization** | This caches responses for future re-use, increasing performance when serving clients web assets. Consider using memoization tools such as *useMemo* and *React.memo*. |
| **useReducer() and useTransition() Hook Leveraging/Utilization** | useReducer() defines how states are to be updated. useTransition() limits updates until when they are needed, potentially increasing performance. |

<br />

**Common Mistakes in ReactJS Development include:**  
  
<br />

| Error | Why It Is Bad |
| :---: | :---: |
| **Forgetting to Use Keys in Lists** | Keys detect added, modified, and removed items. |
| **Imprecise Component Structure** | If logic is spread across components, updating/maintaining components and component reuse can become a mess. |
| **Mutating State Directly** | This can cause errors and other unintended behaviors. Thus, it is better practice to update state immutably. |
| **Overlooking Performance Optimization Techniques** | This includes the principles outlined in the above section. |
| **Overreliance on Inline Functions** | This can cause extraneous rerendering, and therefore unnecessary performance costs. |
   
<hr />
  
## 5. <a name="nextjs">Next.js</a>
  
While ReactJS is a JavaScript library utilized by app developers to build interactive UIs via reusable (and highly flexible) components, *Next.js* is a specific ReactJS-based framework that directly provides extra, built-in functionalities (e.g., API routes, CSR, SSG, SSR) for optimizing full-stack development. Thus, high performance app rendering is more readily provided by Next.js, while native ReactJS mostly relies on client-side rendering and would need libraries to be imported and configured to achieve Next.js's built-in extra functionalities.
  
**Use Case:** *ReactJS* without Next.js may be a more practical option for developing single-page apps that require UI components for interactive, dynamic, or otherwise complex purposes, while *Next.js* integration may be advisable for highly pre-rendered apps, or blogs, e-commerce stores, or otherwise SEO relevant sites.
  
<hr />

## 6. <a name="rav">ReactJS vs. Angular vs. Vue.js</a>
  
| &nbsp; | *[ReactJS](https://react.dev/)* | *[Angular](https://angular.dev/)* | *[Vue.js](https://vuejs.org/)* |
| ---------- | :----------: | :----------: | :----------: |
| **Definition** | JS Library | JS Framework | JS Framework |
| **DOM Type** | Virtual | Real (with Optimization) | Virtual | 
| **(Relative) Learning Curve** | Light | Heavier | Lightest |
| **(Primary) Languages** | JS, JSX | JS, TypeScript, HTML, CSS | JS, HTML, CSS |
| **Primary Use Case** | Interactive Single-Page Apps | Complex Enterprise Apps | Varied/Versatile |


<hr />
  
## 7. <a name="supplemental">Supplemental Resources</a>
  
* *[Intro to MERN and MEAN Stack Overview Guide](https://github.com/chaseofthejungle/intro-to-mern-and-mean-stack)*  
* *[JavaScript Event Handling Guide](https://github.com/chaseofthejungle/js-event-handling-guide)*  
* *[ReactJS Official Website](https://react.dev/)*  
