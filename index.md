---
# More detailed instructions (including how to fill these variables for an # online workshop) are available at https://carpentries.github.io/workshop-template/customization/index.html#yaml-header
# Required variables
venue: "UC OSPO Network (Online)"
address: "online"
country: "us"
language: "en"
latitude: "34.0700"
longitude: "-118.4440"
humandate: "Licensing LOCKED: Thu 8/27 (afternoon) + Fri 8/28 (full day), 2026. Stewards: TBD, may join same session or a later week"
humantime: "Thu: afternoon PT, exact time TBD. Fri: full day PT, exact times TBD"
startdate: 2026-08-24
enddate: 2026-08-28
instructor: ["Tim Dennis (UCLA / UC OSPO Network)"]
helper: []
email: ["tdennis@library.ucla.edu"]
# Optional variables
collaborative_notes:
eventbrite:
what3words:
# DON'T CHANGE THIS
layout: workshop
---

{% assign isOfficial = site.official_curricula | has: site.carpentry %}

{% if page.venue == "FIXME" or
      page.address == "FIXME" or
      page.country == "FIXME" or
      page.language == "FIXME" or
      page.latitude == "FIXME" or
      page.longitude == "FIXME" or
      page.humandate == "FIXME" or
      page.humantime == "FIXME" or
      page.startdate == "FIXME" or
      page.enddate == "FIXME" %}
      {% assign fixmes = true %}
{% endif %}

{% comment %} See instructions in the comments below for how to edit specific sections of this workshop template. {% endcomment %}

{% comment %}
HEADER

Edit the values in the block above to be appropriate for your workshop.
If the value is not 'true', 'false', 'null', or a number, please use double quotation marks around the value, unless specified otherwise.
And run 'make workshop-check' *before* committing to make sure that changes are good.
{% endcomment %}

{% if fixmes %}
<div class="alert alert-danger">
    <p>
        This is the Carpentries workshop template. Fill in the required variables as described in the <a href="{{site.url}}{{site.baseurl}}/customization/index.html#yaml-header">customisation</a> instructions to remove this message.
    </p>
    <p>
        If you are running a self-organized workshop or have not put in a workshop request yet, please also fill in <a href="{{site.amy_site}}/forms/self-organised/">this workshop request form</a> to let us know about your workshop and our administrator may contact you if we need any extra information.
    </p>
    <p>
        If this is a pilot workshop for a new lesson, set the <code>pilot</code> field to <code>true</code> in <code>_config.yml</code>.
        For workshops teaching a lesson in The Carpentries Incubator, remember to uncomment and supply values for <code>incubator_lesson_site</code>, <code>incubator_pre_survey</code>, and <code>incubator_post_survey</code> fields in <code>_config.yml</code>.
    </p>
</div>
{% endif %}


{% comment %}
Check DC curriculum
{% endcomment %}

{% if site.carpentry == "dc" %}
{% unless site.curriculum == "dc-astronomy" or site.curriculum == "dc-ecology" or site.curriculum == "dc-genomics" or site.curriculum == "dc-geospatial" or site.curriculum == "dc-image" or site.curriculum == "dc-socsci" %}
<div class="alert alert-warning">
It looks like you are setting up a website for a Data Carpentry curriculum but you haven't specified the curriculum type in the <code>_config.yml</code> file (current value in <code>_config.yml</code>: "<strong>{{ site.curriculum }}</strong>", possible values: <code>dc-image</code>, <code>dc-astronomy</code>, <code>dc-ecology</code>, <code>dc-genomics</code>, <code>dc-socsci</code>, or <code>dc-geospatial</code>). After editing this file, you need to run <code>make serve</code> again to see the changes reflected.
</div>
{% endunless %}
{% endif %}


{% comment %}
Check SWC curriculum
{% endcomment %}

