# Expert Votes [![license](https://img.shields.io/badge/LICENCE-MIT-blue)]() [![status](https://img.shields.io/badge/STATUS-DONE-brightgreen)]()

> Application developed in "Next Level Week: Expert" event, promoted by Rocketseat 🚀 <br>

**Expert Votes** is an application that allows you to create and vote on polls ✅

<details>
  <summary>✨ <b>Features</b> </summary>

- [x] Create a poll (with N options)
- [x] Get poll details
- [x] Vote
- [x] Monitor votes in real time
</details>

> [!TIP]
> Visit [demo]() or the others repositories of this project:

![NodeJS](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white) ![Fastify](https://img.shields.io/badge/fastify-%23000000.svg?style=for-the-badge&logo=fastify&logoColor=white) ![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)  ![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white) ![Prisma](https://img.shields.io/badge/Prisma-3982CE?style=for-the-badge&logo=Prisma&logoColor=white) ![Postgres](https://img.shields.io/badge/postgres-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white) ![Redis](https://img.shields.io/badge/redis-%23DD0031.svg?style=for-the-badge&logo=redis&logoColor=white) ![WebSocket](https://img.shields.io/badge/WebSocket-gray?style=for-the-badge&logo=socket.io&badgeColor=010101)

<div align="center">
  <img alt="Expert Votes" src="" />
</div>


## Building and running locally

Be sure you have [Git](https://git-scm.com/downloads) and [Node.js](https://nodejs.org/) installed, then follow the directions below.

```bash
# Clone this repository
$ git clone https://github.com/MariaGabrielaReis/expert-votes

# Access project folder
$ cd expert-votes

# Install dependencies
$ yarn
```

> [!IMPORTANT]
> Before running the project, set up the container with database and configure Prisma:
>
> ```bash
> $ docker-compose up -d
> ```
>
> Now, run Prisma migrations:
>
> ```bash
> $ npx prisma migrate dev
> ```

```bash
# Run application
$ yarn dev
```

> [!NOTE]
> The server will start on port 3333 - <http://localhost:3333>
>
> - For quick API testing, use `test.http` file to send requests with the VSCode "REST Client" extension.
> - To test the socket route (to monitor votes), use a tool like [Online Websockets Tester](https://piehost.com/websocket-tester) with URL: `ws://localhost:3333/polls/:pollId/results` and use the HTTP routes to vote and see the count. 
