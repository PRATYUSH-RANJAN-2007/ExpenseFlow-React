# Submission and Deployment Checklist

## Before GitHub
- [ ] `npm install` completes successfully.
- [ ] `npm run dev` opens the application.
- [ ] Signup creates a new User account.
- [ ] User login opens the User module.
- [ ] Admin login opens the Admin module.
- [ ] User can add, search, filter, and delete an expense.
- [ ] User can save a budget and view reports.
- [ ] Admin can search users and review platform transactions.
- [ ] `npm run build` completes successfully.

## Push to GitHub
```bash
git init
git add .
git commit -m "Build ExpenseFlow React dashboard"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
git push -u origin main
```
If the repository has already been initialized, run `git status` and `git remote -v` before running initialization or adding another remote.

## Vercel CLI deployment
```bash
npm install -g vercel
vercel login
vercel
vercel --prod
```
Run the commands from the project root. Accept detected Vite settings only after confirming the build command is `npm run build` and output directory is `dist`.

## Submit for review
- [ ] GitHub repository URL opens.
- [ ] Vercel production URL opens in a private/incognito browser.
- [ ] Test the demo Admin and User accounts on the deployed app.
- [ ] Verify signup and expense updates persist after refresh in the same browser.
- [ ] Keep screenshots of both dashboards and the successful deployment for presentation.
