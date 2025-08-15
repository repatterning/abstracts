# References

Focusing on time series modelling & analysis, <a href="https://aws.amazon.com/what-is/compute" target="_blank">compute</a>, etc.

## Weather Warning Briefs

* [Warnings](https://weather.metoffice.gov.uk/guides/warnings)
* [RSS feeds from the Met Office](https://weather.metoffice.gov.uk/guides/rss)
* [email alerts](https://www.metoffice.gov.uk/about-us/news-and-media/media-centre/subscribe-to-email-alerts)
* [National Severe Weather Warnings Service Public API](https://metoffice.github.io/nswws-public-api)

and

* [Materials & RSS](https://squidfunk.github.io/mkdocs-material/setup/setting-up-a-blog/#rss)

<br>

## Time Series Modelling & Analysis

* [Forecasting Principles & Practice: Stationarity](https://otexts.com/fpp2/stationarity.html)
* [Stationarity, De-trending, Tests](https://www.statsmodels.org/dev/examples/notebooks/generated/stationarity_detrending_adf_kpss.html)
* [Model Identification for Southern Oscillations Data](https://www.itl.nist.gov/div898/handbook/pmc/section4/pmc4461.htm)
* [Robust de-trending, re-referencing, outlier detection, and inpainting for multichannel data](https://pmc.ncbi.nlm.nih.gov/articles/PMC5915520/)
* [Using ARIMA and ETS models for forecasting water level changes for sustainable environmental management](https://www.nature.com/articles/s41598-024-73405-9)
* [Partial Auto-correlation Plot](https://www.itl.nist.gov/div898/handbook/pmc/section4/pmc4463.htm)
* [Auto-correlation Plot](https://www.itl.nist.gov/div898/handbook/eda/section3/autocopl.htm): For investigating questions such as (From <abbr title="National Institute of Standards and Technology">NIST</abbr>)
  * Is an observation related to an adjacent observation?
  * Is an observation related to an observation twice-removed? (etc.)
  * Is the observed time series white noise?
  * Is the observed time series sinusoidal?
  * Is the observed time series autoregressive?
* [Statistical forecasting: notes on regression and time series analysis](https://people.duke.edu/~rnau/411home.htm)
  * [Identifying the order of differencing in an ARIMA model](https://people.duke.edu/~rnau/411arim2.htm)
  * [Identifying the numbers of AR or MA terms in an ARIMA model](https://people.duke.edu/~rnau/411arim3.htm)
* [Natural Logarithm Transformations](https://www.bridgetext.com/log-transforming-time-series-data-in-r)

<br>

## Time & Formatting

* [Epoch Time](https://unixtime.org)
* [UNIX Time Converters](https://time.is/Unix_time_converter)
* [Time Durations](https://en.wikipedia.org/wiki/ISO_8601#Durations)
* [Time Formatting Codes](https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-codes)


<br>

## Programming, Development

<table style="width: 85%; margin-left: 35px; vertical-align: top; font-size: .7rem;">
  <colgroup>
      <col span="1" style="width: 18.5%;">
      <col span="1" style="width: 43.5%;">
  </colgroup>
  <thead><tr style="text-align: left"><th>&nbsp;</th><th>Notes</th></tr></thead>
  <tr><td>linux</td><td>[ubuntu man pages](https://manpages.ubuntu.com/manpages/trusty/man1/)</td></tr>
  <tr>
    <td>GitHub Actions</td>
    <td>Core<ul>
      <li><a href="https://github.com/docker/login-action/releases" target="_blank">docker/login-action</a></li>
      <li><a href="https://github.com/docker/metadata-action/releases" target="_blank">docker/metadata-action</a></li>
      <li><a href="https://github.com/aws-actions/configure-aws-credentials/releases" target="_blank">aws-actions/configure-aws-credentials</a></li>
      <li><a href="https://github.com/aws-actions/amazon-ecr-login/releases" target="_blank">aws-actions/amazon-ecr-login</a></li></ul>
      Extra<ul>
        <li><a href="https://docs.docker.com/reference/dockerfile/" target="_blank">Dockerfile</a></li>
        <li><a href="https://pip.pypa.io/en/stable/reference/requirements-file-format/" target="_blank">requirements.txt</a></li>
        <li><a href="https://docs.docker.com/reference/cli/docker/container/run/" target="_blank">docker run</a></li></ul>
    </td>
  </tr>
  <tr><td>NGINX Servers</td>
      <td><a href="https://hub.docker.com/_/nginx" target="_blank">nginx: docker hub</a>, <a href="https://toxigon.com/setting-up-nginx-with-docker" target="_blank">setting-up docker nginx</a>, <a href="https://www.uptimia.com/questions/how-to-run-nginx-in-the-foreground-within-a-docker-container#implementing-the-solution-in-docker" target="_blank">docker nginx</a>, <a href="https://itnext.io/dockerizing-modern-web-apps-cd9667eebf44" target="_blank">extra help</a>, <a href="https://www.socketxp.com/iot/remote-access-nginx-web-server-from-internet/" target="_blank">more</a>, <a href="https://www.thecoderscamp.com/nginx-g-daemon-off/" target="_blank">nginx -g 'daemon off;'</a>, <a href="https://github.com/devasthali-os/nginx-base/blob/master/Dockerfile" target="_blank">Dockerfile</a>, <a href="https://nginx.org/en/docs/beginners_guide.html#conf_structure" target="_blank">conf</a>, <a href="https://server.hk/blog/14461/" target="_blank">MIME (Multipurpose Internet Mail Extensions) Types</a>, <a href="https://www.slingacademy.com/article/nginx-mime-types-the-complete-guide/" target="_blank">MIME Types</a>, <a href="https://www.slingacademy.com/article/nginx-error-cannot-load-css-js-files/">load error example</a></td>
  </tr>
</table>

<br>


### live server

* [live server](https://itnext.io/dockerizing-modern-web-apps-cd9667eebf44)
* [liver server @ github](https://github.com/tapio/live-server)
* [liver server @ npm](https://www.npmjs.com/package/live-server)

<br>

### vim & vi

* [vi](https://linuxsimply.com/cheat-sheets/vi/)
* [vim](https://vim.rtorr.com)
* [vim](https://www.redhat.com/en/blog/beginners-guide-vim)

<br>

### JavaScript Modules

* [Modules](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules)
* [Modules](https://javascript.info/modules)
* [Module Errors](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors/import_decl_module_top_level#importing_in_a_non-module_script)
* [SCRIPT](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/script)

<br>

### JavaScript & Graphing

* [fetch](https://javascript.info/fetch)
* [1](https://wpdean.com/css-dropdown-menus/), [2](https://jsfiddle.net/cL2x7/), [3](https://www.geeksforgeeks.org/how-to-creating-html-list-from-javascript-array/)
* High Charts
  * [data grouping](https://www.highcharts.com/docs/stock/data-grouping)
  * [the date formats](https://api.highcharts.com/class-reference/Highcharts.Time#dateFormat)

<br>
<br>

<br>
<br>

<br>
<br>

<br>
<br>
