## Dynatrace EasyTravel BizOps Dashboards

If you previously loaded one of my old fastpacks, make sure to delete the old measures, BTs and Incidents. Layering this on top will create "copies" and there is a few bugs in the old fastpack. 

Once the fastpack is loaded, it will create a profile called WorkFlow. Just copy all the Measures, BTs and Incidents from the WorkFlow profile to your easyTravel profile. 

The source for each Dashboard will need to be changed as well as any dashboard links (WorkFlow Summary and Book Travel WorkFlow Dashboards). Might be easier to do a search and replace on the xml in the dashboard folder. 

You will also need to create a "Gold Standard" session store and point to that session file in the WorkFlow Comparison Dashboard.

And lastly, if you are using this against a local easyTravel install, you will need to replace the tripDetailsPanel.xhtml file in easyTravel (e.g. C:\Program Files\dynaTrace\easyTravel (x64)\customer\webapp\WEB-INF\includes\components). This is needed to track "Lost Revenue".
