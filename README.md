# Sofia-Traffic-HA
Virtual tables for Arrival times of public transport vehicles<br> HOME ASSISTANT
[![telegram_badge]][telegram_link]

[telegram_badge]: https://img.shields.io/badge/telegram-❤️-252850?style=plastic&logo=telegram
[telegram_link]: https://t.me/+5G1uRKFbmStmNTQ0

> get results via RESTful json parse  <br>
> /search_all?term=22 <br>
> /lines/stops/geo?line_id=389
> <br>
>/transports/json <br>
> /lines/json/<br>
> /virtual_panel?stop_id=1714 <br>
https://routes.st.bg/resources/stops-bg/en.json <br>
/interactivecard/stops/geo?bbox=25,51,27,53.json
<h1>Table of contents</h1><br>
Installation | Configuration | Full example | Help | Contribution
<br><br>
<h1>Screenshots and features</h1>
<br>

<h1>Installation<h1>
<br>
  <summary> Оставащи минути до пристигане 
  <details>
 **{{ state_attr('sensor.tm22' , 'departure_time') }}** {{
        ((now().hour * 60) + now().minute) - 
        ((strptime(states('sensor.tm22'), '%H:%M').hour * 60) +
        strptime(states('sensor.tm22'), '%H:%M').minute) }} минути  
    

<h1>Configuration</h1>
  <br>
<h1>Help</h1>
[JsonPathFinder](https://jsonpathfinder.com/)
