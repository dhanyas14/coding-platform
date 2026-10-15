
docker build -t coding-judge-java   judge/images/java
docker build -t coding-judge-node   judge/images/node
docker build -t coding-judge-c      judge/images/c
docker build -t coding-judge-cpp    judge/images/cpp
```

2) Start the backend (from project root):

```powershell
node server.js
```

3) Start the frontend (in a separate shell):

```powershell
cd coding-platform
npm install
npm start
```


## Developer notes

- Frontend now calls the Docker-backed `/execute` endpoint and shows `compileError`, `stderr`, and non-zero exit statuses prominently.
- `REACT_APP_API_BASE_URL` is used for configuring the API base URL in different environments.

## Tech stack

- Backend: Node.js (Express)
- Frontend: React (Vite) and CodeMirror for the editor
- Sandboxing: Docker judge images (GCC for C/C++, Temurin JDK for Java, Python 3, Node.js)





