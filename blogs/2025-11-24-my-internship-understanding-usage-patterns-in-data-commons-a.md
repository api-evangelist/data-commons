---
title: "My internship: Understanding Usage Patterns in Data Commons’ API"
url: "https://blog.datacommons.org/2025/11/24/my-internship-understanding-usage-patterns-in-data-commons-api/"
date: "Mon, 24 Nov 2025 14:18:20 +0000"
author: "Luiza"
feed_url: "https://blog.datacommons.org/feed/"
---
<p class="wp-block-paragraph"></p>



<p class="wp-block-paragraph"><em>Google&#8217;s internships </em><em>are an important part of our culture of building for everyone. </em><em>Internships are designed to be more than just a summer job; it&#8217;s an opportunity to tackle real-world challenges and make an impact. Interns work alongside full-time Googlers, contributing to the helpful products and services that people use every day. While they gain hands-on experience and grow their skills under the guidance of dedicated mentors, we benefit from their curiosity and new approaches to problem-solving. To learn more,</em><em> </em><a href="https://goo.gle/3UIYZOt"><em>visit our Google Careers site</em></a><em>, set up job alerts, and apply when applications open.</em></p>



<p class="wp-block-paragraph"><strong>Q. Meet our intern Lucy King. Tell us about yourself!</strong></p>



<p class="wp-block-paragraph">I’m a fourth-year undergraduate student at Columbia University studying computer science. I’m particularly interested in public interest technology, an emerging, interdisciplinary field focused on the responsible design, deployment, and governance of technology to advance the public good and solve societal problems. Working with the Data Commons team has been a wonderful opportunity to explore the field. This internship has been full of technical and nontechnical learnings and I’m excited to share my results!</p>



<p class="wp-block-paragraph"><strong>Q. Share highlights of your internship project. What opportunity were you solving for?</strong></p>



<p class="wp-block-paragraph">Data Commons has an impressive range of coverage across 193 countries and 250K+ statistical variables, however, achieving true global coverage requires persistently addressing existing data gaps.. My project focused on identifying these gaps by exploring patterns in current data utilization. A better understanding of these trends will help us partner and build capacity with <a href="https://blog.google/intl/en-africa/company-news/outreach-and-initiatives/google-helps-africa-build-an-ai-data-future-with-225m-in-support/">National Statistical Offices</a> to fill in gaps and help us reach our goal of serving as a one-stop destination for public data.</p>



<p class="wp-block-paragraph">These usage patterns are especially important to understand as we expand our product offerings – in addition to the Data Commons website and our API tools, we recently released a <a href="https://blog.datacommons.org/2025/10/02/announcing-the-data-commons-model-context-protocol-server/">Data Commons MCP server</a>. Discovering what new insights users are unlocking from this generative AI platform helps us understand how tools like this are enabling our users and informs our future approach to how Data Commons data can help ground Google’s generative AI initiatives.</p>



<p class="wp-block-paragraph"><strong>Q. What is the solution you helped implement?&nbsp;</strong></p>



<p class="wp-block-paragraph">First, let me share a diagram of Data Commons’ serving architecture.</p>



<figure class="wp-block-image size-large is-resized"><img alt="" class="wp-image-884" height="520" src="https://i0.wp.com/blog.datacommons.org/wp-content/uploads/2025/11/image-4.png?resize=1024%2C520&#038;ssl=1" style="width: 851px; height: auto;" width="1024" /></figure>



<p class="wp-block-paragraph">All of our products call back to our Mixer API, where we handle fetching query results from our foundational data stores in Bigtable. I built a structured logger in this API that reports the datasets used to populate results to GCP’s Cloud Logging platform. We wanted to be thoughtful about user privacy with Data Commons, so we don’t include any information about the user making the call – we only log stats about datasets and variables already in the Data Commons knowledge graph. These logs are stored in BigQuery, and from there our team can analyze usage patterns.</p>



<p class="wp-block-paragraph">To populate my logs with additional information about the places that users request, I modified our internal data ingestion pipeline that consolidates massive data stores from each of our partners. Working across Data Commons’ many products, I also collaborated with the Data Commons team to add metadata that indicates which product each call to the Mixer API originated from, helping us to improve our understanding of usage patterns unique to each DC product.</p>



<figure class="wp-block-image size-large is-resized"><img alt="Bar graph displaying the most popular statistical variables in the Data Commons, highlighting 'Count_Person' with the highest number of references." class="wp-image-879" height="675" src="https://i0.wp.com/blog.datacommons.org/wp-content/uploads/2025/11/image-3.png?resize=1024%2C675&#038;ssl=1" style="width: 759px; height: auto;" width="1024" /></figure>



<p class="has-text-align-center wp-block-paragraph"><em>Caption: Unsurprisingly, population data like Count_Person is most popular. DifferenceRelativeToBaseDate2006_Max_Temperature_RCP45 and similar variables come from our weather and climate-related data, which is also popular and featured on place pages.</em></p>



<p class="wp-block-paragraph">To visualize the analysis that can be done with my logs, I created a dashboard that our team can use to identify what data is particularly popular, what data is frequently requested that we don’t yet include, and in which geographies we may have coverage gaps. This tool is a key improvement in understanding Data Commons usage and can inform a better experience for our users as we work to fill these gaps.</p>



<p class="wp-block-paragraph"><strong>Q. What are some of the key learnings you are taking away from this internship, whether project or experience-related?&nbsp;</strong></p>



<p class="wp-block-paragraph">Working across so many of Data Commons’ products gave me a crash-course in languages, frameworks, and development environments that were totally new to me, from understanding Google Cloud’s data processing frameworks to exploring open source development processes when releasing new versions of our Python client library on PyPi.</p>



<p class="wp-block-paragraph">This team also stands at a fascinating intersection between the public and private sector. While interning at the U.S. Census Bureau last summer, I worked on a project to make international trade data more accessible to the public. This gave me insight into how data was created and helped me understand the importance of correct, secure information from the perspective of a public agency. Now, my work with Data Commons has made me part of the dissemination of this data – my focus has shifted from creating data to maximizing the number of people who have access to that information, and has grown from a national to a global scale. Moving between these two worlds has given me an appreciation for both efforts, which is invaluable as I continue to pursue a career at the intersection of technology and the public sector.</p>
