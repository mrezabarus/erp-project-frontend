
mkdir erp-project
cd erp-project
npm init -y
npm install concurrently --save-dev
Edit package.json
```
    "scripts": {
        "start:backend": "npm --prefix backend run start",
        "start:frontend": "npm --prefix frontend run dev -- -p 3001",
        "start": "concurrently \"npm run start:backend\" \"npm run start:frontend\""
    },
```
npm i -g @nestjs/cli
nest new backend (create nestjs apps backend)
npx create-next-app@latest frontend (create nextjs apps frontend)

setelah itu push ke git masing masing
git backend
git frontend
