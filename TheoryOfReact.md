Part 1 - Basic Knowledge:

1.What is React.js?<br/>
React.js is a JavaScript library for building user interfaces.

2.What are the key features of React.js?<br/>
JSX (JavaScript Syntax Extension)<br/>
Virtual DOM<br/>
One-way data binding<br/>
Performance<br/>
Extensions<br/>
Conditional statements<br/>
Components<br/>
Simplicity<br/>

3.What is JSX?<br/>
A syntax extension for JavaScript used in React to describe the user interface.<br/>

4.What is a virtual DOM?<br/>
The virtual DOM (VDOM) is a programming concept where an ideal, or “virtual”, representation of a UI is kept in memory and synced with the “real” DOM by a library such as ReactDOM.<br/>

5.What is the difference between props and state?<br/>
Props are used to pass data from parent to child components, while state is used for managing a component's internal data.<br/>

6.What is the role of Redux in a React.js application?<br/>
Redux is a state management library used to manage global application state in React.<br/>

7.What is the purpose of React Router?<br/>
React Router is used for routing and navigation in a React application.<br/>



Part 2 - Code Implementation:<br/>

1.Create a simple React component that displays "Hello World!" as text.<br/>
```
function HelloWorld() {           
  return <div>Hello World!</div>;
}
```
2.Create a form component with input fields for name and email.
```
function FormComponent() {
  return (
    <form>
      <input type="text" placeholder="Name"/>
      <input type="email" placeholder="Email" />
    </form>
  );
}
```

3.Implement a React component that displays a list of items.
```
function ItemList() {
  const items = ['Item 1', 'Item 2', 'Item 3'];
  return (
    <ul>
      {items.map((item, index) => (
        <li key={index}>{item}</li>
      ))}
    </ul>
  );
}
```
4.Use React Router to create a multi-page application with a navigation menu.<br/>
Install React-router-dom<br/>
Import the necessary Routing Elements<br/>
Build the Routes :<br/>
```
      <main className="container">
        <Header/>
        <Routes>
          <Route path="/" element={<Home/>}/>
          <Route path="/reservations" element={<ReserveSection/>} />
          <Route path="/usersDetails" element={<UsersDetails/>}/>
          <Route path="/pay" element={<PaymentSection/>} />
          <Route path="/bookingconfirmation" element={<ConfmirmedBooking/>}/>
        </Routes>
      </main>
```


Part 3 - Advanced Concepts:<br/>

1.Explain the concept of React hooks.<br/>
React hooks are functions that allow functional components to manage state and side effects, replacing class-based component features.<br/>

2.What are higher-order components in React and how are they useful?<br/>
Higher-order components (HOCs) are functions that wrap a component to provide additional functionality, enhancing reusability.<br/>

3.Explain the difference between server-side rendering and client-side rendering in React.<br/>
Server-side rendering (SSR) renders React components on the server and sends HTML to the client, while client-side rendering (CSR) renders components in the browser.<br/>

4.How would you optimize the performance of a React application?<br/>
To optimize React app performance, use techniques like code splitting, lazy loading, and memoization. Also, minimize unnecessary re-renders.<br/>

5.What is the role of context in React?<br/>
Context in React provides a way to pass data through the component tree without having to pass props manually. It's useful for sharing state with many components or configuration.<br/>



Part 4 - Real-world Application:<br/>

1.Describe a React.js project you have worked on and your contribution to it.<br/>
I built  efficient, user-friendly, maintainable and responsive reservation system for the restaurant from scratch:<br/>

2.How did you ensure the project was maintainable and scalable?<br/>
I organized the project into modular components, making it easier to maintain and extend in the future.<br/>
I utilized state management tools like React's built-in state to ensure data integrity and scalability as the application grows.<br/>
I provided comments and documentation to make the codebase more understandable for potential future developers.<br/>

3.What challenges did you face while working on the project, and how did you overcome them?<br/>
Managing the multi-step reservation process was challenging, but I used React Router to handle navigation and maintain a clear user flow.<br/>
Ensuring the accuracy of reservation and customer details was essential. I implemented client-side validation and incorporated error handling to guide users through the correct input.<br/>
Popup Window: Creating a confirmation portal-popup window required careful handling of UI state and user interactions. I used React Modals for this purpose.<br/>
