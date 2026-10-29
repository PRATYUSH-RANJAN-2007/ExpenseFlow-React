# ExpenseFlow — Viva Questions and Answers

1. **What is React?**  
   React is a JavaScript library for building reusable, component-based user interfaces.

2. **What is Vite?**  
   Vite is a frontend development tool that provides a fast dev server and builds optimized production assets.

3. **Why did you use React with Vite?**  
   React organizes the interface into components, while Vite gives a quick development workflow and a production build command.

4. **What is JSX?**  
   JSX is a syntax extension that lets React components describe UI using markup-like expressions inside JavaScript.

5. **What is `useState` used for?**  
   `useState` stores component state, such as the current page, logged-in user, expense list, and form values.

6. **What is `useEffect` used for in this project?**  
   It initializes sample Local Storage data and loads persisted users, expenses, budgets, and session information when the app starts.

7. **What is Local Storage?**  
   Local Storage is browser storage that keeps string key/value data across page reloads for the same origin.

8. **Why use `JSON.stringify` and `JSON.parse`?**  
   Local Storage stores strings. `JSON.stringify` converts JavaScript data to a string; `JSON.parse` converts a JSON string back to JavaScript data.

9. **What is the difference between Admin and User modules?**  
   Users manage their own expenses and budget. Admins see platform-wide summary data, review users, and inspect transactions across accounts.

10. **How are new accounts assigned a role?**  
    Signup assigns each new account the `user` role. The demo admin account is seeded separately.

11. **How does the budget progress work?**  
    The app sums expenses for the current month and divides the total by the monthly budget to calculate the progress percentage.

12. **What is CSS Grid?**  
    CSS Grid is a two-dimensional layout system for arranging content in rows and columns.

13. **What is Flexbox?**  
    Flexbox is a one-dimensional layout system useful for aligning and distributing items along a row or a column.

14. **What is Git?**  
    Git is a distributed version-control system that records project changes.

15. **What is the difference between Git and GitHub?**  
    Git tracks version history; GitHub hosts Git repositories and adds collaboration features.

16. **What is a branch?**  
    A branch is a separate line of development that lets a change be developed without immediately altering another branch.

17. **What is merging?**  
    Merging integrates changes from one branch into the currently checked-out branch.

18. **What does `npm run build` do?**  
    It runs Vite's production build and writes optimized static files to the `dist` directory.

19. **How is the app deployed to Vercel?**  
    Push the project to GitHub and import the repository into Vercel, or use the Vercel CLI. Vercel builds the app and hosts the static output in `dist`.

20. **Is Local Storage authentication secure for production?**  
    No. Browser storage is editable and accessible to the user. Production authentication requires server-side checks, hashed passwords, secure session management, and a database.
