# 3D Binaural Audio

***This repository contains the code for the project "3D Binaural Audio" using ARCore for Android.***

# Requirements

**1. Android Studio [Latest]**

**2. Java [Latest]**

**3. Android Phone with ARCore Support**

# Usage

Download the code as a .zip file or clone this repository using:

```
git clone https://github.com/anujdutt9/3D-Binaural-Audio.git
```

## Use pre-built APK

To install the pre-built apk, download the APK from [here](https://github.com/anujdutt9/3D-Binaural-Audio/blob/master/APK/BinauralAudio.apk) and install it on your phone. Once the app is installed, follow steps 7 to 11 as mentioned below.

***NOTE: This APK has been built and tested on Google Pixel and Google Pixel 2 XL.***

## Build App using Code

**1.** To build this app, open this project in Android Studio using:

```
File
|_ Open
   |_ Open Existing Project
```

**2.** Clean the project files using:

```
Build
|_ Clean Project
```

**3.** Rebuild Project using:

```
Build
|_ Rebuild Project
```

**4.** Connect your Android phone, **with BT headphones connected**, to your laptop and click on "Run".

**5.** Select your device from the list of device and run the app.

**6.** Now the app should get installed in your phone.

**7.** Open the app, provide "Camera Access" and start scanning any surface like floor, table top etc. until the AR mesh appears on the surface.

**8.** Once the AR mesh appears on your screen, click anywhere on the screen and an "AR Android Object" should appear on the screen.

**9.** Now you should hear some bells audio coming from the "AR Android Object".

**10.** Try moving close or far from the obeject and you will notice that the Volume level of audio changes.

**11.** With the "AR Android Object" in front on the screen, try rotating slowly in clockwise or anticlockwise direction and you should see that the audio volume is high in the headphone side that faces the "AR Android Object" and is lower on the other side.

This effect causes an illusion of audio coming from the source while we move around spatially.

# Use Custom Audio File

To use the custom audio file as audio source, go to [file](https://github.com/anujdutt9/3D-Binaural-Audio/blob/master/app/src/main/assets/):

```
app
|_ src
   |_ main
      |_ assets
         |_ drop_custom_audio_file_here.wav
```

and paste the audio file under "assets".

***NOTE: Make sure the audio file is a 32-bit Mono audio wav file as this is the format supproted by Android VR Audio Engine.***

Then, access the code file [here](https://github.com/anujdutt9/3D-Binaural-Audio/blob/master/app/src/main/java/com/google/ar/core/examples/java/helloar/BinauralAudio.java)

```
app
|_ src
   |_ main
      |_ java/com/google/ar/core/examples/java/
         |_ helloar
            |_ BinauralAudio.java
```

and change the audio file name to your audio file name on [this line](https://github.com/anujdutt9/3D-Binaural-Audio/blob/af73b43bf1e6d01d75f714bdfb576ecb6c95815e/app/src/main/java/com/google/ar/core/examples/java/helloar/BinauralAudio.java#L98) in the code.

# References

Base "Hello AR" app code from Google ARCore examples.
