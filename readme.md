# Support Desk App

Support ticket application built with the MERN stack.

## Inspiration
Inspired by Oracle Cloud and Autonomous DB API support for MongoDB

## What it does
Our API enables you to make use of managing and accessing your resources for storing PDF, TXT files and images [Blogs]

## How we built it
Built around OKE Kubernetes cluster and DB tools

## Challenges we ran into
How to configure our cluster for our Networking
How to setup DB API for MongoDB
How to setup deployments manifest

## Accomplishments that we're proud of
Oracle kubernetes configuration and DB setup

## What we learned
Kubernetes networking, DB configuration with MongoDB

## What's next for Online Support Desk APP
To integrate with more features and setup multi repos for our APP

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
