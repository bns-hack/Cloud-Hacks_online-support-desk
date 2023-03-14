# Support Desk App
![spr-dsk1](https://user-images.githubusercontent.com/11625672/225076972-bde6b72b-e456-4a00-a818-d2c0f8ce377d.png)

![sp5](https://user-images.githubusercontent.com/11625672/225077174-ba186649-5b32-43ed-a48d-f76cc2812ffe.png)


Support ticket application built with the MERN stack.

## Inspiration
Inspired by Oracle Cloud and Autonomous DB API support for MongoDB

## What it does
Our APP enables you to make use of support desk and accessing your queries for any online support and issues

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
