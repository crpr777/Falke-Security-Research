---
layout: post
title: "Breaching the Perimeter: Full Scope Red Team Adventures, From Infiltration to Exfiltration (Part 1)"
date: 2026-10-14 12:00:00 +0000
categories:
  - Red Team Operations
tags:
  - covert-entry
  - red-team
  - physical-security
  - reconnaissance
summary: "Part 1 of a full-scope red team walkthrough: how I approach reconnaissance and plan physical entry into a target facility, from remote OSINT to urban camouflage."
---

In this post I will cover the methods I have used in live environments that have allowed me to break into organizations both physically and digitally. I have been a Red Team operator for about 13 years and have been exposed to various types of facilities, often tasked with breaking into warehouses, skyscrapers, corporate offices of various sizes, banks, and other secure facilities. Much of this work has been enabled by a team of operators, mentors who guided me and helped me watch for cameras and gave feedback, and organizations kind enough to give me the opportunity to break into their environments.

> All of the work described here was performed under explicit legal authorization as part of sanctioned red team engagements.

Engagements often begin with just an organization name, a target facility, and the proper legal authorizations. We will begin this journey with how I approach reconnaissance for a given organization and facility. For this example we can use Harbour Centre in Vancouver.

![Harbour Centre, Vancouver]({{ '/assets/img/breaching-the-perimeter-part-1/01-harbour-centre.png' | relative_url }})

Now that we have a target facility, we can use public sources such as Google Maps, YouTube, realty sites, and other sources to identify easy entry points, information on security measures, and the organizations within this facility so that we can build backstories to use if questioned.

Google Maps street view is a great source for remote physical reconnaissance on targets prior to on-site reconnaissance and surveillance. Using Google Maps we can rapidly identify entry points used by everyday visitors and entrances that would be of interest to me as an attacker, specifically emergency exit stairwells.

![Emergency exit stairwell spotted in street view]({{ '/assets/img/breaching-the-perimeter-part-1/02-emergency-exit.png' | relative_url }})

![Entry point detail]({{ '/assets/img/breaching-the-perimeter-part-1/03-entry-detail.png' | relative_url }})

![Entry point detail]({{ '/assets/img/breaching-the-perimeter-part-1/04-entry-detail2.png' | relative_url }})

While these doors are commonly locked, I would target them with latch bypass techniques such as mica/plastic shims, or one of my favorite tools, the Seattle Rapid Access Tool (SEARAT). Once on site we would test each of these doors to see if any are left unlocked, what the surveillance and alarms look like, or whether there are easier entrances to compromise.

Using realty sites we can also gather information such as how many floors the building has, the types of elevators used, information on security measures, and further validate the locations of stairwells and entrances.

![Realty listing detail]({{ '/assets/img/breaching-the-perimeter-part-1/05-realty.png' | relative_url }})

![Realty listing detail]({{ '/assets/img/breaching-the-perimeter-part-1/06-realty2.png' | relative_url }})

We can also use this information to help inform our backstory. Perhaps we are just a lost student or teacher at Simon Fraser University, or an employee of one of the other major tenants.

![Building tenants]({{ '/assets/img/breaching-the-perimeter-part-1/07-tenants.png' | relative_url }})

Now that we have an idea of what some of the entrances look like and the organizations at this facility, we can select our urban camouflage; in other words, a proper disguise to blend into our environment. Posing as a teacher, I could wear an SFU hoodie, which gives me a reason to carry a book bag where I would stash all my covert entry tools. We can also bring some generic outfit changes, such as a hat to help cover our face from security cameras and a generic safety vest to change our entire look and masquerade as a contractor doing work on the facility.

![Urban camouflage option]({{ '/assets/img/breaching-the-perimeter-part-1/08-camo1.png' | relative_url }})

![Urban camouflage option]({{ '/assets/img/breaching-the-perimeter-part-1/09-camo2.png' | relative_url }})

![Urban camouflage option]({{ '/assets/img/breaching-the-perimeter-part-1/10-camo3.png' | relative_url }})

Now that we have an idea of our target and how we would blend into the environment, we can get started on all our paths for entry, physical, digital, or a combination of both, beginning with low-tech and proximity methods and gradually escalating into more technical methods.

*Part 2, covering the tools of the trade and the entry techniques themselves, is coming soon.*
