# SDC Project Review 2 — Project Report

## Project title
ExpenseFlow: Student Expense Tracker

## Objective
Build a responsive client-side expense tracking application using React and Vite. The application demonstrates Admin and User modules, signup/login using browser Local Storage, responsive UI layout, reports, and a GitHub/Vercel deployment workflow.

## Technology stack
- React: UI components and state-driven rendering
- Vite: development server and production build tool
- JavaScript: application logic, validation, filtering, calculations, CSV export
- HTML: application entry point
- CSS: responsive styling with Grid and Flexbox
- Local Storage: demo persistence for users, expenses, budgets, and session state
- Git/GitHub: source history and remote repository
- Vercel: static hosting of the Vite production output

## Modules
### 1. Authentication module
- Signup with name, email, and password
- Basic form validation
- Duplicate email prevention
- Login against stored demo account records
- Logout and session state
- New registrations receive the User role

### 2. User module
- View the personal dashboard
- Add, search, filter, and delete personal expenses
- Track monthly expenses and remaining budget
- Set a monthly spending limit
- View spending reports
- Export the displayed expenses to CSV

### 3. Admin module
- View platform-level statistics
- Search registered accounts
- View transactions across user accounts
- Remove non-admin accounts and their associated expenses
- View and export reports

### 4. Reporting module
- Filter reports by last 7 days, current month, or all time
- Calculate spending totals, transaction count, average transaction amount, and category totals
- Export data to CSV

## Data model (Local Storage)
- `ef_users`: array of demo user records
- `ef_expenses`: array of expense records
- `ef_budgets`: object mapping user ID to monthly budget
- `ef_session`: current demo session object

An expense includes an ID, user ID, title, category, numeric amount, date, and optional note.

## Execution
1. Install Node.js LTS.
2. Extract the project ZIP and open the folder in VS Code.
3. Run `npm install`.
4. Run `npm run dev` and open the URL printed by Vite.
5. Run `npm run build` to verify the production build.

## Demo accounts
- Admin: `admin@expenseflow.demo` / `Admin123!`
- User: `student@expenseflow.demo` / `Student123!`

New accounts created from the Signup page are User accounts.

## Limitations and security
This is a frontend-only educational prototype. Local Storage can be read and changed by the browser user, and demo passwords are stored as plain text. It is not suitable for real authentication or sensitive financial data. A production version should use a backend API, password hashing, server-side authorization, secure session handling, and a database. Admin role checks in a client-only app demonstrate UI/module separation, not secure access control.