{% if site.carpentry == "swc" %}
{% unless site.curriculum == "swc-inflammation" or site.curriculum == "swc-gapminder" %}
<div class="alert alert-warning">
It looks like you are setting up a website for a Software Carpentry curriculum but you haven't specified the curriculum type in the <code>_config.yml</code> file (current value in <code>_config.yml</code>: "<strong>{{ site.curriculum }}</strong>", possible values: <code>swc-inflammation</code>, or <code>swc-gapminder</code>). After editing this file, you need to run <code>make serve</code> again to see the changes reflected.
</div>
{% endunless %}
{% endif %}


{% comment %}
EVENTBRITE

This block includes the Eventbrite registration widget if
'eventbrite' has been set in the header.  You can delete it if you
are not using Eventbrite, or leave it in, since it will not be
displayed if the 'eventbrite' field in the header is not set.
{% endcomment %}

{% if page.eventbrite %}
<strong>Some adblockers block the registration window. If you do not see the registration box below, please check your adblocker settings.</strong>
<div id="eventbrite-widget-container"></div>
<script src="https://www.eventbrite.com/static/widgets/eb_widgets.js"></script>
<script type="text/javascript">
    window.EBWidgets.createWidget({
        // Required
        widgetType: 'checkout',
        eventId: {{page.eventbrite}},
        iframeContainerId: 'eventbrite-widget-container',
    });
</script>
{% endif %}


{% comment %}
INTRODUCTION

Edit the general explanatory paragraph below if you want to change the pitch.
{% endcomment %}

<div class="row g-3 pb-3">

  <!-- left column spans 2 rows -->
  <div class="col-md-6">
    <div class="card h-100">
        <h5 class="card-header">The Carpentries</h5>
        <div class="card-body">
            <p>
            <strong><a href="https://carpentries.org">The Carpentries</a></strong> project comprises the
            <a href="{{site.dc_site}}">Data Carpentry</a>,
            <a href="{{site.hpcc_site}}">High-Performance Computing Carpentry</a>,  
            <a href="{{site.lc_site}}">Library Carpentry</a>, and
            <a href="{{site.swc_site}}">Software Carpentry</a>
             communities of Instructors, Trainers, Maintainers, helpers, and supporters who share a mission to teach foundational computational and data science skills to researchers.
            </p>
            {% assign intro_file = site.carpentry | append: '/intro.html' %}
            {% if isOfficial %}
            {% include {{ intro_file }} %}
            {% endif %}
        </div>
    </div>
  </div>

  <!-- right column with two stacked cards -->
  <div class="col-md-6 d-flex flex-column gap-3">
    <div class="card flex-fill">
        <h5 class="card-header">Carpentries Clippings</h5>
        <div class="card-body">
        <p class="text-center">
        <strong>Want to learn more and stay engaged with The Carpentries?</strong>
        </p>
        <p class="text-center">
        Carpentries Clippings is The Carpentries' monthly newsletter, where we share community news, community job postings, and more.
        </p>
        <p class="text-center">
            <a href="https://carpentries.org/newsletter/">
                <button type="button" class="btn btn-success">Sign up to our newsletter</button>
            </a>
        </p>
      </div>
    </div>
    <div class="card flex-fill">
      <h5 class="card-header">Code of Conduct</h5>
      <div class="card-body">
        {% comment%}
        CODE OF CONDUCT
        {% endcomment %}
        <p class="text-center">
        Everyone who participates in Carpentries activities is required to conform to the <a href="https://docs.carpentries.org/policies/coc/">Code of Conduct</a>, which also outlines how to report an incident if needed.
        </p>

        <p class="text-center">
        <a href="https://goo.gl/forms/KoUfO53Za3apOuOK2">
            <button type="button" class="btn btn-info">Report a Code of Conduct Incident</button>
        </a>
        </p>
      </div>
    </div>
  </div>
</div>

{% if site.pilot %}
This is a pilot workshop, testing out a lesson that is still under development. The lesson authors would appreciate any feedback you can give them about the lesson content and suggestions for how it could be further improved.
{% endif %}


{% comment %}
LOCATION

This block displays the address and links to maps showing directions
if the latitude and longitude of the workshop have been set.  You
can use https://www.latlong.net/ to find the lat/long of an
address.
{% endcomment %}

