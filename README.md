# Intro to ReactJS

**Definition/Overview:** ReactJS is a client-side JavaScript (JS) library that is utilized by developers to build and customize interactive user interfaces (UIs) via highly reusable and flexible web components. The relatively light learning curve (in comparison to a heavier JS framework, such as AngularJS) of ReactJS assists in optimizing UIs and their associated User Experience (UX) potential.

**How is ReactJS Optimized?:** Some of the ReactJS features and techniques that benefit UI/UX developers include...
  
* Debouncing and Throttling
  + This limits when functions execute, and how often.
* Functional Pattern Adherence
  + This assists in handling complex code/logic, potentially reducing errors and increasing performance.
* Lazy Loading
  + This limits component loading to only when it is needed.
* List Virtualization
  + This limits the rendering of list items to only when they are available on screen to users.
* Memoization
  + This caches responses for future re-use, increasing performance when serving clients web assets.
    - Consider using memoization tools such as *useMemo* and *React.memo*.
* useReducer() and useTransition() Hook Leveraging/Utilization
  + useReducer() defines how states are to be updated.
  + useTransition() limits updates until when they are needed, potentially increasing performance.

**Common Mistakes in ReactJS Development include:**  
* Forgetting to Use Keys in Lists
  + Keys detect added, modified, and removed items.
* Imprecise Component Structure
  + If logic is spread across components, updating/maintaining components and component reuse can become a mess. 
* Mutating State Directly
  + This can cause errors and other unintended behaviors. Thus, it is better practice to update state immutably.
* Overlooking Performance Optimization Techniques
  + This includes the principles outlined in the above section.
* Overreliance on Inline Functions
  + This can cause extraneous rerendering, and therefore unnecessary performance costs.

TODO: Add comparison of ReactJS to AngularJS and Next.js.
