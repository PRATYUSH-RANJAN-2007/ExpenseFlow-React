# ExpenseFlow — React + Vite

Student project demonstrating React + Vite, Admin/User modules, Local Storage signup/login, expense tracking, budgets, reports, Git/GitHub and Vercel deployment.

## Demo accounts
- Admin: `admin@expenseflow.demo` / `Admin123!`
- User: `student@expenseflow.demo` / `Student123!`

New signups are assigned the User role.

## Run locally
1. Install Node.js LTS from https://nodejs.org/
2. Open this folder in VS Code.
3. Run `npm install`
4. Run `npm run dev`
5. Open the URL Vite prints, normally http://localhost:5173

## Test production build
`npm run build`

## GitHub
Create an empty repository, then from this folder:
```bash
git init
git add .
git commit -m "Build ExpenseFlow React dashboard"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
git push -u origin main
```
If a remote already exists, inspect `git remote -v` first.

## Deploy to Vercel
CLI method:
```bash
npm install -g vercel
vercel login
vercel
vercel --prod
```
Accept the detected Vite settings. For GitHub import, use build command `npm run build` and output directory `dist`.

## Security note
This is an educational frontend-only demo. Local Storage is user-editable and demo passwords are stored as plain text. Do not use real credentials or sensitive information. Production authentication requires a backend, password hashing, server-side authorization, and a database.
