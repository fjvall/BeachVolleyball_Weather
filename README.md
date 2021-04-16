This project focuses on determining if weather conditions affect Beach Volleyball's main game stats (kills, errors, aces, etc) in a meaningful way and quantify it. I began by gathering information and assumptions from my own experience in playing beach volleyball, from semi-professional volleyball player contacts ,and later I created a game/weather dataset using an open source professional games dataset and adding the weather at the time of play using gps coordinates and a external API.  After this, I decided to test the following hypothesis using multivariate regression analysis: <br>
1-    Higher wind speed increases the probability of Aces per point played. Serves performed when there is a higher wind speed causes the ball to land sooner. <br>
2-    Location features may affect the probability of Kills per point played. (For instance, sand depth might affect the number of kills by making it harder to jump). <br>
3-    Rain increases the probability of Serve Errors. <br>
4.1-  Higher temperatures may affect the probability of Errors per point played. <br>
4.2-  Minutes played at higher temperatures affect the probability of Errors per point played. As this may cause increased fatigue in players. <br>
5-    Humidity increases the probability of Kills per point played. Moisture/rain packs sand which can make it easier to jump, thus, creating better conditions for kills. <br>
6-    Lower atmospheric pressure increases the number of unforced Errors by hitting the ball out-of-bounds more often.



I generate the Dataset using the following:
Github repository with games data: https://github.com/BigTimeStats/beach-volleyball
Google's map geocoding to get the GPS
Visualcrossing API to get Historic data using date and GPS coordinates: https://www.visualcrossing.com/weather-api
