---
layout: base
title: "Agenda"
description: "" 
published: true
---

<div class="schedule">
    <div class="clearfix"></div>
    <div class="sessions list">
        <div class="followWrap" style="height: 60px;">
            <div class="day-floating"><span>May 8, 2023</span></div>
        </div>
        {% assign sessions = site.sessions | sort: "order" %}
        {% for session in sessions %}
        {% include session.html
                time = session.time
                title = session.title
                location = session.location
                speakers = session.speakers
                url = session.url
                output = session.output
        %}
        {% endfor %}
    </div>
</div>