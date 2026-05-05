---
title: "My internship: integrating Gemini into Data Commons"
url: "https://blog.datacommons.org/2025/10/09/my-internship-integrating-gemini-into-data-commons/"
date: "Thu, 09 Oct 2025 19:27:31 +0000"
author: "Adriana Olmos"
feed_url: "https://blog.datacommons.org/feed/"
---
<p class="wp-block-paragraph"><em>Google&#8217;s internships </em><em>are an important part of our culture of building for everyone. </em><em>Internships are designed to be more than just a summer job; it&#8217;s an opportunity to tackle real-world challenges and make an impact. Interns work alongside full-time Googlers, contributing to the helpful products and services that people use every day. While they gain hands-on experience and grow their skills under the guidance of dedicated mentors, we benefit from their curiosity and new approaches to problem-solving. To learn more,</em><em> </em><a href="https://goo.gle/3UIYZOt"><em>visit our Google Careers site</em></a><em>, set up job alerts, and apply when applications open in the fall.</em></p>



<p class="wp-block-paragraph"><strong>Q. Meet our intern Javier Vazquez: Tell us about yourself!</strong></p>



<p class="wp-block-paragraph">I’m Javi, a grad student doing a Master’s in AI at the University of Texas at El Paso. I’m excited to share a glimpse into my summer internship and the impactful feature I had the privilege to work on. It&#8217;s been an incredible journey of learning, collaboration, and bringing ideas to life.</p>



<p class="wp-block-paragraph"><strong>Q. What opportunity were you solving for? What is the solution you helped implement?&nbsp;</strong></p>



<p class="wp-block-paragraph">A quote from my internship host truly resonated with me throughout the entire internship: <em>“It’s easy to just do a thing, but it is a lot harder to do the thing right.”&nbsp;</em></p>



<p class="wp-block-paragraph">This idea inspired me to deeply consider what makes a feature useful for Data Commons users. With guidance from the team, I developed a new feature that leverages the power of LLMs to suggest new <strong>follow up questions </strong>for deeper exploration of our data.&nbsp;</p>



<p class="wp-block-paragraph">The core of the project was to develop a new feature that integrates Gemini directly into Data Commons. To better serve data analysts, I leveraged Gemini&#8217;s AI generation capabilities &#8211; which are fantastic at producing engaging content &#8211; to upgrade our <a href="https://datacommons.org/tools/statvar">Explore pages</a> on our Data Commons platform. This feature uses context from the Explore pages to automatically generate new engaging content, thereby directly meeting data analysts&#8217; data exploration needs</p>



<figure class="wp-block-image size-full is-resized"><img alt="Keep exploring feature in Data Commons" class="wp-image-820" height="480" src="https://i0.wp.com/blog.datacommons.org/wp-content/uploads/2025/10/Javis-blog-micro.gif?resize=784%2C480&#038;ssl=1" style="width: 547px; height: auto;" width="784" /></figure>



<p class="wp-block-paragraph">As we thought about what model to use (Gemma, Gemini, Gemini 2.5 Pro vs. Flash) we had to think about tradeoffs of quality and speed. After extensive testing, we found the optimal configuration: Gemini 2.5 Flash was best for handling follow-up questions, it achieves the right balance of performance. I’m very proud of the fact that the follow up questions feature is now fully rolled out, and you can give it a try!</p>
