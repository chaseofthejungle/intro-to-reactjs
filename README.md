# Intro to ReactJS

**Definition/Overview:** ReactJS was developed by Facebook (now *Meta*) as a client-side JavaScript (JS) library. It is utilized by developers to build *single-page apps* and customize interactive user interfaces (UIs) via highly reusable and flexible web *components*. The relatively light learning curve (in comparison to a heavier JS framework, such as AngularJS) of ReactJS assists in optimizing UIs and their associated User Experience (UX) potential.
  
ReactJS also utilizes a JavaScription syntax extension known as JavaScript XML, or 'JSX'. It combines JS and HTML scripting within individual files.

#### Table of Contents:

1. ['Hello World' Code Example](#hello-world)
2. [Components and Elements](#components-and-elements)
3. [Optimization and Pitfalls](#optimization-and-pitfalls)
4. [Supplemental Resources](#supplemental)
  
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

## <a name="components-and-elements">2. Components and Elements</a>
  
**What exactly are 'components'?:** A ReactJS component is a piece of code that can be reused throughout an application. There are many possibilities for what ReactJS components can be--buttons, textboxes, and text headings, for example. This reuse of code slices allows for apps to be developed quicker and perform faster.
  
**What about 'single-page apps'?:** Simply put, these are apps in which clicking on elements, such as navigation menu items and various links, does not result in reloading of the app as a whole. Instead, *the only reloaded content is the body of the freshly requested section*. For an example of this, consider a movie and/or television streaming service, such as Hulu or Netflix. The use of a single-page app system allows for users to watch their streaming media content without reloading entire pages.
  
<hr />
  
## <a name="optimization-and-pitfalls">3. Optimization and Pitfalls</a>
  
**How is ReactJS Optimized?:** Some of the ReactJS features and techniques that benefit UI/UX developers include...
  
* **Debouncing and Throttling**
  + This limits when functions execute, and how often.
* **Functional Pattern Adherence**
  + This assists in handling complex code/logic, potentially reducing errors and increasing performance.
* **Lazy Loading**
  + This limits component loading to only when it is needed.
* **List Virtualization**
  + This limits the rendering of list items to only when they are available on screen to users.
* **Memoization**
  + This caches responses for future re-use, increasing performance when serving clients web assets.
    - Consider using memoization tools such as *useMemo* and *React.memo*.
* **useReducer() and useTransition() Hook Leveraging/Utilization**
  + useReducer() defines how states are to be updated.
  + useTransition() limits updates until when they are needed, potentially increasing performance.

**Common Mistakes in ReactJS Development include:**  
* **Forgetting to Use Keys in Lists**
  + Keys detect added, modified, and removed items.
* **Imprecise Component Structure**
  + If logic is spread across components, updating/maintaining components and component reuse can become a mess. 
* **Mutating State Directly**
  + This can cause errors and other unintended behaviors. Thus, it is better practice to update state immutably.
* **Overlooking Performance Optimization Techniques**
  + This includes the principles outlined in the above section.
* **Overreliance on Inline Functions**
  + This can cause extraneous rerendering, and therefore unnecessary performance costs.
  
<hr />
  
## 4. <a name="supplemental">Supplemental Resources</a>
  
* [Intro to MERN and MEAN Stack Overview Guide](https://github.com/chaseofthejungle/intro-to-mern-and-mean-stack)  
* [JavaScript Event Handling Guide](https://github.com/chaseofthejungle/js-event-handling-guide)  

<hr />
  
TODO: Add comparison of ReactJS to AngularJS and Next.js.
