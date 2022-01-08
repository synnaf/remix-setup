# Welcome to Remix!

- [Remix Docs](https://remix.run/docs)

## Development

From your terminal:

```sh
npm run dev
```

This starts your app in development mode, rebuilding assets on file changes.

## Deployment

First, build your app for production:

```sh
npm run build
```

Then run the app in production mode:

```sh
npm start
```

Now you'll need to pick a host to deploy it to.

### DIY

If you're familiar with deploying node applications, the built-in Remix app server is production-ready.

Make sure to deploy the output of `remix build`

- `build/`
- `public/build/`

### Using a Template

When you ran `npx create-remix@latest` there were a few choices for hosting. You can run that again to create a new project, then copy over your `app/` folder to the new project that's pre-configured for your target server.

```sh
cd ..
# create a new project, and pick a pre-configured host
npx create-remix@latest
cd my-new-remix-app
# remove the new project's app (not the old one!)
rm -rf app
# copy your app over
cp -R ../my-old-remix-app/app app
```


### Remix file structure 

Our three main files sets the overall functionality and html output: 
- `entry.client.jsx`
- `entry.server.jsx`
- `root.jsx`

`/routes` folder contain our main React component - `index.jsx`. 



### Why Remix? 
- https://developpaper.com/next-js-strong-opponent-is-coming-remix-officially-announced-open-source/ 
- Remix is a Web Framework, it uses React as the view layer like Next, but it's not tied to React and it's more intended to be a full-stack web application framework.

- Remix has no static site support, so it always needs a server.
- Good for use cases where you have a database, dynamic data, user accounts with private data, etc. 
- The client and server have the same development experience. The client code and server code are written in one file for seamless data interaction. At the same time, based on typescript, type definitions can be shared across clients and servers.  (Love this <3)
