# RaspiCameraSurveillance-Azure
Raspberry Pi Motion Camera with an Azure Website to remotely view the photos.

## Techonology and Framework Used
- Python
  - Azure Python SDK
- ASP.NET MVC
  - C#
  - Azure .NET SDK
  - Bootstrap
  - jQuery

## Deploy and Run
0. Connect PIR Sensor to GPIO 4 and setup Pi Camera.
1. Edit RaspbianProgram\pricam.py, replace YOURACCOUNT, YOURKEY, YOURCONTAINER with your azure storage account information.
2. Copy RaspbianProgram\pricam.py to Raspberry Pi, use "sudo python pricam.py" to run.
3. Edit AzureWebsite\PirCamWatcher\Web.config, replace StorageConnectionString, AzureStorageAccountContainer, AuthUserName, AuthPassword with your information
4. Deploy AzureWebsite to Microsoft Azure
5. You are good to go!
