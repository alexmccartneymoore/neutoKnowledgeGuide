## Neuto Carbon Monitor  uses complex software to scan and analyse every page on your website,creating an accurate report of the carbon emissions generated. We use real user data gathered from the Google Analytics API to construct a detailed breakdown of your emissions.

By [Alex McCartney](https://alexmccartney.com)

### Standards-ready
Neuto Carbon Monitor is standards-compliant and designed to work with established standards such as the [GHG Protocol Corporate Standard](https://ghgprotocol.org/standards/scope-3-standard), to enable organisations to model the environmental impact from digital services. These emissions models fall under ‘Scope 3’, or supply chain, emissions.

### What happens
When a website, along with its analytics data, is submitted to Neuto Carbon Monitor, a series of tests are performed. First, the website urls are checked for certain types of parameters. Then data is collected on each url by accessing the webpage through a browser and recording a HAR file (HTTP Archive format) with some additions of our own to ensure that the data is relevant  to carbon emissions. For example, we collect additional data on media assets, fonts and scripts that can help our users understand the granular impact of these elements on the emissions generated by a particular webpage.

After collecting data associated with the ‘frontend’ (user-facing) part of a website, we collect what data we can about the server – without using intrusive methods. We identify the server’s location and grid/renewable energy mix by comparing data from the Green Web Foundation and national energy databases. Without direct access to the systems behind server infrastructure it is difficult to find and shore up data relating to servers. (As we will explain below, collecting and using accurate data for this aspect of website systems architecture is one of our targets for this year. We are also developing a system for calculating cloud computing emissions.)

Next, we collate the data we have on the website’s users, their devices, location, time spent on the website/webpage, and the energy mix available to them. It is important to remember that all the data we use is anonymised and can not be used to identify individuals.

### The calculations
A full explanation of our calculations is perhaps more suited to an academic paper, so we will provide an overview here.

In essence, our inputs are the many (65+) data points that we collect about a webpage's real users, user devices, user interactions, data sent to those users, and what we know, or can estimate, about the server infrastructure behind the scenes. It is of the utmost importance to our calculations that we use real data as much as possible, scaling down our reliance on large estimates.
This is why we prefer to know the real numbers of users, the devices they are using and the energy mix available to them. For the majority of users we can identify the device they are using and therefore produce an accurate estimate of the energy consumed when visiting any particular webpage.

As an example, the CO2 emissions from a webpage visited by one person using a device powered by coal-generated energy could be the same as for a webpage visited by multiple users whose devices are using renewable power. The same is true when comparing one energy-intensive desktop computer to many low-power and high-efficiency smartphones.

We extract and analyse the data 'sent down the wire' from a server – whether a caching server like a CDN or a stand-alone 'bare-metal' machine – to create, not only an emissions profile, but also a diagnosis of the webpage components that contribute to the emissions profile.

Our outputs are the translation of all of this data into the metrics you can explore in Neuto Carbon Monitor. The main, and most important, of these is the metric pertaining to CO2e emissions. Once you have collated the core energy consumption data, calculating the grams of CO2e emitted is simple. The challenge with constructing this calculation is making sure that the core energy consumption data is as accurate as possible.

### Our approach
Neuto Carbon Monitor uses a granular, 'bottom-up', methodology. The ‘system boundary’ that we use to structure our methodology stretches from the website's users through to the server infrastructure. This includes the data centre, wide area network (WAN), file area network (FAN), radio access network (RAN), and end devices. We use estimates when necessaryt – particularly in the case of the data centre and server architecture – but only based on data from peer-reviewed studies.We will continue to refine these estimates as more information becomes available.

Our effort to include end user devices in our calculations is prompted by the significant energy use that end users represent when contrasted  to other sections of the ICT system. Several estimates suggest that end user devices consume much more energy than networks and data centres combined. [One study](https://www.itu.int/ITU-T/recommendations/rec.aspx?rec=14084&lang=en) attributed 60% of the electricity consumption of the ICT sector to end user devices (excluding TVs), with networks and data centres accounting for only 20% each. The huge impact of the users on a website’s carbon emissions is the current focus of our work on Neuto Carbon Monitor.

One example we often give is that the same webpage can generate starkly different emissions when users in different countries access it on different devices. The ratio between user device, location and interactions with a webpage and its carbon emissions is a direct one. Perhaps obviously, the webpage 'weight' is also a factor, as the data processed by the server and then transferred through networks to the user does have an effect. However, the data we're currently collecting is beginning to suggest that page 'weight' is only one of many factors that can heavily influence associated website emissions, with the user’s device being the most prominent.

While we are beginning to develop a broader understanding of the way websites generate carbon emissions, decreasing the page 'weight' or 'data sent down the wire' can still make a significant improvement to any website's carbon emissions. Improving, and therefore lowering, a webpage's 'weight' should therefore be one of the first considerations for lowering a website's carbon emissions.

### What we want to improve

Our access and approach to ‘backend’ and server infrastructure has been limited to date and we are keen to expand the data we collect and use in our calculations, while respecting privacy.
We are in the process of compiling a database of end user devices, along with their associated energy consumption. We intend to use this data to be able to refine our calculations, using the make, model and viewport-size of a user’s device to accurately identify each device that visits a webpage and provide accurate data on energy consumption, and therefore carbon emissions.


#### Sources 

- [Energy consumption of ICT](https://post.parliament.uk/research-briefings/post-pn-0677/)
- [Streaming kWGB intensity](https://www.iea.org/commentaries/the-carbon-footprint-of-streaming-video-fact-checking-the-headlines)
- [Netflix’s streaming data](https://help.netflix.com/en/node/87)
- [Mobile Devices energy consumption](https://www.sciencedirect.com/science/article/pii/S1877050916317756)
- [Website visits data](https://www.statista.com/statistics/568735/e-commerce-website-visit-duration/)
- Arman Sherhabi et al. 2018
- [Electricity generation by source](https://www.iea.org/reports/tracking-power-2020)
- [Wind turbine carbon footprint](https://yaleclimateconnections.org/2021/06/whats-the-carbon-footprint-of-a-wind-turbine/)
- [Mobile data kw per GB](https://www.mdpi.com/2071-1050/10/7/2494)
- [New perspectives on internet electricity use in 2030, Anders S.G. Andrae](https://pisrt.org/psr-press/journals/easl-vol-3-issue-2-2020/new-perspectives-on-internet-electricity-use-in-2030/)
- [Ember Data Explorer](https://ember-climate.org/data/data-explorer/)
- [Electricity Maps](https://app.electricitymaps.com/map)
- [IPCC: Technology-specific Cost and Performance Parameters](https://www.ipcc.ch/site/assets/uploads/2018/02/ipcc_wg3_ar5_annex-iii.pdf)
- [CO2.js](https://github.com/thegreenwebfoundation/co2.js/blob/2b0c877a8f444e4d2ae5d2364bfb45b7abfa3e7e/data/co2-intensities-ember-2021.csv)
- [Why do estimates for internet energy consumption vary so dramatically?](https://www.wholegraindigital.com/blog/website-energy-consumption/)
- [The overlooked environmental footprint of increasing Internet use](https://www.sciencedirect.com/science/article/abs/pii/S0921344920307072?via%3Dihub)
- [Electricity Intensity of Internet Data Transmission: Untangling the Estimates](https://onlinelibrary.wiley.com/doi/full/10.1111/jiec.12630)
- [Carbon Impact of Video Streaming](https://ctprodstorageaccountp.blob.core.windows.net/prod-drupal-files/documents/resource/public/Carbon-impact-of-video-streaming.pdf)
- [Digital technology and the planet (The Royal Society)](https://royalsociety.org/-/media/policy/projects/digital-technology-and-the-planet/digital-technology-and-the-planet-report.pdf)
- [How to evaluate server manufacturing footprint, beyond greenhouse gas emissions?](https://www.boavizta.org/en/blog/empreinte-de-la-fabrication-d-un-serveur)
- [Building energy consumption models based on smartphone user’s usage patterns](https://www.sciencedirect.com/science/article/abs/pii/S0950705120308091)

