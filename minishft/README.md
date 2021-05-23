## Minishift 

Minishift is used as below:\
1. To develop application locally in a containerized OKD cluster
2. To set-up the Development and Testing environment

## How to Install
1. Go to the url: https://www.okd.io/minishift/
2. Make sure to have and run hypervisor in the system: i use oracle VitualBox
3. GO to the release version (https://github.com/minishift/minishift/releases) and select the required version as per the platform and download ( https://github.com/minishift/minishift/releases/download/v1.34.3/minishift-1.34.3-windows-amd64.zip) : in my case, window.
4. Move the zip file where the VM is install: in my case, it is in C: drive.
5. Open up the CMD promp and point to the directory where minishift.exm present
6. Run the below command:
```
$ minishift.exe start --vm-driver virtualbox

```
when we ran the above command, the minishift.exe will execute and go to the internet, download the minishift ISO file, configure it and give us a url to access the portal.\
7. Give any username and password in the portal in order to log in.(it is unauthenticate)
8. BOOM!! we can use the total portal 

#### NOTE: Remember this is only of the Development and testing environment. NOT FOR PRODUCTION
