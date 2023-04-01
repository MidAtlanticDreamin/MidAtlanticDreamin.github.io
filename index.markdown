---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: core
title: "MidAtlantic Dreamin’"
---
<div class="container-flex">
        {% include homepage-jumbo.html
                conferencetag = ""
                conferencename = "MidAtlantic Dreamin’"
                when = "WHEN"
                date = "May 8, 2023"
                time = "9am &mdash; 6pm"
                where = "WHERE"
                city = "Philadelphia, PA"
                venue = "City Winery"
        %}

        <div id="tile_description" class="container widget tile">
	<h2>Brewed in Philly, Shared with the Ohana</h2>
	<h3></h3>
        <p>Mid-Atlantic Dreamin’ is a community-led conference for professionals with a passion for the Salesforce platform. The event is focused on deep technical content for experienced Developers, Configurators, and Architects on the Platform.</p>
        <p>Our purpose is to elevate the skills and broaden the platform knowledge of all attendees by bringing together the best and brightest technical talent the Salesforce Ohana has to offer.</p>
        <p>Our goal is for each attendee, including non-Salesforce technical professionals, to increase their knowledge and raise their skill level.</p>
        </div>

        <!-- {% include tiles-speaker.html 
                title = "Keynote Speakers"
        %} -->

        {% include tiles-sponsor.html 
                title = "Sponsors"
                homepage = true
        %}

</div>
