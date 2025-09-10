# TRMNL
Collection of TRMNL Plugins, images etc.

# XWeather
This is an Open Source plugin for TRMNL. 
This Plugin will work with many personal weather stations including Ecowitt and Tempest. 
Any weather station that can publish to "PWS weather" or can transmit data to XWeather should work.

## Setup Your Station Example
First setup a <a href="https://www.pwsweather.com/">PWS Weather </a> account, then setup an <a href="https://www.xweather.com/weather-api">XWeather account</a>. Then you will need to link your PWS Weather account to your XWeather account to gain free access to their API.

If your weather station cannot publish directly to PWS Weather, create a PWS Weather account and add a new PWS. Using something like a Tempest or Ecowitt Weather station (Or other Weewx supported weather station) on your local network, have a server such as a Raspberry Pi running Weewx.

<a href="https://weewx.com/">Weewx </a> has many plugins to connect to weather stations hubs. Plugins can interface by intercepting UDP packets or query the station hub/console rest endpoints. These steps will vary, but by installing and configuring existing plugins weewx can publish to PWS weather (other online weather services as well).

Configure Weewx to publish your weather station data to the virtual PWS Weather station you created. Once PWS Weather activates your station (It will take some time), you can link it to your XWeather account. At this point you will add an "App" in XWeather. The "App" will allow you access, and will provide you with a Client ID and Secret token. Plug these into this plugin's setting for your TRMNL and you can use your TRMNL to see your private weather station data displayed. Feel free to reach out in the TRMNL Discord if you need help. This plugin uses a combination of Weather Icons provided by TRMNL and by <a href="https://github.com/erikflowers/weather-icons">Erik Flowers</a>.
