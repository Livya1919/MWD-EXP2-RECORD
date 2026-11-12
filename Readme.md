## Exp 02 - React Lab Exercise: Using Props
## NAME : LIVYA DHARSHINI G
## REG NO: 2305001013
## Aim
To create a React application that demonstrates passing data from a parent component to a child
component using props.
## Objectives
1. To create a React project using Vite.
2. To create a reusable Employee component.
3. To pass employee details such as name, ID, department, and designation using props.
4. To display multiple employees using the same component.
5. To understand props destructuring and one-way data flow in React.
## Program
```
Step 1: Create a React Project

npm create vite@latest props-demo -- --template react
cd props-demo
npm install
npm run dev

Step 2: Create Employee.jsx

function Employee({ name, id, department, designation }) {
  return (
    <div>
      <h2>Employee Details</h2>
      <p>Name: {name}</p>
      <p>ID: {id}</p>
      <p>Department: {department}</p>
      <p>Designation: {designation}</p>
      <hr />
    </div>
  );
}
export default Employee;

Step 3: Write App.jsx

import Employee from "./Employee";
function App() {
  return (
    <div>
      <h1>Employee Information</h1>
      <Employee
        Name="LIVYA DHARSHINI G"
        ID="2305001013"
        Department="CSE"
        Designation="Software Developer"
      />
      <Employee
        Name="user123"
        ID="102"
        Department="IT"
        Designation="Web Developer"
      />
      <Employee
        Name="user456"
        ID="103"
        Department="AIDS"
        Designation="Data Analyst"
      />
    </div>
  );
}
export default App;
```
## Output

<img width="983" height="656" alt="image" src="https://github.com/user-attachments/assets/b3d0ee9d-bb20-4915-b138-d6f4e940fb68" />


## Result
Thus, a React application was successfully created and executed to demonstrate passing employee
information from a parent component to a child component using props.
