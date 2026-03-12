WARNING - Socialite is in DEVELOPEMENT!! Install at your own risk. I AM NOT RESPONSIBLE FOR YOUR STUPIDITY!

BUILD INSTRUCTIONS (macOS on INTEL ONLY!!(NOT APPLE SILICON OR POWERPC!!!!!)):
  HOW TO RUN SOCIALITE LOCALLY IN WEB BROWSER VIA NPM
    $bash
      cd /path/to/Socialite
      npm install
      npm run dev

    Open `http://localhost:3000` in your browser! :)

  HOW TO COMPILE IN ANDROID STUDIO
    Requisites:
      Android Studio
      npm AND node.js
      Java SDK 11 or later!! Oracle has it 
      A boatload of others (NPM will take care of that)
    Okay. You have that. Now what?
        $bash
          cd /path/to/Socialite
          sudo npm install  
          sudo npm run build
          sudo npx cap add android 
          sudo npx cap sync android 
          sudo npx cap open android 
          sudo npm run build

        In Android Studio:
        
        1. Wait for Gradle sync** to complete (first time can take 5-10 minutes)
        2. Go to **Build** → **Build Bundle(s) / APK(s)** → Build APK(s)
        3. Wait for the build to complete
        4. Click **locate** in the notification to find your APK file
        
        The APK will be located at:
        android/app/build/outputs/apk/debug/app-debug.apk
