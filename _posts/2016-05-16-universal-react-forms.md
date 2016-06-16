---
layout: post
title: Universal ReactJS Forms
intro: In this post we'll look at how we can produce user input forms that work with or without JavaScript in a Universal React application.
---

I've [written before on Universal React applications](https://24ways.org/2015/universal-react/) but have never really discussed how to do user input in a Universal React application. If you've created a form with React there's no reason that, with a small amount of extra effort, you can have this form work with or without React.

To demonstrate how this is possible I've created a [sample application on GitHub](https://github.com/jackfranklin/universal-react-example/pull/8/files) that takes a user's email and "subscribes" them to our made up newsletter. In a browser with JavaScript the form is entirely client side, the validation is all done on the client and then with the data it can make a request to an API to store it. In a non JavaScript browser the `form` will post its data to an endpoint, which the server then listens out for and processes the data.

