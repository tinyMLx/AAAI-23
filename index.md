---
title: false
---
<!-- <figure class="figure">
  <center>
  <img src="{{ site.baseurl }}/assets/cover.png" alt="cover banner art" class="vid-fluid rounded center">
  </center>
</figure> -->

## Building Approachable, Hands-On Embedded Machine Learning Curriculum Using Edge Impulse and Arduino

<div class="message">
  <a href="https://aaai.org/Conferences/AAAI-23/aaai23tutorials/">A Tutorial and Lab Forum at AAAI-23</a>.
</div>

Embedded machine learning (ML) is the process of running machine learning algorithms on low-cost, resource-constrained microcontrollers and single board computers and is currently used to solve unique problems in industry and academia. As a result, there is a growing demand to teach embedded ML in higher education institutions to prepare developers, engineers, and researchers for these emerging data-driven approaches.

This lab provides hands-on experience creating an end-to-end embedded ML system using a combination of Edge Impulse and Arduino. In the lab, we will create and deploy a full image classification system by performing data collection using Arduino, model training with Edge Impulse, and live inference with Arduino. This will provide researchers and educators with the knowledge and tools to develop an approachable curriculum around embedded ML.  

Attendees should have an interest in finding ways to make ML easier and approachable to students, especially those outside of the computer science field. Such attendees could be professors or lecturers from other disciplines or those teaching ML in cross-cutting programs. Some programming experience will be needed (ideally C/C++ or Arduino). No machine learning experience is required.

### Schedule

<div id = "LOCAL_TIME"></div><br/>

{% include schedule_table table_data = site.data.schedule %}

<script>
  // top time
  var start = new Date('02/08/2023 08:30:00 AM EST');
  var end = new Date('02/08/2021 12:30:00 PM EST');
  var localTime = start.toLocaleTimeString([], {timeStyle: 'short'}) + " to " + end.toLocaleTimeString([], {timeStyle: 'short'});
  var startString = "The workshop will run from <b>8:30 am – 12:30 pm EST which is "
  var endString = " in your local timezone</b> (according to your computer system time). Times below adjusted to that time zone. Exact timing and topics subject to change."
  document.getElementById('LOCAL_TIME').innerHTML = startString + localTime + endString;
  
  // all times
  var timeElements = document.getElementsByClassName("GMT_TIME");
  for (var i = 0; i < timeElements.length; i++) {
    dateStr = '02/08//2021 ' + timeElements[i].innerHTML + ' EST';
    var gmt_time = new Date(dateStr);
    if (isNaN(gmt_time)) { // d.getTime() or d.valueOf() will also work
      // date object is not valid so add timezone note
      timeElements[i].innerHTML = timeElements[i].innerHTML + ' EST';
    } else {
      // date object is valid so convert to local time
      timeElements[i].innerHTML = gmt_time.toLocaleTimeString([], {timeStyle: 'short'});
    }
  }
</script>

### Team
{% for person in site.data.team.people %}
{% include team_person person = person %}
{% endfor %}

### Registration
Register for our tutorial and lab form through the main [**AAAI-23 website**](https://aaai.org/Conferences/AAAI-23/registration/).

### Supporters
We would like to thank [**ICTP**](https://www.ictp.it/), [**Harvard SEAS**](https://www.seas.harvard.edu/), and the [**tinyML Foundation**](https://www.tinyml.org/) for their continued support of TinyML educational content!

### Questions?
Contact [edu@tinyml.org](mailto:edu@tinyml.org) with any questions regarding this workshop.