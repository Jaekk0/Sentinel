Detection rule collections 

These Analytics rule collections can be used to quickly deploy multiple threat detection rules to new or demo environments. Be cautious when deploying these to production environments. These are only rule templates that need to be parametrized to environment needs.

You can import these Sentinel analytics rule packs to your environment.
![image](https://user-images.githubusercontent.com/81473026/218717311-8462ebcf-79aa-4806-8f8a-cb668e5d7366.png)

Choose the .json file on the prompt. And see if the deployment succeeded in the upper right corner:
![image](https://user-images.githubusercontent.com/81473026/218717424-b5f19737-9727-4062-80b7-5a635dfb47de.png)

Default all the rules will be in state "Disabled".
<ol>
    <li>Option 1, You can select rules from the portal witch you would like to enable (Picture below)</li>
    <li>Option 2, You can change: "enabled": false, ==to==> "enabled": true, directly in the .json file. Example with Visual studio code and ctrl + f (Find and replace)</li>
</ol>
	
![image](https://user-images.githubusercontent.com/81473026/218717484-b42845c0-ea28-4508-8ac3-2d27435272d6.png)
