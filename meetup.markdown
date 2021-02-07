---
layout: page
title: Meetup
permalink: /meetup/
---

Hi, we have a meetup group

You can Meet us online at: [meetup](https://www.meetup.com/de-DE/Dublin-Code-Mentoring/)

Or meet us live at [Dublin](https://www.meetup.com/Dublin-Code-Mentoring/) and [Toronto](https://www.meetup.com/Toronto-Code-Mentoring/)

<h2>Upcoming Events</h2>
<div id="upcoming-events-dublin">
    <h3>Dublin</h3>
</div>
<div id="upcoming-events-toronto">
    <h3>Toronto</h3>
</div>
<script>
  function myCallbackDublin(response) {
    response.data.forEach(data => {
      let date = new Date(data.time)
      let options = { weekday: 'long', year: 'numeric', month: 'long', day: 'numeric', timeZoneName: 'short', hour: 'numeric' };
      let event = {
        name: data.name,
        link: data.link,
        time: date.toLocaleString('en-US', options)
      }
      if (!document.querySelector('#upcoming-events-dublin')) return
      document.querySelector('#upcoming-events-dublin').insertAdjacentHTML('beforeend', `
      <a href="${event.link}" target="_blank" rel="noopener noreferrer">${event.name}</a>
      <div>${event.time}</div>
      <br>
      `
      );
    })
  }
  function myCallbackToronto(response) {
    response.data.forEach(data => {
      let date = new Date(data.time)
      let options = { weekday: 'long', year: 'numeric', month: 'long', day: 'numeric', timeZoneName: 'short', hour: 'numeric' };
      let event = {
        name: data.name,
        link: data.link,
        time: date.toLocaleString('en-US', options)
      }
      if (!document.querySelector('#upcoming-events-toronto')) return
      document.querySelector('#upcoming-events-toronto').insertAdjacentHTML('beforeend', `
      <a href="${event.link}" target="_blank" rel="noopener noreferrer">${event.name}</a>
      <div>${event.time}</div>
      <br>
      `
      );
    })
  }
</script>
<script type="text/javascript"
  src="https://api.meetup.com/Dublin-Code-Mentoring/events?page=4&callback=myCallbackDublin"></script>
<script type="text/javascript"
  src="https://api.meetup.com/Toronto-Code-Mentoring/events?page=4&callback=myCallbackToronto"></script>