{% assign begin_address = page.address | slice: 0, 4 | downcase  %}
{% if page.address == "online" %}
  {% assign online = "true_private" %}
{% elsif begin_address contains "http" %}
  {% assign online = "true_public" %}
{% else %}
  {% assign online = "false" %}
{% endif %}

<div class="card mb-2">
  <h5 class="card-header">Workshop Logistics</h5>
  <div class="card-body">
    <dl class="mb-0">
    <div class="row">
        <dt class="col-sm-2 col-md-2 py-2 px-3 bg-body-light text-body-secondary fw-bold">Who</dt>
        <dd class="col py-2 px-3 mx-0 mb-0">
            {% comment %}
            AUDIENCE

            Explain who your audience is.  (In particular, tell readers if the
            workshop is only open to people from a particular institution.
            {% endcomment %}
            {% assign who_file = site.carpentry | append: '/who.html' %}
            {% if isOfficial %}
            {% include {{ who_file }} %}
            {% else %}
            This is a closed cohort training for two UC OSPO Network lesson development teams (Librarians as Open Source Stewards, and Software Licensing) who have already formed and confirmed participation. It is not open for general registration.
            {% endif %}
        </dd>
    </div>
    <div class="row">
        <dt class="col-sm-2 col-md-2 py-2 px-3 bg-body-light text-body-secondary fw-bold">Where</dt>
        <dd class="col py-2 px-3 mx-0 mb-0">
            {% if page.latitude and page.longitude and online == "false" %}    
                {{page.address}}.
                Get directions with
                <a href="//www.openstreetmap.org/?mlat={{page.latitude}}&mlon={{page.longitude}}&zoom=16">OpenStreetMap</a>
                or
                <a href="//maps.google.com/maps?q={{page.latitude}},{{page.longitude}}">Google Maps</a>.
                {% if page.what3words %}
                    What3Words location:
                    <a href="https://what3words.com/{{page.what3words}}">///{{page.what3words}}</a>.
                {%endif %}
                {% elsif online == "true_public" %}
                    <p id="where">
                        Online at <a href="{{page.address}}">{{page.address}}</a>.
                        If you need a password or other information to access the training,
                        the instructor will pass it on to you before the workshop.
                    </p>
                {% elsif online == "true_private" %}
                    <p id="where">
                        This training will take place online.
                        The instructors will provide you with the information you will need to connect to this meeting.
                    </p>
                {% endif %}        
        </dd>
    </div>
    <div class="row">
        <dt class="col-sm-2 col-md-2 py-2 px-3 bg-body-light text-body-secondary fw-bold">When</dt>
        <dd class="col py-2 px-3 mx-0 mb-0">
            {% comment %}
            DATE

            This block displays the date and links to Google Calendar.
            {% endcomment %}
            {% if page.humandate %}
                <p id="when">
                    {{page.humandate}}; {{page.humantime}}
                    {% include workshop_calendar.html %}
                </p>
            {% endif %}    
        </dd>
    </div>
    <div class="row">
        <dt class="col-sm-2 col-md-2 py-2 px-3 bg-body-light text-body-secondary fw-bold">Requirements</dt>
        <dd class="col py-2 px-3 mx-0 mb-0">
            {% comment %}
            SPECIAL REQUIREMENTS

            Modify the block below if there are any special requirements.
            {% endcomment %}
            <p id="requirements">
            {% if online == "false" %}
                Participants must bring a laptop with a
                Mac, Linux, or Windows operating system (not a tablet, Chromebook, etc.) that they have administrative privileges on.
            {% else %}
                Participants must have access to a computer with a
                Mac, Linux, or Windows operating system (not a tablet, Chromebook, etc.) that they have administrative privileges on.
            {% endif %}
            They should have a few specific software packages installed (listed <a href="#setup">below</a>).
            </p>
        </dd>  
    </div>
    <div class="row">
        <dt class="col-sm-2 col-md-2 py-2 px-3 bg-body-light text-body-secondary fw-bold">Accessibility</dt>
        <dd class="col py-2 px-3 mx-0 mb-0">
            {% comment %}
            ACCESSIBILITY

            Modify the block below if there are any barriers to accessibility or special instructions.
            {% endcomment %}

            <p id="accessibility">
            We are committed to making this workshop accessible to everybody. 
            {% if online == "false" %}
                The workshop organizers have checked that:
                <br/>
                <ul>
                    <li>The room is wheelchair / scooter accessible.</li>
                    <li>Accessible restrooms are available.</li>
                </ul>
            {% endif %}
            </p>
            <p>
            We are dedicated to providing a positive and accessible learning environment for all. 
            We do not require participants to provide documentation of disabilities or disclose any unnecessary personal information. 
            However, we do want to help create an inclusive, accessible experience for all participants. 
            We encourage you to share any information that would be helpful to make your Carpentries experience accessible.
            To request accessibility support for this workshop, please fill out the 
            <a href="https://carpentries.typeform.com/to/B2OSYaD0">accessibility support request form</a>.
            If you have questions or need assistance with the accessibility support form please <a href="mailto:team@carpentries.org">email us</a>.
            </p>
            <p>
            <a href="https://glosario.carpentries.org/">Glosario</a> is a multilingual glossary for computing and data science terms.
            The glossary helps learners attend workshops and use our lessons to make sense of computational and programming jargon written in English by offering it in their native language.
            Translating data science terms also provides a teaching tool for Carpentries Instructors to reduce barriers for their learners.
            </p>
        </dd>
    </div>
    <div class="row">
        <dt class="col-sm-2 col-md-2 py-2 px-3 bg-body-light text-body-secondary fw-bold">Workshop Recordings</dt>
        <dd class="col py-2 px-3 mx-0 mb-0">
            {% comment %}
            WORKSHOP RECORDINGS

            Modify or remove the block below if you plan to record the workshop.
            {% endcomment %}
            <p id="recordings">
            We strongly recommend joining live, since this training is interactive and each session builds on the last.
            That said, we know availability across four teams and multiple time zones is a real crunch — sessions will
            be recorded, so if you have to miss one (or step out for an hour for another meeting) you can catch up on
            the recording and get a team catch-up from your cohort.
            </p>
        </dd>
    </div>
    <div class="row">
        <dt class="col-sm-2 col-md-2 py-2 px-3 bg-body-light text-body-secondary fw-bold">Contact</dt>
        <dd class="col py-2 px-3 mx-0 mb-0">
            {% comment %}
            CONTACT EMAIL ADDRESS

            Display the contact email address set in the configuration file.
            {% endcomment %}
            <p id="contact">
            Please email
            {% if page.email %}
            {% for email in page.email %}
            {% if forloop.last and page.email.size > 1 %}
            or
            {% else %}
            {% unless forloop.first %}
            ,
            {% endunless %}
            {% endif %}
            <a href='mailto:{{email}}'>{{email}}</a>
            {% endfor %}
            {% else %}
            to-be-announced
            {% endif %}
            for more information.
            </p>
        </dd>
    </div>
    
    <div class="row">
        <dt class="col-sm-2 col-md-2 py-2 px-3 bg-body-light text-body-secondary fw-bold">Workshop FAQ</dt>
        <dd class="col py-2 px-3 mx-0 mb-0">
            <p id="workshops-faq">
            For answers to frequently asked questions about workshops,
            refer to <a href="https://carpentries.org/workshops/workshops-faq">the Carpentries Workshop FAQ</a>.
            </p>    
        </dd>
    </div>

    <!-- <div class="row">
        <dt class="col-sm-2 col-md-2 py-2 px-3 bg-body-light text-body-secondary fw-bold">Accessibility</dt>
        <dd class="col py-2 px-3 mx-0 mb-0">
        
        </dd>
    </div> -->

    </dl>
  </div>
</div>


<div class="card mb-2">
  <h5 class="card-header">Who Can Attend</h5>
  <div class="card-body">
    <p id="who-can-attend">
      This training is closed to two confirmed UC OSPO Network lesson development cohorts:
      <strong>Librarians as Open Source Stewards</strong> (UC Berkeley Library Data Services) and
      <strong>Software Licensing</strong>. It is not open for public registration. Both cohorts get
      the same content, so Stewards has the option to join Licensing's locked session (Thu 8/27 PM +
      Fri 8/28) instead of a separate one, if that timing works for enough of the team. If you're
      interested in a future UC OSPO CLDT cohort, contact
      <a href="mailto:tdennis@library.ucla.edu">tdennis@library.ucla.edu</a>.
    </p>
  </div>
