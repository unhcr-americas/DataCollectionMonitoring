# Data Collection Monitoring

This is a report template for Data Collection Monitoring.

it is set up here to allow for automation.

 
## Step 1 - Set up and/or refresh the `manifest.json`

You first need to create a documentation file - which allow the Rstudio server to regenerate your report. This files is created by th e `rsconnect::writeManifest`.

Note that if you are the one developing any of this package, you will first need to re-install them from github or gitlab for the manisfest file to be correctly written. See more documentation here: [Git Backed Content - RStudio Connect: User Guide](https://docs.rstudio.com/connect/user/git-backed/)

```{r}

# devtools::install_github("rstudio/rsconnect")

# rsconnect::writeManifest(appPrimaryDoc = "DataCollectionMonitoring.Rmd")
```

## Step 2 -  Publish the report to Rstudio Connect from Github

Got to UNHCR Rstudio server - [http://rstudio.unhcr.org](http://rstudio.unhcr.org) - you need first to have a license associated to your account - Contact Global Data Service Data Science team for that.
 
![ ](https://github.com/unhcr-americas/DataCollectionMonitoring/raw/master/img/fromGit.png)


![ ](https://github.com/unhcr-americas/DataCollectionMonitoring/raw/master/img/fromGit2.png)



## Step 3 -  Set up your kobotoolbox API key within Rstudio Connect


## Step 4 -  Set up report frequency generation and sending it to your email


## Step 5 -  Use power automate to forward automatically the email with the report to the data supervisor
 
[Microsoft Power Automate](https://make.powerautomate.com/)



