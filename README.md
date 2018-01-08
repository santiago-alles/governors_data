# governors_data
Governors in Argentina, 1973-2017
=================================

Governors are powerful actors in Latin American federal countries, and Argentina is an example of a robust federal system.

Governors are powerful actors, with abundant fiscal resources; large influence over the organization of national parties, candidate nomination and the career of national legislators; a predominant position in state-level elections; and an active participation in the national policymaking process.

This dataset provides information of the gubernatorial elections in Argentina since 1973. It comprises information of:

(a) elected governors and lieutenant governors,<br />
(b) gubernatorial election rules, and<br />
(c) results of the gubernatorial election.

In total, the data contain information on 236 gubernatorial elections that occurred in Argentina from 1973 through 2017.

The sources of the data are reported with the definition of the variables. The Appendix reports a complete list of the sources of election results, by province and year.

Data Availability
------------------

Data can be directly called from the repository using Hadley Wickham's <a href="https://cran.r-project.org/web/packages/readr/readr.pdf" target="_blank">readr</a> package:

<pre><code>require(readr)
url <- 'https://raw.githubusercontent.com/santiago-alles/governors_data/master/'
file <- 'ProvGov_ARG19732017_v20180108.csv'
read_csv(paste(url, file, sep='/')) -> dat
</code></pre>

Special characters may appear in name and last name variables. Character strings might be converted to <code>UTF-8</code> encoding using <code>iconv</code>:

<pre><code>iconv(x, from = 'latin1', to = 'UTF-8')</code></pre>

Suggested Citation
------------------

When using this dataset, please cite:

Alles, Santiago. 2018. <i>Gubernatorial Elections in Argentina, 1973-2017</i>. Data version: v20180108.<br />Available at: http://santiago-alles.net/governors_data.

Data Releases
------------------

Previous releases of this dataset:
<pre>"Governors in Argentina, 1983-2015," v20170504
"Governors in Argentina, 1983-2015," v20161124</pre>
