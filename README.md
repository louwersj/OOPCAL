# OOPCAL - Open Oracle Public Cloud API Library
OOCAL, Open Oracle Public Cloud API Library is set of pre-defind bash functions and scripts to be used with the Oracle Public cloud. The general intend is to provide standard functions, scripts and solutions to be used with Oracle cloud products to enable automation when deploying new instances and code on the Oracle Public Cloud. This includes functions like first-boot options when deploying a new compute instance. 

By using OOPCAL developers who promote products to the Oracle Public Cloud can easily make use of the standard functions provided by both Oracle and the OOPCAL solution. 

### current project status and version
The current status is ALPHA - v01. This means that we are currently working on the first stable release of OOPCAL. We do NOT recommend using OOPCAL in production yet. We do encourage developers at this moment to participate in supporting the development and to help us develop the first stable release. 

### General use - custom scripting
to make use of the OOPCAL functions you will have to ensure that you include OOPCAL by calling it in your bash script by using the below call to OOPCAL:

_source /opt/oopcal/lib/oopcal.lib_

To find usable examples on how you can use OOPCAL please refer to the example directory which holds some example scripts that can be used as a reference for developers who intend to build their own custom scripts based upon OOPCAL

### General use - first boot
- to be completed - 

## Compute Cloud Functions
All functions used for the compute functions from th Oracle Public Cloud are stored in the opc_comp_api_functions.lib functions library. The below mentiond functions can be found in this library. 

**_ccVm functions_**
Functions used for internal use within the VM are recognizable as they start with ccVm "Compute Cloud Virtual Machine". The functions take "aim" against the internal API which can be accessed from within a VM at http://192.0.0.192/. This can be used (for example) to configure a newely created virtual machine based upon this information.

##### _ccVmGetNumOfVersions_
_Function input_      : (none)  
_Function output_     : number of API versions currently available in the public API   
_Function error code_ : In case of an error retrieving the values the function will return the code ERROR  
_Additional info_     : none.

##### _ccVmGetVersions_
_Function input_      :
_Function output_     :
_Function error code_ : In case of an error retrieving the values the function will return the code ERROR
_Additional info_     : none

##### _ccVmGetAmiId_
_Function input_      : 
_Function output_     : 
_Function error code_ : In case of an error retrieving the values the function will return the code ERROR  
_Additional info_     : none.

##### _ccVmGetAmiLaunchIndex_

##### _ccVmGetAmiManifestPath_

##### _ccVmGetAncestorAmiIds_



##### _ccVmGetBlockDeviceMapping_

##### _ccVmGetInstanceId_
##### _ccVmGetInstanceType_
##### _ccVmGetKernelId_
##### _ccVmGetLocalHostname_
##### _ccVmGetLocalIpv4_
##### _ccVmGetProductCodes_
##### _ccVmGetPublicHostname_
##### _ccVmGetPublicIpv4_
##### _ccVmGetRamdiskId_
##### _ccVmGetReservationId_
##### _ccVmGetSecurityGroups_
##### _ccVmGetNumOfPublicKeys_
##### _ccVmGetPublicKeyType_
##### _ccVmGetPublicSshKey_
_Function input_      : 
  the "id" of the key (note: ccVmGetNumOfPublicKeys will give you the number of keys, do remember; "id's" start at 0  
_Function output_     : 
  the public SSH key for the given "id"   
_Function error code_ : 
  In case of an error retrieving the values the function will return the code ERROR  
_Additional info_     :   
  none.
