# Fastify + Svelte

Experimental backend server using [Fastify](https://www.fastify.io/).

### Install dependencies

```sh
npm install
```

### Run server
The server responds to `/api/counter` with JSON of the form:  
`{ "hello": "world", "count": count++ }`

The server also hosts static files from '../fullstack-frontend/build' at the server root `/`.

```sh
# Configure server to accept CORS credentials from frontend
# If this is unset, the server will accept all origins.
export FULLSTACK_FRONTEND=http://localhost:3000

npm start
```

### Developing with Gitpod
The main Gitpod configuration for this repo lives in https://github.com/jldec/fullstack-frontend.

Cloning this repo and creating a Gitpod project will trigger automatic prebuilds
when changes are committed to the repo.

The Gitpod workspace is configured to clone this backend repo into ../backend
of https://github.com/jldec/fullstack-frontend and run `npm install` on
both repos during prebuilds

Workspaces start with a backend server (running on port 3001) 
and a frontend dev server (running on port 3000).

---