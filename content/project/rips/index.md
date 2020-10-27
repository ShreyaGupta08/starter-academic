---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Risk Assessment and Measurement of Privacy Leak in Google's Ads Data Hub"
summary: "My work done as a part of RIPS internship - in Institute of Pure and Applied Mathematics, UCLA and with Google, LA - on measuring privacy leaks to protect the end-user safety while making online search databases useful for advertisers"
authors: 
- admin
tags:
- privacy protection
- IPAM 
- UCLA
- Google
categories: []
date: 2019-09-20T00:00:00Z 
# 2020-10-27T16:46:12+05:30

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: "Mid-term presentation"
  focal_point: ""
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_code: ""
url_pdf: ""
url_slides: ""
url_video: "https://youtu.be/-AxHgeYTnB0"

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---


In the summers of 2019, I had the opportunity to work with a team of three talented researchers, with support of an academic advisor (Dr. Bao Wang) and with two industrial advisors (Vardhan Akopian and Scott Schneider), under the RIPS scholarship program conducted by Institute of Pure and Applied Mathematics, UCLA.  

## Introduction: RIPS Internship

RIPS stands for Research in Industrial Projects for Students. It is an annual research program organised by the Institute of Pure and Applied Mathematics (IPAM) of UCLA. With an acceptance rate of 3%, it hosts every year 36 interns who work on 9 industrial projects in groups of 4. I was one of the interns selected for the year 2019. Application Procedure and pre-intern experience is available [here](https://shreyagupta08.github.io/rips-internship-application-2019/) and Personal Experience is covered [here](https://shreyagupta08.github.io/rips-internship-people/).

## THE INTERNSHIP

RIPS is a crossover between research and industrial experience. We are given an industrial problem and have to solve it using quantitative and qualitative research. Each year witnesses industrial companies bringing their problems. I had a chance to work, with my fellow teammates, for Google, LA. 


## Problem Description

Google has an Ads Data Hub (ADH) for advertisers (customers) to analyze their ad campaigns (system diagram in figure 1). 
The advertisers can not see the raw data, for it can violate users' privacy. Hence advertisers can query the database to generate useful analytics. ADH has its own privacy filters so that advertisers only obtain aggregate results. Despite those filters, leaks can still occur. Our goal was to develop a framework that can measure the risk of privacy leaks in Google's ADH.

<figure>
	<a href="adh_system_rips.png"><img src="adh_system_rips.png"></a>
	<figcaption>Figure 1: High level overview of working of ADH</figcaption>
</figure>

## Conclusion

We provided Google, LA with the necessary deliverables, designing a framework that gives a risk assessment score descriptive of how at risk each user is and how each attribute contributes to the risk. We call it the PIRATE Score (Probabilistic Identification Risk and Attacker Threat Estimate score). Paper for the same will soon be available.

## Tangibles

We presented our work to RIPS Colloquium. Our research was selected to represent RIPS at the annual CUR Sympoisum, held at Alexandria, Virginia, where we were selected to present a poster. The work received recognition and appreciation for its logical improvisation and technical extention of the previous state-of-the-art methodology [1]. Additionally, the work received Outstanding Poster Award at Joint Mathematics Meet 2020, held at Denver and Best Poster Award at [ACSS](http://lcs2.iiitd.edu.in/acss2020/) held at IIIT-Delhi. The project's report is available on request. 


### Slides, Presentation recording and project report available on request

Feel free to email at shreyag [at] iiitd [dot] ac [dot] in - if you are interested in discussing the work, perusing the report or both.


References: 

[1] Streit, M., Dammers, J., Simsek-Kraues, S., Brinkmeyer, J., Wolwer, W., Ioannides, A.: Time course of regional brain activations during facial emotion recognition in humans. Neurosci. Lett. 342(12), 101–104 (2003)