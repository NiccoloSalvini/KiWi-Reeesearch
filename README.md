
<!-- README.md is generated from README.Rmd. Please edit that file -->

# KiWi Reeesearch <img src="https://i.pinimg.com/originals/1b/db/46/1bdb46cf377ae1c06617d6b9bfc54793.png" align="right" height="80" />

*author*: **[Niccolò Salvini](https://niccolosalvini.netlify.app/)** ,
**[Jędrzej Dziedziul](https://www.linkedin.com/in/jedrzej-dziedziul/)**

*date*: 2020-05-06

<br> <br>

## Deployment happens:

–\> see the *slides* **[HERE](https://kiwiresearch.netlify.com/#1)** –\>
see the *Shiny APP*
**[HERE](https://jedrzejdziedziul.shinyapps.io/Housing/)**

## Description:

This tool has been designed to explore apartements in Milan next to your
preferred location and compute a monthly rent price estimation given the
spatial coordinates and the expected characteristics of the house, such
as: rooms square meters. It is composed by a `Shiny` deployed from a
bitbucket repo into [shinyapps.io](https://www.shinyapps.io/) and a set
of `xaringan` slides deployed on [Netlify](https://www.netlify.com/).
House data are scraped from [immobiliare](https://www.immobiliare.it/).
Full explanation on the slides.

## Visuals:

<p align="center">

<img src="snapshot/screenshot 1.png" width="1906" />

</p>

<p align="center">

<img src="snapshot/screenshot 2.png" width="1913" />

</p>

<p align="center">

<img src="snapshot/screenshot 3.png" width="1913" />

</p>

<p align="center">

<img src="snapshot/screenshot 4.png" width="1913" />

</p>

## Dependecies

``` r
libs = c("rvest", "magrittr", "stringr", "httr",
"furrr", "plotly", "ggplot2", "DT", "readxl", "dplyr")

new.packages = libs[!(libs %in% installed.packages()[,"Package"])]
if(length(new.packages)) install.packages(new.packages)
```

## Usage:

the first tab-panel in the tab-set let you explore the available houses
on the Milano house market, then once you have find the location of the
apartement you right click it. This will assign a marker in `leaflet`
object. This marker will be cached in the second tab panel, the *price
prediciton calculator*, where you can also specify other characteristics
of the desired house. An autoML model will give the estimation in the
lower down part on the left.  
In the right drop-down column you can discover other further options to
select and the autoML will do its job in parallel.

## Project status:

this project is still `IN ITINERE`, but it has stopped since my
university class is completed.

## Next features:

  - implement auto-scraping functions
  - choose boostrap .css style
  - better
UX

## License:

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Licenza Creative Commons" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />Quest’opera
è distribuita con Licenza
<a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative
Commons Attribuzione 4.0 Internazionale</a>.
