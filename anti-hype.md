---
layout: page
title: anti-hype
permalink: /anti-hype/
---
## Becoming an Anti-Hype Data Engineer

I have been working in data engineering for about eight years now. When I started, I caught the tail end of the Hadoop era. I got my start on a technology known then as MapR at a boutique energy firm in Houston, Texas. This was a period of personal growth and learning, from Python, Spark, Scala, Docker, Airflow, and how to check in code to GitLab. It was an exciting time. As a junior developer, you are more fascinated by what you can do with a language rather than what you can solve. This is the way.

As I progressed in my career, became somewhat wiser (debatable), more business-oriented (less debatable), and apathetic with the technology I was using, I realized that most companies overspend and under-deliver on their data projects. But why?

It seems like there are tons of companies who are buying into the marketing hype surrounding the two major data platform as a service offerings: Databricks and Snowflake. My cached take for the week: 80% of companies do not need what these companies are offering for the price they are paying. The global economy is headed for a recession. That's not my opinion, that's the Federal Reserve's. So in a time where most companies should be cutting back, how and where should you cut?

Both of these platforms are charging their customers for Ferraris when most companies would be happy with a Toyota Camry with some aftermarket parts. Don't get me wrong, both platforms are doing impressive things; Snowflake's Data Cloud is really coming to life with their partnership with NVIDIA, and Databricks is putting runs on the board with the Spark Human API. These are not reasons you should use their platforms. These are marketing gimmicks to garner the attention of the decision-makers to loosen the company's purse strings.

This is a fundamental mistake in the way businesses operate: Pay to make a problem disappear. We operate as if these platforms solve problems when fundamentally they do not and often exacerbate large inefficiencies that already exist within an organization.

If you want to make a big impact, be anti-hype.

Alright, so how do you become anti-hype, you ask? Trust in people. People solve problems; thus, we should encourage businesses to get to the core of their data problems first before they start to spend $$$. Here is a list of things you can do as a cost-conscious, anti-hype data person:

1. **Sit down with your customer and be their data advocate.**

This is probably the hardest thing to do because ultimately, your business wants "The Art of the Possible." What a way to pass any and all responsibility to the engineer while maintaining none of the responsibility of defining your product. It's a great reminder that despite all of the hype around data, people do not know what they want. This is a huge red flag in any project I commit to because it shows immaturity and a lack of understanding of how the customer wishes to translate data into business value.

The most important thing about being anti-hype is truly understanding customer desire and translating that into an appropriate and measured response. Questions I would ask to engage the customer are:

* How do you see yourself using the data?
* Are you going to passively look at the data daily, or are you going to require some functionality to send data to another vendor?
* What is the frequency of the data?
* What is the volume?

Any engineer can code. A great anti-hype engineer asks questions until they hear "I do not know." Once this is said, then you can draw on your experience and expertise to help design and architect a solution that meets their needs.

2. **Do the boring stuff: Make a data model.**

This art has been lost amidst the data hype train. Most people are focused on going as fast as possible without realizing the architectural hole they might be burying their careers under. Modern Data Stack is great at producing velocity, but if you are fast at doing things wrong, it might spell doom if your other systems rely on the Modern Data Stack to finish performing analysis on very wide and long tables.

Think about your architecture, and decide on a data architecture for your data warehouse (Kimball, Inmon, etc.) and a visualization layer (Snowflake schema, star schema, galaxy schema). If you are doing a data lake, define the columns you want to partition on and colocate columns that you would filter on. Define when you should compact files and when to Z-order. If data needs to move bidirectionally, decide on how data updates on load in both directions.

Talk with your stakeholders. Ask the question how they want to see the data, colocate the fields they want to see together, and push the data fields they don't want to see to other tables. If
