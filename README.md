![alt text](https://github.com/JKannekens/kontent-custom-element-sendpulse/blob/master/SendPulseMailingListSelector.gif "SendPulse mailing list selector")

# SendPulse mailing list selector for Kentico Kontent
This repository contains the source code of SendPulse mailing list selector custom element for Kentico Kontent. Created by <a href="https://www.truelime.nl/">TrueLime</a>

## Setup
1. Deploy the code to a secure public host
2. Follow the instructions in the Kentico Kontent documentation to add the element to a content model.
3. Configure the JSON parameters as detailed in the JSON Parameters section

## JSON Parameters
```
{
    "id": "<YOUR API ID>",
    "secret": "<YOUR API SECRET>"
}
```

## Response
Mailing lists are retrieved in an array of mailing list objects. After selecting a mailing list from SendPulse the object is saved in Kentico Kontent.
For more information see: https://sendpulse.com/br/integrations/api/bulk-email
```
[
{
    "id": "1",
    "name": "My first list",
    "all_email_qty": "1",
    "active_email_qty": "0",
    "inactive_email_qty": "1",
    "creationdate": "2015-04-20 08:52:40",
    "status": "0",
    "status_explain": "Active"
  },
  {
    "id": "2",
    "name": "My second list",
    "all_email_qty": "6",
    "active_email_qty": "0",
    "inactive_email_qty": "6",
    "creationdate": "2015-04-20 09:02:39",
    "status": "0",
    "status_explain": "Active"
  }
]
```

## Deploying
Netlify has made this easy. If you click the deploy button below, it will guide you through the process of deploying it to Netlify and leave you with a copy of the repository in your GitHub account as well.
<br>
<br>
<a href="https://app.netlify.com/start/deploy?repository=https://github.com/JKannekens/kontent-custom-element-sendpulse" rel="nofollow"><img src="https://camo.githubusercontent.com/be2eb66bb727e25655f1dcff88c2fdca82a77513/68747470733a2f2f7777772e6e65746c6966792e636f6d2f696d672f6465706c6f792f627574746f6e2e737667" alt="Deploy to Netlify" data-canonical-src="https://www.netlify.com/img/deploy/button.svg" style="max-width:100%;"></a>
