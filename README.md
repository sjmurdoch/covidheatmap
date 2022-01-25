# COVID-19 age demographics

The UK's COVID-19 dashboard plots a heatmap of cases by date, broken down into age brackets.
This is very interesting but somewhat limited because it clips data above 800 per 100k people
and (like the rest of the dashboard) [only uses 8 colours](https://github.com/publichealthengland/coronavirus-dashboard/blob/19f5712f5fdbe873472d771bb248bff3c7a1ff1a/src/common/utils/visualisation.js#L51).

To explore this data in more detail, this Jupyter notebook generates a similar heatmap, but using a continuous colour scale.
This avoids the distortion resulting from clipping and binning, allowing more features of the data to be seen.

Like the official dashboard, this uses [Plotly](https://plotly.com/) and so allows interactive scrolling and zooming.

Thanks to Pouria Hadjibagheri for the [helpful discussion](https://twitter.com/sjmurdoch/status/1485618794022289421) which led to this code being produced.

## Run this code in a browser

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sjmurdoch/covidheatmap/HEAD?labpath=covidheatmap.ipynb)
