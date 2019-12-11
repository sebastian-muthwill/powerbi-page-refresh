# Power Bi page refresh

I have been searching for a way how to display a Power Bi report on a monitor or kiosk in fullscreen and refresh the page frequently. And found some bread crumbs which lead to this solution. This HTML page embeds Power Bi reports in an iframe and refreshs them by a given time. But wait, there is more! It is also possible to embed more then one report or page of a report and show so different pages. 

Functionalities:

- refresh reports frequently
- loop thru pages or reports
- fullscreen display or reports

## How to set up the page
The refresh interval can be set with setInterval() in seconds x milliseconds 

Example: for every 10 minutes set this to 600 x 1000
        setInterval(iSequencer,600 * 1000);
        
You can either refresh a single page or loop thru different dashboards or pages of a dashboard.
sites takes a list of webpages.
Paste here the embed link from the PowerBi Service.

Example: sites = ['https://google.com', 'https://ebay.com']

If the script should loop thru the pages of a dashboard, open each page in the service and copy the embed Url from each page.
You can also copy just the apendix "&pageName=ReportSectionxxxxxxxxxxxxxxxxxxxx" and append it to the Url. 

For a full documentation please refere to: https://powerbi.microsoft.com/en-us/blog/easily-embed-secure-power-bi-reports-in-your-internal-portals-or-websites/

## Ideas for further improvement

It is also possible to set filters thru url variables. So it could also be possible to change the same report with different filters.

For a full documentation please refere to: https://powerbi.microsoft.com/en-us/blog/easily-embed-secure-power-bi-reports-in-your-internal-portals-or-websites/