# Data Collection Monitoring

This is a report template for Data Collection Monitoring.

it is set up here to allow for automation with a direct connection to UNHCR kobo server using an authentication token.

In most cases, Survey Data should rather be analyzed only once it has been curated and documented within UNHCR Internal Data Library: http://ridl.unhcr.org. Data Collection Quality Monitoring is actually the outlier - in such situation, you need to review on a high Frequency Level, how well the data collection is going. 

The approach from this report build from [High Frequency Checks](https://edouard-legoupil.github.io/HighFrequencyChecks/docs/).

Below is a step by step how to in order to configure the automation.

 
## Step 1 - Set up and/or refresh the `manifest.json`

You first need to create a documentation file - which allow the Rstudio server to regenerate your report. This files is created by th e `rsconnect::writeManifest`.

Note that if you are the one developing any of this package, you will first need to re-install them from github or gitlab for the manisfest file to be correctly written. See more documentation here: [Git Backed Content - RStudio Connect: User Guide](https://docs.rstudio.com/connect/user/git-backed/)

```{r}

# devtools::install_github("rstudio/rsconnect")

# rsconnect::writeManifest(appPrimaryDoc = "DataCollectionMonitoring.Rmd")
```

## Step 2 -  Publish the report to Rstudio Connect from Github

Got to UNHCR Rstudio server - [http://rstudio.unhcr.org](http://rstudio.unhcr.org) - you need first to have a license associated to your account - Contact Global Data Service Data Science team for that.
 
![ ](https://raw.githubusercontent.com/unhcr-americas/DataCollectionMonitoring/main/fromGit.png) 



![ ](https://raw.githubusercontent.com/unhcr-americas/DataCollectionMonitoring/main/fromGit2.png)


![ ](https://raw.githubusercontent.com/unhcr-americas/DataCollectionMonitoring/main/fromGit3.png)



## Step 3 -  Set up your kobotoolbox API key within Rstudio Connect

You need now to set up the kobotoolbox authentication token within the Rstudio server so that the server can actually pull the data from Kobotoolbox in order to regenerate the Report.

![ ](https://raw.githubusercontent.com/unhcr-americas/DataCollectionMonitoring/main/fromGit4.png)

![ ](https://raw.githubusercontent.com/unhcr-americas/DataCollectionMonitoring/main/fromGit5.png)


![ ](https://raw.githubusercontent.com/unhcr-americas/DataCollectionMonitoring/main/fromGit6.png)


## Step 4 -  Set up report frequency generation and sending it to your email


![ ](https://raw.githubusercontent.com/unhcr-americas/DataCollectionMonitoring/main/fromGit7.png)

et voila...

![ ](https://raw.githubusercontent.com/unhcr-americas/DataCollectionMonitoring/main/fromGit8.png)


## Step 5 -  Use power automate to forward automatically the email with the report to the data supervisor
 
[Microsoft Power Automate](https://make.powerautomate.com/) is a convenient way to automatically re-forward the generated report to your surrvey coordinator and data collection supervisor.





