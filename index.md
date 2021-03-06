---
layout: col-sidebar
title: OWASP Waterloo
tags: waterloo
level: 0
region: North America
meetup-group: owasp-waterloo-meetup-group
country: Canada
postal-code: 

---

Welcome to the Waterloo chapter homepage.
-----------------

### Upcoming Meetings

We schedule our meetings on the [OWASP Waterloo Meetup Group](https://www.meetup.com/owasp-waterloo-meetup-group/)

{% include chapter_events.html group=page.meetup-group %}

Our meetings are open to the public, and you do not need to be a member to attend. Please do consider [joining OWASP](https://owasp.org/membership/) if you find our community, projects, and meetings valuable, or sponsoring this chapter.

Past Sessions
-----------------
<br>

| # | Date / Time |  Title | 
| -------- | -------- | ----------- | 
| 2021-01 | April 22, 2021 7:30 PM| A Journey Through the Kubernetes Threat Matrix - Part 1 | 
| 2021-02 | June 24, 2021 7:30 PM| A Journey Through the Kubernetes Threat Matrix - Part 2 | 


<br> 

**-----------**

**Meetup 2021-01**

Date / Time: April 22, 2021 @ 7:30 PM <br>
Location: TBD 

**Welcome to OWASP Waterloo** 

This is our first meetup of 2021! 
We are excited to meet everyone and since this is the first OWASP waterloo meetup of 2021, will begin with an introduction, followed by a presentation and discussion. 

**A Journey Through the Kubernetes Threat Matrix - Part 1**

**Summary:**

In this presentation we explore a Kubernetes Threat Matrix and the impact that a vulnerable application has on a poorly configured cluster. This talk draws from examples of teams that rush in to adopt Kubernetes without consideration for security guidance and best practices. In our example, a devops engineer deploys a vulnerable legacy application to an internet facing cluster and decides to use the Kubernetes CA for internal TLS certificates as an easy option since it is available and trusted in the cluster. As we journey through the Kubernetes threat matrix, we demonstrate how an attacker might take advantage of the vulnerable container and cluster misconfiguration for profit. The focus of this talk is to explore threats in Kubernetes and discuss security misconfigurations from the [OWASP top 10](https://owasp.org/www-project-top-ten/)

**Presenters:**
Scott Handfield,
Kris Jamieson,
Deepak Sharma


**-----------**

**Meetup 2021-02**

Date / Time: Jun 24, 2021 @ 7:30 PM <br>
Location: TBD 


**A Journey Through the Kubernetes Threat Matrix - Part 2**

**Summary:**

This presentation is a continuation from Part 1, where we switch focus to explore preventative and detective controls based on the Kubernetes Threat Matrix. We explore using OPA to create policies that prevent abuse of the Kubernetes CA, privileged pods, etc. As we journey through the Kubernetes threat matrix, we demonstrate how a defender might apply policy as code to identify and restrict vulnerable container and cluster misconfigurations. The focus of this talk is to explore best practices and guidance from the [OWASP Kubernetes Security Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/Kubernetes_Security_Cheat_Sheet.html)

**Presenters:**
Scott Handfield,
Kris Jamieson,
Deepak Sharma

<br> 

**-----------**

### Check our Upcoming Meetup Events:
{% include chapter_events.html group=page.meetup-group %}


<script type='text/javascript'>
  $(function(){
    $(".timeclass").hover(function() {
      utc_str = $(this).text();
      ndx = utc_str.indexOf(':');
      st_hour_str = utc_str.substring(0, ndx);
      st_min_str = utc_str.substring(ndx + 1, ndx + 3);
      utc_dt = luxon.DateTime.utc(2020, 06, 06, parseInt(st_hour_str), parseInt(st_min_str), 0);
      start_dt = utc_dt.setZone(luxon.DateTime.local().zoneName);

      ndx = utc_str.lastIndexOf(':');
      end_hour_str = utc_str.substring(ndx - 2, ndx - 1);
      end_min_str = utc_str.substring(ndx + 1, ndx + 3);
      utc_dt = luxon.DateTime.utc(2020, 06, 06, parseInt(end_hour_str), parseInt(end_min_str), 0);
      end_dt = utc_dt.setZone(luxon.DateTime.local().zoneName);
      popstr = start_dt.toLocaleString(luxon.DateTime.TIME_WITH_SECONDS) + ' to ' + end_dt.toLocaleString(luxon.DateTime.TIME_WITH_SHORT_OFFSET);
      $(this).prop('title', popstr);
    });
  });