</div>

<div class="card mb-2">
  <h5 class="card-header">Participants</h5>
  <div class="card-body">
    <div class="row">
      <div class="col-md-6">
        <h6>Cohort 1: Librarians as Open Source Stewards</h6>
        <p class="text-muted mb-1">
          Lead contact: Anna Sackmann &middot;
          <a href="https://github.com/UC-OSPO-Network/education/issues/121">lesson concept (issue #121)</a>
        </p>
        <ul>
          <li>Anna Sackmann (UC Berkeley) — Data Services Librarian, lead contact</li>
          <li>Sam Teplitzky (UC Berkeley) — Open Science Librarian</li>
          <li>Jake Gibson (UC Berkeley) — Data Curator</li>
          <li>Rachel Torres (UC Berkeley) — Data Instruction and Outreach Librarian</li>
        </ul>
        <p class="text-muted mb-0"><em>Schedule: TBD. May join Licensing's Thu 8/27 PM + Fri 8/28 session, or a separate week — a fresh availability poll is going out (one team member works EST Tue-Thu).</em></p>
      </div>
      <div class="col-md-6">
        <h6>Cohort 2: Software Licensing</h6>
        <p class="text-muted mb-1">
          Lead contact: Karla Padilla &middot;
          <a href="https://github.com/UC-OSPO-Network/education/issues/83">lesson concept (issue #83)</a>
        </p>
        <ul>
          <li>Karla Padilla (UC San Diego) — lead</li>
          <li>Reid Otsuji (UC San Diego)</li>
          <li>Laura Langdon (UC OSPO)</li>
          <li>Jose Niño Muriel (UC Santa Barbara)</li>
        </ul>
        <p class="text-muted mb-0"><em>Schedule: locked — Thu 8/27 afternoon + Fri 8/28 (full day).</em></p>
      </div>
    </div>
  </div>
</div>


{% comment %}
COLLABORATIVE NOTES

If you want to use an Etherpad, go to

https://pad.carpentries.org/YYYY-MM-DD-site

where 'YYYY-MM-DD-site' is the identifier for your workshop,
e.g., '2015-06-10-esu'.

Note we also have a CodiMD (the open-source version of HackMD) available at https://codimd.carpentries.org
{% endcomment %}
{% if page.collaborative_notes %}
<h2 id="collaborative_notes">Collaborative Notes</h2>
<p>
We will use this <a href="{{ page.collaborative_notes }}">collaborative document</a> for chatting, taking notes, and sharing URLs and bits of code.
</p>
{% endif %}


{% comment %}
SURVEYS - DO NOT EDIT SURVEY LINKS
{% endcomment %}
<div class="card mb-2">
  <h5 class="card-header">Surveys</h5>
  <div class="card-body">
    <div class="row">
    <div class="col-sm-6">
        <div class="card text-center">
            <div class="card-body">
                <h5 class="card-title">Pre-Workshop Survey</h5>
                <p class="card-text">Please fill out this survey <strong>before attending</strong> the workshop.</p>
                {% if site.carpentry == "incubator" %}
                <a href="{{ site.incubator_pre_survey }}">Pre-workshop Survey</a>
                {% elsif site.incubator_pre_survey %}
                <div class="alert alert-danger">
                WARNING: you have defined custom pre- and/or post-survey links for
                a workshop not configured for The Carpentries Incubator
                (the value of `curriculum` is not set to `incubator` in `_config.yml`).
                Please comment out the `incubator_pre_survey` and `incubator_post_survey` fields
                in `_config.yml` or, if this workshop is teaching a lesson in the Incubator,
                change the value of `carpentry` to `incubator`.
                </div>
                {% elsif site.carpentry == "hpcc" %}
                <a href="{{ site.hpcc_pre_survey }}{{ site.github.project_title }}" class="btn btn-primary">Fill Out the Pre-Workshop Survey</a>
                {% else %}
                <a href="{{ site.pre_survey }}{{ site.github.project_title }}" class="btn btn-primary">Fill Out the Pre-Workshop Survey</a>
                {% endif %}
            </div>
        </div>
    </div>
    <div class="col-sm-6">
        <div class="card text-center">
            <div class="card-body">
                <h5 class="card-title">Post-Workshop Survey</h5>
                <p class="card-text">Please fill out this survey <strong>before you leave</strong> the workshop.</p>
                {% if site.carpentry == "incubator" %}
                <a href="{{ site.incubator_post_survey }}">Post-workshop Survey</a>
                {% elsif site.incubator_post_survey %}
                <div class="alert alert-danger">
                WARNING: you have defined custom pre- and/or post-survey links for
                a workshop not configured for The Carpentries Incubator
                (the value of `curriculum` is not set to `incubator` in `_config.yml`).
                Please comment out the `incubator_pre_survey` and `incubator_post_survey` fields
                in `_config.yml` or, if this workshop is teaching a lesson in the Incubator,
                change the value of `carpentry` to `incubator`.
                </div>
                {% elsif site.carpentry == "hpcc" %}
                <a href="{{ site.hpcc_post_survey }}{{ site.github.project_title }}" class="btn btn-primary">Fill Out the Pre-Workshop Survey</a>
                {% else %}
                <a href="{{ site.post_survey }}{{ site.github.project_title }}" class="btn btn-primary">Fill Out the Post-Workshop Survey</a>
                {% endif %}
            </div>
        </div>
    </div>
    </div>
  </div>
</div>


{% comment %}
SCHEDULE

Show the workshop's schedule.

Small changes to the schedule can be made by modifying the
`schedule.html` found in the `_includes` folder for your
workshop type (`swc`, `lc`, or `dc`). Edit the items and
times in the table to match your plans. You may also want to
change 'Day 1' and 'Day 2' to be actual dates or days of the
week.

For larger changes, a blank template for a 4-day workshop
(useful for online teaching for instance) can be found in
`_includes/custom-schedule.html`. Add the times, and what
you will be teaching to this file. You may also want to add
rows to the table if you wish to break down the schedule
further. To use this custom schedule here, replace the block
of code below the Schedule `<h2>` header below with
`{% include custom-schedule.html %}`.
{% endcomment %}

<div class="card mb-2">
  <h5 class="card-header">Schedule</h5>
  <div class="card-body">
    <p class="text-muted"><em>Draft agenda below, adapted from the standard Carpentries CLDT structure.</em></p>
    <p class="text-muted">
      Sessions are recorded, so a missed session (or stepping out for an hour for another meeting) isn't a blocker —
      you can catch up on the recording and get a quick team catch-up from your cohort.
    </p>

    <h6 class="mt-3">Licensing cohort — locked</h6>
    <p class="text-muted">
      <strong>Thu 8/27 afternoon + Fri 8/28 (full day) = 12 hours</strong>, the whole training in one week.
      Confirmed with all four: Jose, Karla, Reid, and Laura (Laura may need to duck out around 2pm on
      Thursday for another meeting — covered by the recording). Exact start/end times to follow.
    </p>
    <p class="text-muted">
      Episode order below follows the official
      <a href="https://carpentries.github.io/lesson-development-training/">CLDT curriculum</a> (13 episodes,
      instructor notes linked). For a licensing lesson, "example data" matters less than the narrative/use-case
      thread does — we'll lean on the narrative half of episode 5 and de-emphasize dataset selection.
    </p>
    <div class="row">
      <div class="col-md-5">
        <h6>Day 1 — Thu 8/27, afternoon</h6>
        <table class="table table-striped">
          <tr><td><a href="https://carpentries.github.io/lesson-development-training/instructor/introduction.html">Introduction</a></td></tr>
          <tr><td><a href="https://carpentries.github.io/lesson-development-training/instructor/lesson-design.html">Lesson Design</a></td></tr>
          <tr><td><a href="https://carpentries.github.io/lesson-development-training/instructor/audience.html">Identifying Your Target Audience</a></td></tr>
          <tr><td>Break</td></tr>
          <tr><td><a href="https://carpentries.github.io/lesson-development-training/instructor/objectives.html">Defining Lesson Objectives</a></td></tr>
          <tr><td><a href="https://carpentries.github.io/lesson-development-training/instructor/narrative.html">Example Data and Narrative</a> — introduced, not finished</td></tr>
        </table>
        <p class="text-muted"><em>Overnight: each team sits with the narrative/use-case question and comes back Friday with a candidate thread for their lesson — not a finished answer, just something to react to.</em></p>
      </div>
      <div class="col-md-7">
        <h6>Day 2 — Fri 8/28, full day</h6>
        <table class="table table-striped">
          <tr><td>Share narrative threads from overnight, refine as a group</td></tr>
          <tr><td><a href="https://carpentries.github.io/lesson-development-training/instructor/episodes.html">Episodes</a></td></tr>
          <tr><td><a href="https://carpentries.github.io/lesson-development-training/instructor/formative-assessment.html">Designing Exercises</a></td></tr>
          <tr><td>Break</td></tr>
          <tr><td><a href="https://carpentries.github.io/lesson-development-training/instructor/explanation.html">How to Write a Lesson</a></td></tr>
          <tr><td><a href="https://carpentries.github.io/lesson-development-training/instructor/infrastructure.html">The Carpentries Workbench</a></td></tr>
          <tr><td><a href="https://carpentries.github.io/lesson-development-training/instructor/lesson-content.html">Adding Lesson Content</a> — drafting episode content in teams</td></tr>
          <tr><td>Lunch break</td></tr>
          <tr><td><a href="https://carpentries.github.io/lesson-development-training/instructor/operations.html">How We Operate</a></td></tr>
          <tr><td><a href="https://carpentries.github.io/lesson-development-training/instructor/preparing.html">Preparing to Teach</a> — pilot-teach planning &amp; timeline; next steps (repo setup, Zenodo DOI, checkout path)</td></tr>
          <tr><td><a href="https://carpentries.github.io/lesson-development-training/instructor/wrap-up.html">Wrap-up</a></td></tr>
        </table>
      </div>
    </div>

    <h6 class="mt-4">Stewards cohort — schedule TBD</h6>
    <p class="text-muted">
      Anna's group has the option to join the Licensing session above (Thu 8/27 PM + Fri 8/28) if that timing
      works for enough of the team. Otherwise, working assumption is a later date in September — a fresh
      availability poll is going out (complicated a bit by one team member working EST hours Tuesday through
      Thursday, though he's usually flexible). Same content and agenda either way; this section will fill in
      once a date is confirmed.
    </p>

    <p class="text-muted mb-0 mt-3">Asynchronous lesson-drafting work continues between sessions and after the training, with bi-weekly check-ins.</p>

    {% comment %}
    Edit/replace the text above if you want to include a schedule table.
    See the contents of the _includes/custom-schedule.html file for an example of how one of these schedule tables is constructed.
    {% endcomment %}

    {% if site.pilot %}
    The lesson taught in this workshop is being piloted and a precise schedule is yet to be established.
    The workshop will include regular breaks. Please <a href="mailto:{{page.email}}">contact the workshop organisers</a> if you would like more information about the planned schedule.
    {% endif %}
  </div>
</div>

<div class="card mb-2">
  <h5 class="card-header">After the Live Training</h5>
  <div class="card-body">
    <p>
      Live instruction is the start, not the finish. Support continues afterward — Tim will go over content with
      teams, help with the Carpentries Workbench lesson infrastructure and markdown/markup, and work alongside each
      team as they build out their lesson repo in the UC-OSPO-Network GitHub organization. This mirrors what worked
      well for the IMLS Open Science lesson cohorts: post-workshop coaching, not just a one-time training, is what
      gets a lesson from outline to a real draft ready to pilot.
    </p>
  </div>
</div>

<hr/>


{% comment %}
SETUP

Delete irrelevant sections from the setup instructions.  Each
section is inside a 'div' without any classes to make the beginning
and end easier to find.

This is the other place where people frequently make mistakes, so
please preview your site before committing, and make sure to run
'tools/check' as well.
{% endcomment %}

<h2 id="setup">Setup</h2>
<p>
  This is a Collaborative Lesson Development Training (CLDT), not a standard workshop —
  you'll be building a lesson, not just following one. You will need access to software
  as described below, plus an up-to-date web browser.
</p>
<p>
  We maintain a list of common issues that occur during installation as a reference for instructors that may be useful on the
  <a href="{{site.swc_github}}/workshop-template/wiki/Configuration-Problems-and-Solutions">Configuration Problems and Solutions wiki page</a>.
</p>


{% comment %}
For online workshops, the section below provides:
- installation instructions for the Zoom client
- recommendations for setting up Learners' workspace so they can follow along the instructions and the videoconferencing

If you do not use Zoom for your online workshop, edit the file `_includes/install_instructions/videoconferencing.html` to include the relevant installation instructions.
{% endcomment %}

{% if online != "false" %}
  {% include install_instructions/videoconferencing.html %}
{% endif %}


{% comment %}
These are the installation instructions for the tools used during the workshop.
{% endcomment %}

{% assign setup_file = site.carpentry | append: '/setup.html' %}
{% if isOfficial %}
  {% include {{ setup_file }} %}
{% elsif site.carpentry == "incubator" %}
  Please check the "Setup" page of <a href="{{site.incubator_lesson_site}}">the lesson homepage</a> for instructions to follow to obtain the software and data you will need to follow the lesson.
{% else %}
  <h3 id="prep">Preparing for the Training</h3>
  <p>
    This training is designed for a team working together to collaboratively design and develop a new lesson.
    It helps to meet beforehand as a team and talk through:
  </p>
  <ul>
    <li>Topic and scope — already drafted for us in <a href="https://github.com/UC-OSPO-Network/education/issues/83">issue #83</a>; worth a quick team read before Thursday</li>
    <li>Who the lesson is aimed at</li>
    <li>A candidate narrative or use case to hang the licensing content on — since this isn't a data-analysis lesson, we're leaning on the narrative half of the CLDT curriculum's <a href="https://carpentries.github.io/lesson-development-training/instructor/narrative.html">Example Data and Narrative</a> episode more than the dataset half</li>
  </ul>
  <p>
    If your schedule allows, set aside some time between Thursday and Friday to follow up together on what
    we started — not required, but past trainees said the extra time helped.
  </p>
  <p>
    You'll need a GitHub account (see below) — we'll be working in the UC-OSPO-Network org, not personal
    repos. Team setup in the org is in progress.
  </p>

  <h3 id="workbench">The Carpentries Workbench</h3>
  <p>
    Lessons in this training are built with
    <a href="https://carpentries.github.io/sandpaper-docs/">The Carpentries Workbench</a>
    (R packages: <code>sandpaper</code>, <code>varnish</code>, <code>pegboard</code>, <code>tinkr</code>).
    Install R and RStudio, then run:
  </p>
  <pre><code>install.packages(c("sandpaper", "varnish", "pegboard", "tinkr"),
    repos = c("https://carpentries.r-universe.dev/", getOption("repos")))</code></pre>

  <h3 id="github">GitHub</h3>
  <p>
    You'll need a <a href="https://github.com/join">GitHub account</a> and a basic working
    knowledge of Git — your team's lesson repo will live in the UC-OSPO-Network GitHub
    organization.
  </p>
{% endif %}
