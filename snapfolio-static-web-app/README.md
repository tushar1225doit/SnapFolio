## Aim:- Develop and deploy a portfolio Azure static Web App on a custom domain (tushargalhotra.shop) creating and using git repository, In this pursuit I downloaded a web template and customise it then commited to the repository and then using Azure static web app then configure a custom domain

flowchart LR
    Dev[Developer: Push code to GitHub] -->|Commit| Repo[GitHub Repo]
    Repo -->|CI/CD via GitHub Actions| Azure[AWS Static Web App]
    Azure --> Domain[Custom Domain: tushargalhotra.shop]
    Domain --> User[End Users Access Website]


Technologies Used

   Azure Static Web App for hosting
   GitHub Actions for CI/CD
   Git + GitHub for version control


Deployment Steps

Initialize Git repository & push code to GitHub

   git init
   git add .
   git commit -m "Initial commit with portfolio template"
   git remote add origin <repo-url>
   git push -u origin main


Create Azure Static Web App

   Go to Azure Portal → “Static Web App” → Connect GitHub repo.
   Select branch (main) and build presets (custom/static).

Add Custom Domain

   In Static Web App → Custom domains → Add tushargalhotra.shop.
   Configure DNS (CNAME record).
   Verify and apply SSL certificate.

🔄 CI/CD Workflow

   Every push to main triggers GitHub Actions.
   Workflow builds the static files and deploys them to Azure automatically.

🌍 Live Demo
   👉 tushargalhotra.shop

🛠️ Troubleshooting

      404 error after deployment → Check index.html in root.
      Domain not resolving → Verify DNS records in your registrar.
      SSL error → Re-bind certificate in Azure portal.
