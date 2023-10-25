# Kinde Starter Kit - Nuxt 3

## Register an account on Kinde

To get started set up an account on [Kinde](https://app.kinde.com/register). This is a [Nuxt 3](https://nuxt.com/) project bootstrapped with [`nuxi`](https://www.npmjs.com/package/nuxi).

## Setup your local environment

Clone this repo and install dependencies by running `npm i`

Make a copy of `.env.example` and name it simply `.env`. Replacing the following values from the Kinde `Settings -> Applications -> Backend app` page.

```
NUXT_AUTH_DOMAIN="https://<your_kinde_subdomain>.kinde.com"
NUXT_CLIENT_ID="<your_kinde_client_id>"
NUXT_CLIENT_SECRET="<your_kinde_client_secret>"
```

## Set your Callback and Logout URLs

Your user will be redirected to Kinde to authenticate. After they have logged in or registered they will be redirected back to your Nuxt application.

You need to specify in Kinde which url you would like your user to be redirected to in order to authenticate your app.

On the `Settings -> Applications -> Backend app` page set `Allowed callback URLs` to `http://localhost:3000/api/auth/callback`

> Important! This is required for your users to successfully log in to your app.

You will also need to set the url they will be redirected to upon logout. Set the ` Allowed logout redirect URLs` to http://localhost:3000.

Look at the [Nuxt 3 documentation](https://nuxt.com/docs/getting-started/introduction) to learn more.

## Start your project

Run `npm run dev` in a terminal and navigate to `http://localhost:3000`.

Click on `Sign up` and register your first user for your business!

## View users in Kinde

If you navigate to the "Users" page within Kinde you will see your newly registered user there. 🚀

## Production

Build the application for production:

```bash
npm run build
```

Locally preview production build:

```bash
npm run preview
```

Check out the [deployment documentation](https://nuxt.com/docs/getting-started/deployment) for more information.
