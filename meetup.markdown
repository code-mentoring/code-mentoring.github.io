---
layout: page
title: Meetup
permalink: /meetup/
---

Hi, we have a meetup group!
And you're very welcome to join us.

<h2>Upcoming Events</h2>
<div id="upcoming-events-dublin">
    <h3>Dublin</h3>
</div>
<div id="upcoming-events-toronto">
    <h3>Toronto</h3>
</div>
<div id="upcoming-events-melbourne">
    <h3>Melbourne</h3>
</div>
<div id="upcoming-events-medellin">
    <h3>Medellín</h3>
</div>

<script>
    let options = { weekday: 'long', year: 'numeric', month: 'long', day: 'numeric', timeZoneName: 'short', hour: 'numeric' };
    function showLinks(id, data){
        let event = {
            name: data.name,
            link: data.link,
            time: new Date(data.time).toLocaleString('en-US', options)
        }
        if (!document.querySelector(`#${id}`)) return
        
        document.querySelector(`#${id}`).insertAdjacentHTML('beforeend', `
          <a href="${event.link}" target="_blank" rel="noopener noreferrer">${event.name}</a>
          <div>${event.time}</div>
          <br>
        `)
    }
    
  const handleResponse = (id, res) =>  {
    response.data.forEach(data => {
      showLinks(id, data);
    })
  }  
    
  function myCallbackDublin(response) {
    handleResponse('upcoming-events-dublin', response)
  }
  function myCallbackToronto(response) {
    handleResponse('upcoming-events-toronto', response)
  }
</script>

<script type="text/javascript"
  src="https://api.meetup.com/Dublin-Code-Mentoring/events?page=4&callback=myCallbackDublin"></script>
<script type="text/javascript"
  src="https://api.meetup.com/Toronto-Code-Mentoring/events?page=4&callback=myCallbackToronto"></script>
