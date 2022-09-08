# Support Desk App

Support ticket application built with the MERN stack.

## Inspiration
Inspired by Oracle Cloud and Autonomous DB API support for MongoDB

## What it does
Our API enables you to make use of managing and accessing your resources for storing PDF, TXT files and images [Blogs]

## How we built it
Built around CIVO Kubernetes cluster and Devtron tools

## Challenges we ran into
How to configure our cluster for our Networking
How to setup CI/CD pipelines
How to setup deployment charts

## Accomplishments that we're proud of
CIVO kubernetes configuration and CI/CD pipelines setup

## What we learned
Kubernetes networking, CI/CD configuration with Devtron tools.

## What's next for Resource Management APP
To integrate with UI and setup multi repos for our APP using Devtron tools

## Usage

### Set Environment Variables

Rename the .envexample to .env and add your [MongoDB](https://www.mongodb.com/) database URI and your JWT secret

### Install backend dependencies

```bash
cd backend
npm install
```

### Install client dependencies

```bash
cd frontend
npm install
```

### Run app in development (frontend & backend)

```bash
npm run dev
```
