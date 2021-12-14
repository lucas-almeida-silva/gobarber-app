<div style="display: flex; justify-content: center;">
   <img src=".github/gobarber-logo.jpg" alt="GoBarber" width="100%"/>
</div>

# :page_with_curl: Table of Contents

* [About](#information_source-about)
* [Technologies](#computer-technologies)
* [Features](#rocket-features)
* [How to run](#seedling-how-to-run)
* [License](#pencil-license)

# :information_source: About

GoBarber is a application to make appointments with hairdressers or barbers. The application has [Web](https://github.com/lucas-almeida-silva/gobarber-web) and mobile versions, that was developed during the bootcamp GoStack offered by RocketSeat. This is the mobile project, that consumes GoBarber [API](https://github.com/lucas-almeida-silva/gobarber-api).

# :computer: Technologies

- [React Native](https://reactnative.dev/)
- [TypeScript](https://www.typescriptlang.org/)

# :rocket: Features

### Users

- Create an user
- Update user avatar
- Update user profile
- Login and logout
- Recover password

### Clients

- List providers.
- List the availability of a provider in a month (whether or not there are times available on each day of the month).
- List the availability of a provider in a day (available and unavailable times).
- Create an appointment.

### Providers

- List the appointments of a day.

# :seedling: How to run

```bash
# Clone the repository
$ git clone https://github.com/lucas-almeida-silva/gobarber-app.git

# Go to the project folder
$ cd gobarber-app

# Install Dependencies
$ yarn
# or npm install

# Run the application
$ yarn android
# or yarn ios
# or npx react-native run-android
# or npx react-native run-ios
```
You need to have a simulator or you can use your smartphone connected through the USB cable.
Also, you need to change the baseURL in the file **src/services/api.ts** based in how you are running the application. This is the file that has the configuration to access the API.

-   IOS with emulator: localhost
-   IOS with smartphone: machine IP or run the command `adb reverse tcp:3333 tcp:3333`
-   Android with emulator: localhost, but its necessary to run the comand `adb reverse tcp:3333 tcp: 3333`
-   Android with emulator: run the command `adb reverse tcp:3333 tcp: 3333` ou use the IP 10.0.2.2 for Android Studio Emulator or the IP 10.0.0.2 for Genymotion emulator.
-   Android with smartphone: machine IP or run the command `adb reverse tcp:3333 tcp:3333`

OBS: 3333 it's the port of the localhost that the API runs.

# :pencil: License

This project is under the [MIT license](LICENSE).
