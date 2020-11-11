# 📓 Lesson 07: Add a Stripe API Key as an Environment Variable in Next.js & Vercel

With Stripe or many other services, their APIs rely on special keys that authenticate requests or allow that service to track usage for things like billing.

Some of these keys are able to be used publicly and some must be kept private, but ultimately we want to have a way to easily manage these keys and not hard-code them into our application, which is where environment variables come in.

## Getting Started

The API key is what allows us to connect to Stripe and integrate their checkout experience with our app.

In lesson 7, we're going to find our API key in our Stripe account and figure out how we can use it in our Next.js app. We'll set it up as an environment variable which will allow us to access it later in our code as well as make it easily interchangeable if we ever need to change it.

## Objectives
* Find API key in Stripe dashboard
* Create a .env.local file and store API key as an environment variable
* Test the environment variable by logging it to the web console
* Add API key as an environment variable to Vercel deployment

## Exercises



### 1. Locate your unique API key in the Stripe dashboard



### 2. Create an environment variables file to store the API key



#### Where We'll Make Changes
* `.env.local`

### 3. Log the environment variable to the web console


#### Where We'll Make Changes
* `pages/index.js`

### 4. Add the API key as an environment variable in Vercel

## Extra Credit

### 1. Update the global environment file

Each lesson in this course uses its own set of files, meaning, changes to the `.env.local` file won't carry on to the next lesson.

To get around that, future lessons will be taking advantage of a shared `.env.shared` file that lives in the `lessons` folder of this repository where we can make our environment changes and have them available throughout all of the lessons.

Take a moment to review the shared `.env.shared` file inside of `shared/.env.shared` and update the Stripe API key.

> 👋 **Hey! Quick Note**
>
> In order for the Stripe integration to work later, you'll need to make sure you have the right API key.

#### Where We'll Make Changes
* `lessons/shared/.env.shared`