# Majestic extractor for Keboola
KBC Docker app for extracting data from Majestic [Majestic.com](http://majestic.com)

The Extractor gets list of campaign stats for previous day and saves the data to Storage API. Date of downloaded stats can be changed in configuration.


## Configuration

- **parameters**:
    - **token** - provided by Majestic.com (1)
    - **domain** - domain 
    - **commands** - Password to Srovnáme (2)
    - **bucket** - Name of bucket where the data will be saved

## Obtain token (1)

Token is generated by authorizing app via OpenApps mechanism.

1) Go to [Keboola extractor Open App](https://majestic.com/apps/KIU4A7AXAJ) Access granter
2) Click on Grant Access
3) Copy Access Token and paste into **token**(1) field


## Commands (2)
Commands are used for data download. You can find overview of commands at  [Majestic Developer Commands](http://developer-support.majestic.com/api/commands/).

For example you can paste to **commands**(2) following: `GetBackLinkData,GetRefDomains` 
