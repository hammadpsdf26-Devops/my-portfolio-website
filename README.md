Aaj ka Kaam — DevOps Journey (Day Log)

Tareekh: 22 July 2026

Kya seekha aur kiya:
Git basics practice ki — git init, git add, git commit, git push, git pull, branches, aur merge conflicts ka concept clear kiya.
Apna personal portfolio website banaya — HTML aur CSS use karke, jisme About Me, Skills, aur Contact sections included the.
GitHub pe project push kiya — local machine se VS Code aur Git Bash ke through command line se repository create karke code GitHub pe upload kiya.
Azure Static Web App create ki — Azure Portal pe naya resource banaya aur usay GitHub repository se connect kiya taake automatic CI/CD ho sake.
CI/CD Pipeline (GitHub Actions) setup ki — Azure ne khud ek workflow file (.yml) generate ki jo har push pe automatically build aur deploy karti hai.
Website ko live deploy kiya — poora end-to-end flow complete kiya: Local Code → GitHub → Azure Static Web App (Live URL).
Mushkilein jo face ki aur unko kaise solve kiya:
Region Policy Error: Azure for Students subscription ke saath Central US region allowed nahi tha. Region change karke resolve kiya.
Branch Mismatch: Local repository ki branch main thi, lekin Azure ne workflow master branch pe set kar di thi — is wajah se pehle deployment content receive nahi kar rahi thi. Consistency ke liye master branch use ki.
Build Failure (Oryx Error): GitHub Actions workflow fail ho rahi thi kyunke Azure ka build system (Oryx) site ko Node.js project samajh raha tha aur npm run build dhoondh raha tha, jabke ye simple static HTML/CSS site thi. Workflow file mein skip_app_build: true add karke is masle ko fix kiya.
Result:

✅ Live Portfolio Website deploy ho gayi with full CI/CD pipeline — koi bhi future update push karne pe automatically deploy hoga.
