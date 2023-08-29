<h1>Detection rule collections</h1>

These Analytics rule collections can be used to quickly deploy multiple threat detection rules to new or demo environments. Be cautious when deploying these to production environments. These are rule templates that need to be parametrized to environment needs. These templates and .json files are based on default rule collection of Sentinel solution. Individual detection rules can be also found directly in Sentinel github page: https://github.com/Azure/Azure-Sentinel/tree/master/Detections 

<br/><br/>

List of Detection rules per .json file:

<table>
   <thead>
      <tr>
         <th>Name</th>
         <th>Json filename</th>
	 <th>Rule count</th>
	 <th>Comment</th>
      </tr>
   </thead>
   <tbody>
      <tr>
         <td>Aws</td>
         <td>ms-sentinel-aws-detection-rules-14022023</td>
	 <td>52 rules</td>
	 <td></td>
      </tr>
      <tr>
         <td>Azure Activity</td>
         <td>ms-sentinel-azure-activity-detection-rules-15022023</td>
	 <td>16 rules (2 NRT)</td>
	 <td>One rule has UEBA tables incluuded so remember to enable UEBA too.</td>
      </tr>
      <tr>
         <td>Azure AD</td>
         <td>ms-sentinel-azuread-detection-rules-02062023</td>
	 <td>50 rules</td>
	 <td></td>
      </tr>
      <tr>
         <td>Azure Key Vault</td>
         <td>ms-sentinel-key-vault-detection-rules-29082023</td>
	 <td>4 rules</td>
	 <td>Azure Key Vault connector needs to be enabled before use.</td>
      <tr>
      <tr>
         <td>Defender 365</td>
         <td>ms-sentinel-microsoftdefender365-detection-rules-02062023</td>
	 <td>9 rules</td>
	 <td>One rule has UEBA tables incluuded so remember to enable UEBA too.</td>
      <tr>
      <tr>
         <td>TI - 1</td>
         <td>ms-sentinel-threatintelligence-1-detection-rules-06062023</td>
	 <td>13 rules</td>
	 <td>Threat Intelligence rule templates for data connectors: Microsoft 365, Microsoft 365 Defender, Microsoft Defender for Cloud, Azure Active Directory, Azure Activity and Azure Key Vault</td>
      <tr>
         <td>Defender 365</td>
         <td>ms-sentinel-microsoftdefender365-detection-rules-02062023</td>
	 <td>9 rules</td>
	 <td>One rule has UEBA tables incluuded so remember to enable UEBA too.</td>
      <tr>
      <tr>	      
	   <tr>
         <td>Web Shells Threat Protection</td>
         <td>ms-sentinel-web-shells-threat-protection-detection-rules-29082023</td>
	 <td>3 rules</td>
	 <td>Defender 365 connector needs to be enabled before use.</td>   
   </tbody>
</table>

<br/><br/>
<br/><br/>

You can import these Sentinel analytics rule packs to your environment.
![image](https://user-images.githubusercontent.com/81473026/218717311-8462ebcf-79aa-4806-8f8a-cb668e5d7366.png)

Choose the .json file on the prompt. And see if the deployment succeeded in the upper right corner:
![image](https://user-images.githubusercontent.com/81473026/218717424-b5f19737-9727-4062-80b7-5a635dfb47de.png)

Default all the rules will be in state "Disabled".
<ol>
    <li>Option 1, You can select rules from the portal witch you would like to enable (Picture below)</li>
    <li>Option 2, You can change: "enabled": false, ==to==> "enabled": true, directly in the .json file. Example with Visual studio code and ctrl + f (Find and replace, just dont replace the groupingConfiguration parameters :))</li>
</ol>
	
![image](https://user-images.githubusercontent.com/81473026/218717484-b42845c0-ea28-4508-8ac3-2d27435272d6.png)

