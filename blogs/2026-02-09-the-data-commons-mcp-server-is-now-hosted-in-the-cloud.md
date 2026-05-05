---
title: "The Data Commons MCP server is now hosted in the cloud!"
url: "https://blog.datacommons.org/2026/02/09/the-data-commons-mcp-server-is-now-hosted-in-the-cloud/"
date: "Mon, 09 Feb 2026 16:26:48 +0000"
author: "Kara Moscoe"
feed_url: "https://blog.datacommons.org/feed/"
---
<p class="wp-block-paragraph">In late 2025, we announced the Data Commons <a href="https://blog.datacommons.org/2025/10/02/announcing-the-data-commons-model-context-protocol-server/">Model Context Protocol (MCP) server</a> and the <a href="https://blog.datacommons.org/2025/12/02/announcing-the-data-commons-gemini-cli-extension/">Gemini CLI extension</a>. Both launches required that you install additional open-source Python tools and run the MCP Server package locally.</p>



<p class="wp-block-paragraph">Today, to make it easier for everybody to use <a href="http://datacommons.org">datacommons.org</a> with an LLM, we are providing a hosted Data Commons MCP service in Google Cloud Platform. Now you don&#8217;t have to run your own server – you can just connect to the free service and let Google manage the rest.</p>



<h3 class="wp-block-heading">Connect today!</h3>



<p class="wp-block-paragraph">If you&#8217;re already using the Data Commons Gemini CLI extension, you don&#8217;t need to do anything. The next time you run Gemini CLI, the extension will automatically update itself to connect to the server over the web instead of starting up a local server instance. If you haven&#8217;t used the extension before, see <a href="https://docs.datacommons.org/mcp/run_tools.html#extension">Use the Gemini CLI extension</a> to get started.</p>



<p class="wp-block-paragraph">If you&#8217;re using Gemini CLI without the extension, or any other agent, you&#8217;ll need to update your configuration to point to the hosted server. Along with a <a href="http://apikeys.datacommons.org">Data Commons API key</a>, the snippet below is all you need. For complete details, see <a href="https://docs.datacommons.org/mcp/run_tools.html#use-gemini-cli">Use Gemini CLI</a>.</p>



<pre>"mcpServers": {
   "datacommons-mcp": {
      "httpUrl": "https://api.datacommons.org/mcp",
      "headers": {
        "X-API-Key": "YOUR DC API KEY"
      }
   }
}</pre>



<p class="wp-block-paragraph">And as always, if you’re interested in sharing your cool usage of Data Commons or have feedback, please email us at <a href="mailto:support@datacommons.org">support@datacommons.org</a>.&nbsp;</p>



<p class="wp-block-paragraph"><strong>Note:</strong> The hosted MCP server can only be used to query <a href="http://datacommons.org">datacommons.org</a>. If you&#8217;re running your own Custom Data Commons instance, you&#8217;ll still need to run your own MCP server. See <a href="https://docs.datacommons.org/custom_dc/run_mcp_tools.html">Run MCP tools</a> for more information.</p>



<p class="wp-block-paragraph"></p>
