<a name="readme-top"></a>

# Twak - A Real-Time Video Conferencing App (Yoom) using Next.js 14.

<!-- Table of Contents
<details>
<summary>

# Table of Contents

</summary>

- [Folder Structure](#bangbang-folder-structure)
- [Getting Started](#toolbox-getting-started)
- [Screenshots](#camera-screenshots)
- [Tech Stack](#gear-tech-stack)
- [Acknowledgements](#gem-acknowledgements)
- [Deploy on Vercel](#page_with_curl-deploy-on-vercel)

</details> -->

## Folder Structure

Here is the folder structure of this app.

```bash
video-conferenceing-app/
    |- actions/
        |-- stream.actions.ts
    |- app/
        |-- (auth)/
            |--- sign-in/[[...sign-in]]/
                |---- page.tsx
            |--- sign-up/[[...sign-up]]/
                |---- page.tsx
        |-- (root)/
            |--- (home)/
                |---- personal-room/
                    |----- page.tsx
                |---- previous/
                    |----- page.tsx
                |---- recordings/
                    |----- page.tsx
                |---- upcoming/
                    |----- page.tsx
                |---- layout.tsx
                |---- page.tsx
            |--- meeting/[id]/
                |---- page.tsx
        |-- global.css
        |-- layout.tsx
    |- components/
        |-- ui/
            |--- button.tsx
            |--- card.tsx
            |--- dialog.tsx
            |--- dropdown-menu.tsx
            |--- input.tsx
            |--- popover.tsx
            |--- sheet.tsx
            |--- textarea.tsx
            |--- toast.tsx
            |--- toaster.tsx
            |--- use-toast.ts
        |-- Alert.tsx
        |-- CallList.tsx
        |-- EndCallButton.tsx
        |-- HomeCard.tsx
        |-- Loader.tsx
        |-- MeetingCard.tsx
        |-- MeetingModel.tsx
        |-- MeetingRoom.tsx
        |-- MeetingSetup.tsx
        |-- MeetingTypeList.tsx
        |-- Navbar.tsx
        |-- Sidebar.tsx
    |- constants/
        |-- index.ts
    |- hooks/
        |-- useGetCallById.ts
        |-- useGetCalls.ts
    |- lib/
        |-- utils.ts
    |- providers/
        |-- StreamClientProvider.tsx
    |- images/
    |- .eslintrc.json
    |- .gitignore
    |- components.json
    |- middleware.ts
    |- next.config.mjs
    |- package-lock.json
    |- package.json
    |- postcss.config.js
    |- tailwind.config.ts
    |- tsconfig.json
```

<br />

## Getting Started

1. Make sure **Git** and **NodeJS** is installed.
2. Clone this repository to your local computer.
3. Create `.env.local` file in root directory.
4. Contents of `.env.local`:

```bash
# .env.local

NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=pk_test_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
CLERK_SECRET_KEY=sk_test_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx

NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_OUT_URL=/sign-out

NEXT_PUBLIC_STREAM_API_KEY=xxxxxxxxxxxxxxx
STREAM_SECRET_KEY=xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx

```

5. Open terminal in root directory. Run `npm install` or `yarn install`.

6. Now app is fully configured 👍 and you can start using this app using `npm run dev` or `yarn dev`.

## Screenshots:

![Landing Page](/public/screenshots/landing-page.png "Landing Page")

![Modern UI/UX](/public/screenshots/modern-uiux.png "Modern UI/UX")

![Personal Room](/public/screenshots/personal-room.png "Personal Room")

![Create Meeting](/public/screenshots/create-meeting.png "Create Meeting")

![Call Logs](/public/screenshots/call-logs.png "Call Logs")

## Tech Stack

[![React JS](https://skillicons.dev/icons?i=react "React JS")](https://react.dev/ "React JS") [![Node](https://skillicons.dev/icons?i=nodejs "Node")](https://react.dev/ "Node") [![Typescript](https://skillicons.dev/icons?i=ts "Typescript")](https://www.typescriptlang.org/ "Typescript") [![Next JS](https://skillicons.dev/icons?i=next "Next JS")](https://nextjs.org/ "Next JS") [![Tailwind CSS](https://skillicons.dev/icons?i=tailwind "Tailwind CSS")](https://tailwindcss.com/ "Tailwind CSS") [![Vercel](https://skillicons.dev/icons?i=vercel "Vercel")](https://vercel.app/ "Vercel")

## Acknowledgements

Useful resources and dependencies that are used in Yoom.

- [@clerk/nextjs](https://www.npmjs.com/package/@clerk/nextjs) - Version: ^5.2.3
- [@radix-ui/react-dialog](https://www.npmjs.com/package/@radix-ui/react-dialog) - Version: ^1.1.1
- [@radix-ui/react-dropdown-menu](https://www.npmjs.com/package/@radix-ui/react-dropdown-menu) - Version: ^2.1.1
- [@radix-ui/react-popover](https://www.npmjs.com/package/@radix-ui/react-popover) - Version: ^1.1.1
- [@radix-ui/react-slot](https://www.npmjs.com/package/@radix-ui/react-slot) - Version: ^1.1.0
- [@radix-ui/react-toast](https://www.npmjs.com/package/@radix-ui/react-toast) - Version: ^1.2.1
- [@stream-io/node-sdk](https://www.npmjs.com/package/@stream-io/node-sdk) - Version: ^0.3.0
- [@stream-io/video-react-sdk](https://www.npmjs.com/package/@stream-io/video-react-sdk) - Version: ^1.2.14
- [class-variance-authority](https://www.npmjs.com/package/class-variance-authority) - Version: ^0.7.0
- [clsx](https://www.npmjs.com/package/clsx) - Version: ^2.1.1
- [lucide-react](https://www.npmjs.com/package/lucide-react) - Version: ^0.408.0
- [next](https://www.npmjs.com/package/next) - Version: 14.2.5
- [react](https://www.npmjs.com/package/react) - Version: ^18
- [react-datepicker](https://www.npmjs.com/package/react-datepicker) - Version: ^7.3.0
- [react-dom](https://www.npmjs.com/package/react-dom) - Version: ^18
- [tailwind-merge](https://www.npmjs.com/package/tailwind-merge) - Version: ^2.4.0
- [tailwindcss-animate](https://www.npmjs.com/package/tailwindcss-animate) - Version: ^1.0.7
- [@types/node](https://www.npmjs.com/package/@types/node) - Version: ^20
- [@types/react](https://www.npmjs.com/package/@types/react) - Version: ^18
- [@types/react-datepicker](https://www.npmjs.com/package/@types/react-datepicker) - Version: ^6.2.0
- [@types/react-dom](https://www.npmjs.com/package/@types/react-dom) - Version: ^18
- [eslint](https://www.npmjs.com/package/eslint) - Version: ^8
- [eslint-config-next](https://www.npmjs.com/package/eslint-config-next) - Version: 14.2.5
- [postcss](https://www.npmjs.com/package/postcss) - Version: ^8
- [tailwindcss](https://www.npmjs.com/package/tailwindcss) - Version: ^3.4.1
- [typescript](https://www.npmjs.com/package/typescript) - Version: ^5

<!-- ## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details. -->
