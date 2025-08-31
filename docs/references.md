# References

## Modelling & Analysis

<table style="width: 85%; margin-left: 35px; vertical-align: top; font-size: .7rem;">
  <colgroup>
      <col span="1" style="width: 43.5%;">
  </colgroup>
  <thead><tr style="text-align: left"><th>PAPERS, BOOKS, etc.</th></tr></thead>
  <tr><td><a href="https://link.springer.com/book/10.1007/978-3-030-76124-0" target="_blank">Bayesian Inference of State Space Models</a></td></tr>
  <tr><td><a href="https://projecteuclid.org/journals/annals-of-applied-statistics/volume-9/issue-1/Inferring-causal-impact-using-Bayesian-structural-time-series-models/10.1214/14-AOAS788.full" target="_blank">Inferring causal impact using Bayesian structural time-series models</a></td></tr>
  <tr><td><a href="https://direct.mit.edu/books/oa-monograph-pdf/2514321/book_9780262256834.pdf">Gaussian Processes for Machine Learning</a></td></tr>
  <tr><td><a href="https://link.springer.com/article/10.1007/s10994-021-05946-3" target="_blank">Aleatoric and epistemic uncertainty in machine learning: an introduction to concepts and methods</a></td></tr>
  <tr><td><a href="https://otexts.com/fpp2/stationarity.html" target="_blank">Forecasting Principles & Practice: Stationarity</a></td></tr>
  <tr><td><a href="https://www.nature.com/articles/s41598-024-73405-9" target="_blank">Using ARIMA and ETS models for forecasting water level changes for sustainable environmental management</a>, Scientific Reports 14, 22444 (2024)</td></tr>
  <tr><td><a href="https://otexts.com/fpp3/ets-forecasting.html">Forecasting with ETS Models</a></td></tr>
  <tr><td><a href="https://otexts.com/fpp3/arima-ets.html">ARIMA vs ETS</a></td></tr>
  <tr><td><a href="https://www.bridgetext.com/log-transforming-time-series-data-in-r" target="_blank">Natural Logarithm Transformations</a></td></tr>
</table>


## Programming, Development

<table style="width: 85%; margin-left: 35px; vertical-align: top; font-size: .7rem;">
  <colgroup>
      <col span="1" style="width: 18.5%;">
      <col span="1" style="width: 43.5%;">
  </colgroup>
  <thead><tr style="text-align: left"><th>&nbsp;</th><th>Notes</th></tr></thead>
  <tr><td>linux</td><td><a href="https://manpages.ubuntu.com/manpages/trusty/man1/" target="_blank">ubuntu man pages</a></td></tr>
  <tr><td>time & formatting</td>
      <td><ul>
          <li>time converters: <a href="https://unixtime.org" target="_blank">https://unixtime.org</a>, <a href="https://time.is/Unix_time_converter" target="_blank">unix time converter</a></li>
          <li><a href="https://en.wikipedia.org/wiki/ISO_8601#Durations" target="_blank">durations</a></li>
          <li><a href="https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-codes" target="_blank">formatting (python)</a></li>
      </ul></td></tr>
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
      <td><a href="https://hub.docker.com/_/nginx" target="_blank">nginx @ docker hub</a>, <a href="https://toxigon.com/setting-up-nginx-with-docker" target="_blank">setting-up docker nginx</a>, <a href="https://www.uptimia.com/questions/how-to-run-nginx-in-the-foreground-within-a-docker-container#implementing-the-solution-in-docker" target="_blank">running nginx in the foreground within a docker container</a>, <a href="https://itnext.io/dockerizing-modern-web-apps-cd9667eebf44" target="_blank">docker & modern web apps</a>, <a href="https://www.socketxp.com/iot/remote-access-nginx-web-server-from-internet/" target="_blank">how to remotely access a NGINX web server from the internet</a>, <a href="https://www.thecoderscamp.com/nginx-g-daemon-off/" target="_blank">nginx -g 'daemon off;'</a>, <a href="https://github.com/devasthali-os/nginx-base/blob/master/Dockerfile" target="_blank">a Dockerfile example</a>, <a href="https://nginx.org/en/docs/beginners_guide.html#conf_structure" target="_blank">conf</a>, <a href="https://server.hk/blog/14461/" target="_blank">MIME (Multipurpose Internet Mail Extensions) Types</a>, <a href="https://www.slingacademy.com/article/nginx-mime-types-the-complete-guide/" target="_blank">MIME Types</a>, <a href="https://www.slingacademy.com/article/nginx-error-cannot-load-css-js-files/">nginx & loading errors</a></td>
  </tr>
  <tr><td>live server</td><td><a href="https://itnext.io/dockerizing-modern-web-apps-cd9667eebf44">live server & modern web apps</a>, <a href="https://github.com/tapio/live-server" target="_blank">live server @ github</a>, <a href="https://www.npmjs.com/package/live-server">live server @ npm</a></td>
  </tr>
  <tr><td>vi & vim</td><td><a href="https://linuxsimply.com/cheat-sheets/vi/">vi reference sheet</a>, <a href="https://vim.rtorr.com">vim reference sheet</a>, <a href="https://www.redhat.com/en/blog/beginners-guide-vim">beginners guide @ redhat</a></td></tr>
  <tr><td>graphing</td>
      <td><ul>
        <li>highcharts: <a href="https://api.highcharts.com/class-reference/Highcharts.Time#dateFormat">the date formats of highcharts</a>, <a href="https://www.highcharts.com/docs/stock/data-grouping">data grouping</a></li>
        <li>dropdowns & lists: <a href="https://wpdean.com/css-dropdown-menus/">1</a>, <a href="https://jsfiddle.net/cL2x7/">2</a>, <a href="https://www.geeksforgeeks.org/how-to-creating-html-list-from-javascript-array/">3</a></li>
      </ul></td></tr>
  <tr><td>JavaScript Modules</td><td><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules" target="_blank">modules</a>, <a href="https://javascript.info/modules" target="_blank">modules</a>, <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors/import_decl_module_top_level#importing_in_a_non-module_script" target="_blank">module errors</a></td></tr>
</table>

<br>
<br>

<br>
<br>

<br>
<br>

<br>
<br>
