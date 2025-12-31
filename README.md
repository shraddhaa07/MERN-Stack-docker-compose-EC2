# 🚀 MERN Stack Application with Docker & AWS EC2
A full-stack MERN application deployed using Docker Compose on an AWS EC2 instance.
<img width="765" height="334" alt="diagram-export-17-12-2025-12_07_03-pm" src="https://github.com/user-attachments/assets/298276f0-1074-4239-8540-eda79323ce43" />


**Note** - To run this project using `docker compose`, follow the below steps.

<!--Switch to the `compose` branch to learn the-->

1. Implementation of `Dockerfile` for `client` and `server`.
2. Run the containers using `Docker Compose`.
3. Deploy it on `AWS EC2`

## 🐳 Docker Architecture
- Frontend container (Vite – React)
- Backend container (Node + Express)
- MongoDB container
- Custom Docker network


## ⚙️ Environment Variables

Create a `.env` file based on `.env.example`

```env
VITE_API_URL=http://<EC2_PUBLIC_IP>:5050
MONGO_URI=mongodb://mongo:27017/mydatabase
```

## Run it local without Docker
`docker compose up --build -d`

### Prerequisite

- Install `npm`

#### Start Server:

```
cd mern/server
npm install
npm start
```

#### Start Client

```
cd mern/client
npm install
npm run dev
```
<img width="1919" height="782" alt="image" src="https://github.com/user-attachments/assets/1930cd6c-3f8c-47a6-94c9-397a5cd158c8" />

<!--<img width="1790" alt="Screenshot 2024-08-31 at 11 07 58 PM" src="https://github.com/user-attachments/assets/f414230b-8bd6-4393-b8de-6a10444a8dfd">-->
