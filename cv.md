---
layout: page
title: CV
permalink: /cv/
---

For my full CV, please refer to <a href="https://stackoverflow.com/story/timcluyts" target="_blank">my Stackoverflow CV</a> or <a href="https://www.linkedin.com/in/tim-cluyts" target="_blank">my linkedIn account</a>

<div class="leftBox">
    <div class="mainNode"></div>
    <div class="secondaryNode">
        <div class="textNode">C#</div>
    </div>
</div>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.10.2/jquery.min.js"></script>
<script type="text/javascript">
$('.secondaryNode').click(function() {
    var element = $('.secondaryNode');   
    if (!element.hasClass('show')) {
        element.removeClass('hide');        
        element.addClass('show'); 
        element.before(element.clone(true)).remove();
    } else {
        element.removeClass('show');        
        element.addClass('hide');
        element.before(element.clone(true)).remove();
    }    
})
</script>
<!-- 
<svg version="1.1"
     baseProfile="full"
     width="550" height="400"
     xmlns="http://www.w3.org/2000/svg">
    <g id="mainNodeTechnologies">
        <circle cx="50%" cy="25%" r="80" class="mainNode"/>
        <text x="50%" y="25%" font-size="25" transform="rotate(-20, 285, 100)" text-anchor="middle" fill="white">
            <tspan>Technologies</tspan>
        </text>
    </g>
    <g class="secondaryNodeTechnologies">
        <circle cx="75%" cy="32%" r="40" class="secondaryNode"/>
        <text x="75%" y="32%" font-size="20" transform="rotate(15, 385, 130)" text-anchor="middle" fill="white">
            <tspan>NodeJS</tspan>
        </text>
    </g>
    <g class="secondaryNodeTechnologies">
        <circle cx="10%" cy="17%" r="40" class="secondaryNode"/>
        <text x="10%" y="17%" font-size="20" transform="rotate(-10, 80, 60)" text-anchor="middle" fill="white">
            <tspan>SQL</tspan>
        </text>
    </g>
    <g class="secondaryNodeTechnologies">
        <circle cx="18%" cy="55%" r="40" class="secondaryNode"/>
        <text x="18%" y="55%" font-size="20" transform="rotate(12, 80, 215)" text-anchor="middle" fill="white">
            <tspan>ReactJS</tspan>
        </text>
    </g>
    <g class="secondaryNodeTechnologies">
        <circle cx="50%" cy="65%" r="40" class="secondaryNode"/>
        <text x="50%" y="65%" font-size="20" transform="rotate(-14, 300, 260)" text-anchor="middle" fill="white">
            <tspan>.NET</tspan>
        </text>
    </g>
</svg>-->

<!-- 
<svg version="1.1"
     baseProfile="full"
     width="550" height="400"
     xmlns="http://www.w3.org/2000/svg">
    <g id="mainNodeProjects">
        <circle cx="50%" cy="25%" r="80" class="mainNodeSecondary"/>
        <text x="50%" y="25%" font-size="25" transform="translate(-17 105) rotate(-20)" text-anchor="middle" fill="white">
            <tspan>Projects</tspan>
        </text>
    </g>
</svg> -->

<div class="technologiesSubDiv">
    <div class="inner">
        <div class="title">
            Here be some text
        </div>
    </div>
</div>