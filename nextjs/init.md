# Building Next.js environment with docker
## Notice
The Vercel platform does not support the deployment of Docker images.

Vercel: [Does Vercel support Docker deployments?](https://vercel.com/support/articles/does-vercel-support-docker-deployments)

So basically, build a development environment using ShellScript.

This is only think of it as a Docker practice.
## How to use
1. make directory
```
mkdir [your project name]
```

2. move to the created directory
```
cd [your project name]
```

3. copy nextjs/Dockerfile & nextjs/docker-compose.yml to your project

4. install create-next app
```
docker-compose run --rm app npm install create-next-app
```

5. install Next.js(TypeScript)
```
docker-compose run --rm app npx create-next-app frontend --ts
```

6. check
```
docker-compose up -d
```