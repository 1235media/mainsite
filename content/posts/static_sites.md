+++
date = '2025-01-11'
title = 'Static Websites Are Great (and Cheap)'
author = 'Jon Wear'
tags = ["netlify","static sites"]
+++

A statically generated website is one where all the files are created ahead of time and uploaded to a server. How does this work? A program processes all the content files (like this article), combines them with a set of template files (usually pre-made for you), and generates HTML, CSS, and JavaScript. These files are then uploaded to the server. If your domain name is configured correctly, that collection of files will display a website (like this one). Why is this cool?

1. There's no web server to configure and maintain that has to handle lots of server side rendering. Everything is already rendered
1. There's no database to configure and maintain
1. There's no load balancer to configure or maintain
1. There's nothing to hack
1. In most instances there's no bandwidth to monitor
1. Depending on the provider, there's no SSL certificate to manage (or pay for)

Keep in mind when you see words like "configure", "maintain" and _especially_ "hack", that means spending money.  Can a static site do everything?  Of course not, but you can do a surprising amount with them.  Services like Netlify (which I use but am in no way affiliated with) will let you host a static site and you get up to 500gb of bandwidth free each month.  If you have a site that's around 5mb in size, you can get about 100,00 views per month and never go over their free tier.  Register a domain name, point it at the Netlify location where your static site is and there you go.  

You can embedded user forms in your site using a provider like Netlify (again with their generous free tier) and have potential customers sign up for a newsletter or ask questions.  Netlify manages the spam detection and storage.  You can also make changes to your template, add new articles and have preview links so you and others can review things before making them public.

And should Netlify or some other hosting provider go out of business or stop providing a great service, your content is all normal web pages (HTML, CSS, and JavaScript).  You can easily move your site elsewhere, point the domain name to the new location and there you go.

The cost with a site like this is all up front.  The domain name isn't free and you will probably spend money on _some_ design work although there are LOTS of free templates available.  Why don't more companies use them?  My guess is that they aren't recommend by software consultants all that much because there isn't any money to be made.  But there is a lot of utility to be had here for very low cost.  If you'd like to know more, you can email me here: jon@1235media.com or submit a question at our [contact form](https://1235media.com/#contact).

If you're a bit technical and want to try some of this on your own, here is the exact technical stack we use for 1235Media.com

1. [https://gohugo.io](Hugo) is the software we use to generate our static site
    1. It is free and open source.
    1. You can find lots of cool templates [here](https://hugothemesfree.com)
1. [Github.com](https://github.com) to hold all of the template files and content
    1. You can create a free account
1. We registered the domain name with [squarespace.com](https://domains.squarespace.com)
1. [Netlify](https://netlify.com) hosts our content
    1. Whenever we push a new article to our main branch on github, netlify picks up the change and updates the site
