Sync Azure Keyvault Secrets and Certificates between vaults
===========================================================

            

If you have a keyvault in your primary region and a secondary region, you may have a reason to sync up Keyvaults.


Possibly you need to sync a keyault from a primary Vault to a secondary Vault for Dev or Testing.


This script synchronizes secrets/keys based on the last modified time.


--


The Keyvault info used by this script is stored in a separate json metadata files, however it would be easy to just hard code the values in this script.


The json metadata file looks like this


 


e.g. primary





{
  'HubRGName' : 'AZC1-ADF-RG-P0',
  'KVName' : 'AZC1-ADF-P0-kvVault01'
}





e.g. secondary





{
  'HubRGName' : 'AZC1-ADF-RG-P0',
  'KVName' : 'AZC1-ADF-P0-kvVault01'
}

If you want to force a sync of a secret or certificate, you can disable and enable it and that will change the 'Updated' value.










 




        
    
TechNet gallery is retiring! This script was migrated from TechNet script center to GitHub by Microsoft Azure Automation product group. All the Script Center fields like Rating, RatingCount and DownloadCount have been carried over to Github as-is for the migrated scripts only. Note : The Script Center fields will not be applicable for the new repositories created in Github & hence those fields will not show up for new Github repositories.
