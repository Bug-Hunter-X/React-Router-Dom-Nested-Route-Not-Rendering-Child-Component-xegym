# React Router Dom Nested Route Bug
This repository demonstrates a common issue with nested routes in React Router Dom v6.  The problem involves a nested route not rendering the child component when a route with parameters is used.

## Problem
The `/contact/:id` nested route is not working as expected. When you navigate to a URL like `/contact/123`, the `Contact` component renders instead of the `ContactDetails` component. 

## Solution
The solution involves using the `useParams` hook to access the route parameters, which is then passed to the `ContactDetails` component.