---
layout: post
title:  "CV"
author: Tim Cluyts
color: red
width:   3 
height:  1
date:   2016-03-30 11:31:49 +0200
categories: info
permalink: cv
isMain: true
---
<div class="row">
    <div class="col-xs-12">
        <div class="btn-group btn-group-lg btn-group-justified" data-toggle="buttons">
            <label class="btn btn-primary ">
                <input type="radio" name="options" id="showTimeline" autocomplete="off"  /> Timeline
            </label>
            <!--<label class="btn btn-primary active">
                <input type="radio" name="options" id="showTechnologies" autocomplete="off"  checked/> Technologies
            </label>-->
            
        </div>
    </div>
</div>
<div class="timeline" id="experienceTimeline">
    {% for employer in site.data.exp %}
        <span class="timeline-label ">
                <h1><span class="label label-info">{{ employer.Company }}</span></h1>
        </span>
        {% assign start = employer.StartDate | date: "%Y" %} 
        {% assign end = employer.EndDate | default : "now" | date: "%Y" %} 
        {% if employer.Projects.size == 1 %}
            <span class="timeline-label ">
                        <h3><span class="label label-success">from {{ start }} until {{ end }}</span></h3>
            </span>
            {% for project in employer.Projects %} 
                {% include projectTimeline.html %} 
            {% endfor %} 
        {% else %} 
            {% for year in (start..end) reversed %}
                <span class="timeline-label ">
                    <h3><span class="label label-success">{{ year }}</span></h3>
                </span>
                {% for project in employer.Projects %} 
                    {% assign projectStart = project.StartDate | date : "%Y" | round %} 
                    {% if projectStart == year %} 
                        {% include projectTimeline.html %} 
                    {% endif %}
                 {% endfor %} 
            {% endfor %} 
        {% endif %} 
    {% endfor %}
</div>
<script>  
jQuery(document).ready(function() {
    $('#showTimeline').on('change', function () {
        $("#calendarView").hide();
        $("#technologies").hide();
        $("#experienceTimeline").show();
    });  
});
</script>