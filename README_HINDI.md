# ZYRON Android Project — Hindi Guide

## Is version mein kya hai
- Android app ka native Kotlin source code
- Dark ZYRON chat interface
- Mic button se speech recognition (phone ke speech service par nirbhar)
- Android Text-to-Speech replies
- Basic offline replies
- Optional OpenAI-compatible `/chat/completions` API settings

## Important limitations
- “Hello Bro” phrase ko app khuli hone par mic button se bolkar recognize kiya ja sakta hai.
- Ye build background always-listening wake-word service implement nahi karta.
- Online AI tabhi chalega jab tum apna endpoint, model aur API key add karoge. API key free ya unlimited hona guaranteed nahi hai.
- API key app ke local preferences mein save hoti hai; production app ke liye secure backend behtar hai.
- Hindi/Odia speech recognition aur TTS phone mein installed speech engine/language support par depend karta hai.

## APK kaise build karein
Is project ko Android Studio wale computer par open karke:
1. Gradle sync hone dein.
2. Build > Build Bundle(s) / APK(s) > Build APK(s) chunein.
3. APK `app/build/outputs/apk/debug/app-debug.apk` mein milega.

## Android phone only
Sirf phone se APK build karna mushkil ho sakta hai. Android par browser se GitHub Codespaces ya kisi cloud Android build service ka use karna pad sakta hai; availability/free limits badal sakti hain. Project ZIP ko pehle download/extract karke compatible cloud build environment mein upload karein.

## Build prerequisites
- Android Gradle Plugin 8.7.3
- Kotlin Android plugin 2.0.21
- JDK 17
- Android SDK platform 35

## Safety
API key kisi ko share mat karna. Unknown API providers par key enter karne se pehle unki privacy aur billing terms check karo.
