# Expocaster

>Expo mobile, web and API for creating Farcaster native applications.

**Version: v0.0.0**

The one stop repository for native mobile farcaster experiences offering the same to web and additional API building possibilities.

That way with the same code written once you can

- Run a native mobile app
- Run a responsive web app
- Farcaster Frames Backend and general API/backend

Write once, enjoy everywhere.

[Contribute](#contribute)

## Getting Started

to test: 
1) Clone the repository
1) ```npm install``` 
1) ```npm expo start```

You'll now be greated by Expo where you can [check their docs](https://docs.expo.dev/get-started/expo-go/)

## built using Farcaster Ecosystem awesomness

- [Farcasterkit - React Hooks](https://www.farcasterkit.com/)

```
npm install farcasterkit
```

- [Neynar Types and optional API integration](neynar.com)

- [Litecast - Inspired Frame Rendering](https://github.com/dylsteck/litecast)

## also built on top of Typescript awesomeness

- [Create Expo Stack - spin up an expo mobile, web, api stack the way it should be in 10s](https://createexpostack.com/)

## Contribute

The stack used has NativeWind for styling so you can use the typical ```className=""``` syntax your might now from web with Tailwind.

otherwise it's straight Typescript and Expo.

### To contribute changes/improvements

1) fork the repository
2) make your changes
3) submit a PR

### To contribute feedback and bug reports

1) create an Issue

# Deployment of Frames and Web

>Official Expo [Deployment Documentation here](https://vercel.com/docs/cli/deploying-from-cli#deploying-from-local-build-prebuilt) to be used as most up to date document and reference checked if the below doesn't work!

## NodeJS with Express

> Expo's [Official Documentation can be found here and should be referenced if the below doesn't work](https://docs.expo.dev/router/reference/api-routes/#express)

Copy the following file structure over to your server where you have nodeJS installed

```
/
|
|_ server.js
|
|_ dist/

```

then run the node server

```
node server.js
```

## Vercel

>NOTE: this hasn't been made work, but is what documentation states! If you make it work please open a PR!

If your remote build doesn't work you may try [prebuilding and then uploading](https://vercel.com/docs/cli/deploying-from-cli#deploying-from-local-build-prebuilt) like so:

this assumes you have vercel installed (```npx vercel```) and configured

```
npx vercel build && npx vercel deploy --prebuilt
```