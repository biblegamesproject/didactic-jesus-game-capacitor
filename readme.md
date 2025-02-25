# DIDACTIC JESUS GAME

<p align="center">
  <img src="./demo.gif" alt="" width="400" />
</p>

This project if the mobile app Didactic Jesus Game, a role-playing game where you will learn, read and see everything that Jesus did and said for you.
You will find it in the stores:
- [Apple App Store](https://apps.apple.com/us/app/didacticjesusgame/id1671402476)
- [Android Play Store](https://play.google.com/store/apps/details?id=com.biblegamesproject.didacticjesusgame&pli=1)

The app is based on a web app created with [RPG Maker](https://www.rpgmakerweb.com). The entire project [here](https://github.com/biblegamesproject/didactic-jesus-game).

Finally, check out the [Bible Games Project](https://biblegamesproject.com)!

# WIKI

### INIT CAPACITOR
- npm install
- Create www directory
- Copy all rpgmaker project inside wwww
- npx cap add android
- npx cap add ios
- npx cap sync
- npx cap open android / ios

---

### ICON/SPLASH
1. npm install capacitor-resources
2. Create the folder which is named resources under the root of your capacitor based project
3. Add your icon.png (1024x1024 px) and splash.png (2732x2732 px)
4. Add to your package.json a script definition:
"scripts": {
   "resources": "capacitor-resources -p android,ios"
}

5. npm run resources

---

### RELEASE ANDROID
- npx cap sync android
- Change build number and version name
  - android/app/build.gradle
- Set the .jks inside android folder
- npx cap build --keystorepath path --keystorepass password --keystorealias alias --keystorealiaspass password android
