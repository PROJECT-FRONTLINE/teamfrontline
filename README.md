# teamfrontline
First Hand Information for First Responders who are always on the Frontline with the help of Chatbot and an Interactive Dashboard powered by IBM Watson.This Project is part of IBM Call for Code 2020 COVID-19 Challenge.

## Authors

- Savio Lobo
- Lavin Peeyus

## Contents

1. [Overview](#overview)
2. [The idea](#the-idea)
3. [How it works](#how-it-works)
4. [Diagrams](#diagrams)
5. [Documents](#documents)
6. [Technology](#technology)
7. [Getting started](#getting-started)
8. [Resources](#resources)


## Overview

### What's the problem?

Our World is hit with a COVID-19 Pandemic Crisis. In this tines, the First Responders are the First ones to respond.The only way to solve this crisis is by helping our Firsst Responderd who are always on present on the Frontlines.We believe that "First Responders need First Response". First Response in terms of what they need and an immediate and timely answers to their Questions which they face while Serving us on the Frontline. 

### How can technology help?

We believe Technology especially build with the capabilities of IBM Watson can bridge the problem between the First Responders and the First Response they need by the Government Authorities.

## The idea

The goal is to build a Responsive Web Application like a website which can be accessed both by the Computer and a Smartphone. This Website will have a Chatbot powered by IBM Watson Assistant specially Designed for First Responders. It will as hold a form which will serve as a Data Collection tool to collect Information from the First Responder regarding their needs and the problems they face or encounter on the Frontlines.This data will in turn be fed into IBM Watson Studio to provid Insights in terms of Data Visualisation in An Interactive Dashboard. This Dashboard can be viewed by Government Authorities to assess Whar are the needs and the problems of the First Responders?

## How it works

A.First Responder(The First Responder will access the Website which have the chatbot and the form. The First Responders can access the Chatbot secially designed for First Responders and ask specific Questions like "How to clean a transport Vehicle?","What is the recommened PPE?" and get answers.The First Responders can aslo fill the form to specify their needs like which ppe they need? or the problems they face?)
B.Government Authorities(The Government Authorities can visitt this website and view the Interactive Dashboard powered by IBM Watson Studio having Data Visualisation based on the Data filled up in the form by the First Responders.)

## Diagrams

![Cooperation architecture diagram](/images/architecture-diagram.png)

This Architecture comprises of Chatbot powered by IBM Watson Assistant to be used by First Responders and an Interactive Dashboard powered by Watson Studio to be used by Government Authorities.  

For First Responder
1. The First Responder launches the Website.
2. He/She then launches the chatbot integrated with slack called as Frontline Chatbot specially designed for First Responders powered by IBM Watson.
3. He/She asks the Questions that he faces on the Frontline like "What precaustions are needed if I work in a Nursing facility?", "I am Pregnant, What care must I take while attending COVID-19 patients?".
4. The Chatbot then harnesses the capabilities of IBM Watson and answers the First Responders Query.
5. The First Responder can also fil a form in order to specify the needs and problems that they face on the frontlines like "hygiene", "whether their basic needs are satisfied?".
6. The Data collected by the form is fed into watson studio in order to be analysed by Government Authorities.

For Government Authorities:
1. The Government Authority launches the website.
2. He/She then lauches the Interactive Dashboard called as Frontline Insights powered by IBM Watson Studio to show the data filled in the for by the First Responders in terms of Data Visualisation.
3. The data can also be analysed in Watson Studio and decision can be made by the authorities and the needs of the first responders can be addressed.

## Documents

Trusted sources for COVID-19 Information:
- [CDC COVID-19 FAQ](https://www.cdc.gov/coronavirus/2019-ncov/faq.html)
- [WHO COVID-19 page](https://www.who.int/health-topics/coronavirus)


## Technology

### IBM Cloud Services

- [IBM Watson Assistant](https://www.ibm.com/cloud/watson-assistant/)
- [How-to guides for chatbots](https://www.ibm.com/watson/how-to-build-a-chatbot)
- [Learning path: Getting started with Watson Assistant](https://developer.ibm.com/series/learning-path-watson-assistant/)
- [Chat Bot Slack Integration](https://developer.ibm.com/technologies/artificial-intelligence/videos/integrating-watson-assistant-with-slack-using-built-in-integrations/#)
- [Chat Bot Slack deployment](https://cloud.ibm.com/docs/assistant?topic=assistant-deploy-slack)
-[IBM Watson Studio](https://cloud.ibm.com/catalog/services/watson-studio)


## Getting started

### Prerequisites

- Register for an [IBM Cloud](https://www.ibm.com/account/reg/us-en/signup?formid=urx-42793&eventid=cfc-2020?cm_mmc=OSocial_Blog-_-Audience+Developer_Developer+Conversation-_-WW_WW-_-cfc-2020-ghub-starterkit-cooperation_ov75914&cm_mmca1=000039JL&cm_mmca2=10008917) account.
- Install and configure [IBM Cloud CLI](https://cloud.ibm.com/docs/cli?topic=cloud-cli-getting-started#overview).
- Register for a [HERE](https://developer.here.com/ref/IBM_starterkit_Disasters2020?create=Freemium-Basic) account.
- Install [React Native CLI dependencies](https://reactnative.dev/docs/getting-started.html) (for iOS).
    - [Node.js](https://nodejs.org/en/)
    - [Watchman](https://facebook.github.io/watchman/docs/install.html)
    - [Xcode](https://itunes.apple.com/us/app/xcode/id497799835?mt=12)
    - [CocoaPods](https://guides.cocoapods.org/using/getting-started.html)
- Clone the [repository](https://github.com/Call-for-Code/Solution-Starter-Kit-Cooperation-2020).

### Steps

1. [Set up an instance of Watson Assistant](#1-set-up-an-instance-of-watson-assistant).
1. [Integrate your Watson Assistant with Slack](#2-Integrate your Watson Assistant with Slack).
1. [How to Create an Interactive Dashboard](#3-How to Create an Interactive Dashboard).
1. [How to Embed the Interactive Dashboard in a Website](#4-How to Embed the Interactive Dashboard in a Website).
1. [Run the mobile application](#5-run-the-mobile-application).

### 1. Set up an instance of Watson Assistant

Log in to IBM Cloud and provision a Watson Assistant instance.

1.Provision an instance of **Watson Assistant** from the [IBM Cloud catalog](https://cloud.ibm.com/catalog/services/watson-assistant).
2.Launch the Watson Assistant service.
3.[Create an **Assistant**](https://cloud.ibm.com/docs/assistant?topic=assistant-assistant-add).
4.Add a dialog skill to the **Assistant** by importing the  file.
5.Go back to All Assistants page, open **Settings** from the action menu ( **`⋮`** ) and click on **API Details**.
6.Note the **Assistant ID**, **API Key**, and **Assistant URL**. For **Assistant URL**, make note of the base URL/domain (e.g., `https://api.us-south.assistant.watson.cloud.ibm.com` or `https://api.eu-gb.assistant.watson.cloud.ibm.com`) and not the full directory/path. You will need all three of these values in Step 4 below.
7.Go to **Preview Link** to get a link to test and verify the dialog skill.

### 2.Integrate your Watson Assistant with Slack

1.Once you have got your Watson Assistant up and running follow this tutorial https://developer.ibm.com/tutorials/create-crisis-communication-chatbot-integrate-slack/

### 3.How to Create an Interactive Dashboard

1.Follow this tutorial to create an Interactive Dashboard powered by IBM Watson Studio https://developer.ibm.com/tutorials/create-interactive-dashboards-on-watson-studio/

### 4.How to Embed the Interactive Dashboard in a Website

1.Once your dashborad is ready Follow this tutorial to embed your Dashboard into a Website https://www.ibm.com/support/pages/how-do-you-embed-dashboard-watson-studio-service-your-web-site
 
Running the Project Frontline Website

1.Run the file 




![Intro Screen](/images/0-screen-home.png)
![Donate Screen](/images/1-screen-donate.png)
![Search Screen](/images/2-screen-search.png)
![Chat Screen](/images/5-screen-chat.png)
![Map1 Screen](/images/3-screen-map.png)
![Map2 Screen](/images/4-screen-map.png)

## Resources

- [IBM Cloud](https://www.ibm.com/cloud)
- [Watson Assistant](https://cloud.ibm.com/docs/assistant?topic=assistant-getting-started)
- [Watson Studio](https://cloud.ibm.com/catalog/services/watson-studio)


