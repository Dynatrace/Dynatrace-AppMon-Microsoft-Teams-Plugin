# MS Teams
Microsoft Teams integration for Dynatrace
This integration works via WebHooks for Microsoft Teams.

I used the code from [HipChat](https://github.com/dynaTrace/Dynatrace-HipChat-Plugin) to maker it work. Huge thanks to them.


Tested with Dynatrace 7.0.6.1013 this works.

![Incident Started](https://github.com/tutnes/Dynatrace-MSTeams-Integration-Plugin/raw/master/images/readme/incident_started.png "Incident Started")

![Incident Ended](https://github.com/tutnes/Dynatrace-MSTeams-Integration-Plugin/raw/master/images/readme/incident_ended.png "Incident Ended")



## Installation

### Create Web Hook in a channel
![Add connector](https://github.com/tutnes/Dynatrace-MSTeams-Integration-Plugin/raw/master/images/readme/add_connector.png "Add connector")

Select the options for the channel you want to have the notifications in. 
Then click on the Connectors.

![Select Webhook](https://github.com/tutnes/Dynatrace-MSTeams-Integration-Plugin/raw/master/images/readme/select_incoming_webhook.png "Select Webhook")

Select the Incoming Webhook

![Configure Webhook](https://github.com/tutnes/Dynatrace-MSTeams-Integration-Plugin/raw/master/images/readme/configure_webhook.png "Configure Webhook")

Choose a name for the Webhook, and if you want to, an image.


![Copy Webhook](https://github.com/tutnes/Dynatrace-MSTeams-Integration-Plugin/raw/master/images/readme/copy_webhook.png "Copy Webhook")

Copy the Webhook URL and keep it. Click Done.

## Dynatrace Configuration
Install the plugin



![Configure plugin](https://github.com/tutnes/Dynatrace-MSTeams-Integration-Plugin/raw/master/images/readme/configure_dynatrace.png "Configure Plugin") 

Configure the plugin to point to the Webhook URL from the previous section

![Configure Incidentrule](https://github.com/tutnes/Dynatrace-MSTeams-Integration-Plugin/raw/master/images/readme/edit_incident_rule.png "Configure Incidentrule")

Add the plugin as an action on an Incident Rule

## Future development
It is entirely possible to use the Action buttons in Teams to close Incidents with comments.
This should be a future work.