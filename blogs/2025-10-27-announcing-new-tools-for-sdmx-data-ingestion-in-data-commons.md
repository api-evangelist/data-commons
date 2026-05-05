---
title: "Announcing New Tools for SDMX Data Ingestion in Data Commons"
url: "https://blog.datacommons.org/2025/10/27/announcing-new-tools-for-sdmx-data-ingestion-in-data-commons/"
date: "Mon, 27 Oct 2025 08:10:25 +0000"
author: "Rohit Kumar"
feed_url: "https://blog.datacommons.org/feed/"
---
<p class="wp-block-paragraph">We are excited to announce a new set of open-source tools that simplify the initial steps of importing data in the Statistical Data and Metadata eXchange (SDMX) format into Data Commons. These tools address the critical first stage of the data ingestion pipeline, making it easier for our growing community to work with SDMX data and contribute to Data Commons.</p>



<h3 class="wp-block-heading">What is SDMX?</h3>



<p class="wp-block-paragraph">SDMX is a global standard for exchanging statistical data and metadata among organizations &#8211; it provides a common language and standardized data structure for critical indicators such as unemployment rates, GDP, and population figures, ensuring global interoperability among statistical bodies. SDMX is widely used by national statistical offices, central banks, and international organizations like the OECD, the World Bank, and the United Nations.</p>



<p class="wp-block-paragraph">Starting today, our Data Commons tools support <strong>SDMX 2.1</strong>, the most widely adopted version of the standard.</p>



<h3 class="wp-block-heading">Key features</h3>



<p class="wp-block-paragraph">Our new SDMX import tools, which can be used by both contributors to base Data Commons and owners of Custom Data Commons instances, offer several capabilities designed to streamline the first stage of data integration:</p>



<ul class="wp-block-list">
<li><strong>Dual usage modes:</strong> The tools function both as a command-line download tool and as a Python library (<code>SdmxClient</code>) for programmatic integration into data pipelines.&nbsp;</li>



<li><strong>Automatic format conversion</strong>: The tools automatically download from an SDMX feed to local storage and convert the data to a standardized CSV format, regardless of whether the source provides data in XML, JSON, or other formats. This simplifies downstream processing by providing a clean, tabular starting point. It&#8217;s important to note that after this conversion, the process of mapping the data concepts and columns to the Data Commons schema remains a manual step, similar to other CSV ingestions.</li>



<li><strong>Rich metadata mapping</strong>: SDMX&#8217;s rich metadata provides the necessary context to facilitate the manual mapping of concepts to Data Commons. For data providers, enriching your metadata with clear definitions is the most effective way to make your data more discoverable and easier to integrate in the future.</li>



<li><strong>Simplified auto-refresh setup</strong>: Datasets can be configured for automatic periodic updates without writing custom download scripts for each dataset, making it easy to keep data current as sources update.</li>
</ul>



<p class="wp-block-paragraph">All tools are available in our <a href="https://github.com/datacommonsorg/data/tree/master/tools/sdmx_import">GitHub repository</a>, with detailed usage instructions in the <a href="https://github.com/datacommonsorg/data/tree/master/tools/sdmx_import/README.md">README</a>.</p>



<h3 class="wp-block-heading">How to get started and contribute</h3>



<p class="wp-block-paragraph">We envision three primary ways for the community to engage with these new tools:</p>



<figure class="wp-block-table"><table class="has-fixed-layout"><tbody><tr><td><strong>User group</strong></td><td><strong>How you can help</strong></td></tr><tr><td><strong>Custom Data Commons owners</strong></td><td>Leverage our Python client to download and standardize SDMX data for your own custom ETL processes and private Data Commons instances.</td></tr><tr><td><strong>Open source contributors</strong></td><td>The tools are open source. Help us improve them by adding features, fixing bugs, and enhancing their robustness.</td></tr><tr><td><strong>SDMX data providers</strong></td><td>Focus on providing high-quality, comprehensive metadata in your SDMX files. This is the single most impactful way to ensure your data can be more easily mapped and utilized.</td></tr></tbody></table></figure>



<p class="wp-block-paragraph">To see an example, we have used these tools to <a href="https://github.com/datacommonsorg/data/tree/master/statvar_imports/oecd/quarterly_gdp">import</a> the <a href="https://data-explorer.oecd.org/vis?fs%5B0%5D=Topic%2C1%7CEconomy%23ECO%23%7CNational%20accounts%23ECO_NAD%23&amp;fs%5B1%5D=Topic%2C3%7CEconomy%23ECO%23%7CNational%20accounts%23ECO_NAD%23%7CGDP%20and%20non-financial%20accounts%23ECO_NAD_GNF%23%7CGDP%20and%20components%23ECO_NAD_GNF_GDP%23&amp;pg=0&amp;fc=Topic&amp;snb=22&amp;vw=tb&amp;df%5Bds%5D=dsDisseminateFinalDMZ&amp;df%5Bid%5D=DSD_NAMAIN1%40DF_QNA_EXPENDITURE_GROWTH_OECD&amp;df%5Bag%5D=OECD.SDD.NAD&amp;df%5Bvs%5D=&amp;dq=Q..AUS%2BAUT%2BBEL%2BCAN%2BCHE%2BCHL%2BCOL%2BCRI%2BCZE%2BDEU%2BDNK%2BESP%2BFIN%2BEST%2BFRA%2BGBR%2BGRC%2BHUN%2BISL%2BLTU%2BISR%2BITA%2BJPN%2BKOR%2BLUX%2BLVA%2BMEX%2BNLD%2BNOR%2BNZL%2BPOL%2BPRT%2BSVK%2BSVN%2BSWE%2BTUR%2BUSA%2BOECD%2BG20%2BG7%2BUSMCA%2BOECDE%2BEA20%2BEU27_2020...B1GQ......G1.&amp;lom=LASTNPERIODS&amp;lo=5&amp;to%5BTIME_PERIOD%5D=false&amp;ly%5Bcl%5D=TIME_PERIOD&amp;ly%5Brw%5D=REF_AREA">OECD&#8217;s quarterly GDP data</a>, which can be <a href="https://datacommons.org/tools/statvar#sv=Adjusted_GrowthRate_GrossDomesticProduct_EconomicActivity_QuarterOnChange">explored</a> in Data Commons.</p>



<h3 class="wp-block-heading">What&#8217;s next?</h3>



<p class="wp-block-paragraph">To address the current manual mapping effort and further automate the pipeline, our future roadmap is focused on following enhancements, with releases planned across the coming quarters:</p>



<ul class="wp-block-list">
<li><strong>SDMX 3.0 support</strong>: We will add support for version 3.0 of the standard as it gains wider adoption.</li>



<li><strong>Auto-schematization</strong>: We plan to leverage SDMX&#8217;s rich metadata to automatically generate schema mappings, reducing the manual effort required to integrate new datasets.</li>



<li><strong>Enhanced auto-refresh</strong>: Future improvements will enable checking SDMX metadata for data availability and triggering updates only when new data is released.</li>
</ul>



<p class="wp-block-paragraph">We look forward to seeing the new and interesting datasets that the community will bring to Data Commons!</p>



<p class="wp-block-paragraph"></p>
