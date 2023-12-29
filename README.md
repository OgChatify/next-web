## OgChatify is the newer and updated ersion of chatify.

Features Included:

- Real-time messaging
- Delete & Edit messages in real time
- Create Text, Audio and Video call Channels
- 1:1 conversation between members
- 1:1 video calls between members
- Member management (Kick, Role change Guest / Moderator)
- Unique invite link generation & full working invite system
- Server creation and customization
- Beautiful UI
- Full responsivity and mobile UI
- Light / Dark mode
- Websocket fallback: Polling with alerts
- ORM using Prisma
- MySQL database using Planetscale
- Authentication with Clerk

### Prerequisites

**Node version 18.x.x**

### Cloning the repository

```shell
git clone https://github.com/OgChatify/next-web
```

### Install packages

```shell
yarn install
```

### Setup .env file

```js
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=
NEXT_PUBLIC_CLERK_SIGN_IN_URL=
NEXT_PUBLIC_CLERK_SIGN_UP_URL=
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=


DATABASE_URL=

UPLOADTHING_SECRET=
UPLOADTHING_APP_ID=

LIVEKIT_API_KEY=
LIVEKIT_API_SECRET=
NEXT_PUBLIC_LIVEKIT_URL=

NEXT_PUBLIC_SITE_URL=
```

### Setup Prisma

Add Postgresql Database (I used Supabase)

```shell
npx prisma generate
npx prisma db push

```

### Start the app

```shell
yarn dev
```

## Available commands

Running commands with npm `yarn [command]`

| command | description                              |
| :------ | :--------------------------------------- |
| `dev`   | Starts a development instance of the app |
| `build` | Build the application                    |
