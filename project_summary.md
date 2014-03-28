# Clairvoyant - Embrace Human Diversity
*(Clairvoyant - French: clear vision)*

## Authors
- Abiel M. Woldu      (MSc. Computer Science) - https://github.com/Abiel
- Degol S. Woldegaber (MSc. Computer Science)
- Yohannes K. Russom  (MSc. Computer Science)
- Zeregaber M. Woldu  (MSc. Hydraulic Engineering)

## Description
Clairvoyant 1.0
Our diversity, is a feature that could bring variety in our understanding of our socio-cultural interactions, our perception and value of the planet we live in. Unfortunately, diversity is also the root of racism and people not appreciating the difference in others.
Clairvoyant - A spherical ball - an outdoor installation (radius 2 meters) with rotating map on it that visually takes a user to any part of the world to show a city, the diversity of people in the city and other features of that area.


A user comes close to the sphere and names a city (verbally in any language) - a microphone in the base of the sphere processes the speech and translates it to English text and feeds the data to Google maps API and get the coordinates of the venue/city. The sphere rotates to that location and zooms in to display features of the venue as well as a set of pictures that depict the social diversity of people in that area.

When no input is fed to Clairvoyant, it rotates to show the rotation of the planet around its axis

Clairvoyant 2.0 
Multiple clairvoyant installations in different cities enabling different people to exchange hand-waves, smiles and friendly gestures.


## Purpose
The purpose of Clairvoyant project is to use art and technology to embrace diversity and cultural differences and help people to discover other parts of the world, and the cultural diversity there. It is a small attempt at motivating fraternity among people in different parts of the planet.

## Challenges
1. Hardware setup of glass or plastic sphere.
2. 3 to 4 projectors that cover sections of the sphere projecting google maps or map of the earth.
3. Voice to Text Module.
4. Google maps API and streaming map video/images 30 frames/sec ?
5. Sync between multiprojectors to cover certain sections of the globe in relation to what the user sees.


## Interaction
A user comes to one side of the clairvoyant (sphere is rotating* at this moment). The user calls out a city/country/venue name. The sphere stops at that Geo-location and zooms in to display detailed features of what was called. Down below the array of monitors display images of cultural/social diversity, popular spots and history of that Geo-location.


## Links to External Libraries and References
http://kml-samples.googlecode.com/svn/trunk/interactive/index.html#./Lines_and_Paths/Line_Strings.Tessellated.kml
https://developers.google.com/maps/web/
https://github.com/The-Shadow/java-speech-api


