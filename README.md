# KiWi Logo

### Designed by Consumers for Consumers 
```{r include=FALSE}
libs = c("rvest", "magrittr", "stringr", "httr", "furrr", "plotly", "ggplot2", "DT", "readxl", "dplyr")
lapply(libs, require, character.only = TRUE)
```
-------
background-image: url(https://i.pinimg.com/originals/1b/db/46/1bdb46cf377ae1c06617d6b9bfc54793.png)
background-size: 100px
background-position: 90% 8%
  
# Accomodation in Milan is a Mess
##Socio-Economic Circumstances:
- Too much *Demand* wrt to the available *Offer* 

--

- Rent Prices, for the same reason, are .red[**Overshooted**]
  
--
  
- .red[**Condominium**] is a really tough component of the monthly budget and actually It does not make so much sense

--
  
- Asymmetry of information between you and the agency Advisor

--
  
- Time factor: you are in a Hurry, houseolds are **Not**
  
---
background-image: url(https://i.pinimg.com/originals/1b/db/46/1bdb46cf377ae1c06617d6b9bfc54793.png)
background-size: 100px
background-position: 90% 8%
  
# The questions you come up 
##The most of us:
  
- Where do phisically I have to search?  --> **Immobiliare.it**<sup>[1]</sup> 
  
--
  
- Where do I need my apt to be? --> **select zone** 
  
--
  
- Once you have spotted it '(if you made it') you should verify *if it is a good deal*
  
--

  
- Are they trying to steal my money? Am I going to pay a fair price?
  
--
  
- Hey, **I REALLY NEED SOMEONE TO TELL ME IF IT IS GOOD OR NOT**, let's find something which is similar to my option, oh I would say a *Comparable*

--

- Do you know how many are the chances to find a **Comparable** ?

.footnote[
[1] Here it is [immobiliare](https://www.immobiliare.it/), n1 player in online mrkt

]

---
background-image: url(https://video-images.vice.com/_uncategorized/1498664480808-Screen-Shot-2017-06-28-at-164017.png)
background-size: 700px
---
# Odds

Now let's try this:
*TRY* to compute the probability to find an apartement given some certain characteristics (even location) equal to someone else with the **SAME** chars

- Randomly select 1 obs from the dataset

--

- Filter the dataset given the characteristics *(rand selct)* both .red[*Streched*] and .blue[*Strict*]

--

- Compare the `len` output of the `vec`  wrt to dataset `len`
