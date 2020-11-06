# Next Level Week week v1

Project of Next Level Week organized by @rocketseat

# Description

The next level week is designed as sequence of video-tutorials in one week aimed at using NodeJS + React + React Native stack to build a real application.

The proposed app is called "Ecoleta". Its allows people to register an ecopoint (exclusively via the frontend) and input their location, contect data, location and items that point collects. In the mobile app, it is possible to filter ecopoints by their location (UF/City) and items. Also, it is possible to contact the ecopoint via e-mail or whatsapp, properly deep-linked. As this project was an demo project it lacks proper authentication, or editing capabilities.

# Building

## Backend
Backend is developed with NodeJS and Sqlite3. To start the API, run `yarn dev` or `npm dev`. The default port is 3333 and can be changed in [server.ts](server/src/server.ts). To run with the mobile version, please also change the `image_url` value in [itemsController.ts](server/src/controllers/itemsController.ts), line 12, and [pointsController.ts](server/src/controllers/pointsController.ts), lines 25 and 90.

## Web frontend
Frontend is a React app created with create-react-app and is located in folder `web`. Frontend can also be started running `yarn start` or `npm start`. If you are not using the default address/port for the server please change them in [api.ts](web/src/services/api.ts). Default port for web interface is 3000.

## Mobile frontend
The mobile frontend was build using React Native with @expo/expo. Before starting, change `baseURL` in [api.js](mobile/src/services/api.ts) to point to your local ip address. After that, run `yarn start` or `npm start` to start the server. If you are using your own mobile to test, you'll need expo app installed. After starting an QR code will be shown, scan it with the expo app and expo will automatically bundle and send the javascript to your phone.

# PRs

Feel free to fork and contribute with PRs and/or open issues. But keep in mind this projects lacks several features on purpose as it is an demo project.

See the License in [LICENSE](LICENSE)