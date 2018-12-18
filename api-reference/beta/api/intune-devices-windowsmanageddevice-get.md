---
title: Abrufen von windowsManagedDevice
description: Lesen Sie Eigenschaften und Beziehungen des WindowsManagedDevice-Objekts.
author: tfitzmac
ms.openlocfilehash: 51d5adb884779a850c9689ec8b25704cde916a13
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314056"
---
# <a name="get-windowsmanageddevice"></a><span data-ttu-id="56fbd-103">Abrufen von windowsManagedDevice</span><span class="sxs-lookup"><span data-stu-id="56fbd-103">Get windowsManagedDevice</span></span>

> <span data-ttu-id="56fbd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="56fbd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56fbd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="56fbd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="56fbd-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="56fbd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="56fbd-107">Lesen Sie Eigenschaften und Beziehungen des [WindowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="56fbd-107">Read properties and relationships of the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="56fbd-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="56fbd-108">Prerequisites</span></span>
<span data-ttu-id="56fbd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56fbd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56fbd-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="56fbd-111">Permission type</span></span>|<span data-ttu-id="56fbd-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="56fbd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56fbd-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="56fbd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="56fbd-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="56fbd-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="56fbd-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="56fbd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56fbd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="56fbd-116">Not supported.</span></span>|
|<span data-ttu-id="56fbd-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="56fbd-117">Application</span></span>|<span data-ttu-id="56fbd-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="56fbd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56fbd-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="56fbd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/managedDevices/{managedDeviceId}
GET /deviceManagement/managedDevices/{managedDeviceId}
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="56fbd-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="56fbd-120">Optional query parameters</span></span>
<span data-ttu-id="56fbd-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="56fbd-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="56fbd-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="56fbd-122">Request headers</span></span>
|<span data-ttu-id="56fbd-123">Header</span><span class="sxs-lookup"><span data-stu-id="56fbd-123">Header</span></span>|<span data-ttu-id="56fbd-124">Wert</span><span class="sxs-lookup"><span data-stu-id="56fbd-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56fbd-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="56fbd-125">Authorization</span></span>|<span data-ttu-id="56fbd-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="56fbd-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56fbd-127">Accept</span><span class="sxs-lookup"><span data-stu-id="56fbd-127">Accept</span></span>|<span data-ttu-id="56fbd-128">application/json</span><span class="sxs-lookup"><span data-stu-id="56fbd-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56fbd-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="56fbd-129">Request body</span></span>
<span data-ttu-id="56fbd-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="56fbd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56fbd-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="56fbd-131">Response</span></span>
<span data-ttu-id="56fbd-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [WindowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="56fbd-132">If successful, this method returns a `200 OK` response code and [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56fbd-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="56fbd-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="56fbd-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="56fbd-134">Request</span></span>
<span data-ttu-id="56fbd-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="56fbd-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}
```

### <a name="response"></a><span data-ttu-id="56fbd-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="56fbd-136">Response</span></span>
<span data-ttu-id="56fbd-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="56fbd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7567

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsManagedDevice",
    "id": "97842b67-2b67-9784-672b-8497672b8497",
    "userId": "User Id value",
    "deviceName": "Device Name value",
    "hardwareInformation": {
      "@odata.type": "microsoft.graph.hardwareInformation",
      "serialNumber": "Serial Number value",
      "totalStorageSpace": 1,
      "freeStorageSpace": 0,
      "imei": "Imei value",
      "meid": "Meid value",
      "manufacturer": "Manufacturer value",
      "model": "Model value",
      "phoneNumber": "Phone Number value",
      "subscriberCarrier": "Subscriber Carrier value",
      "cellularTechnology": "Cellular Technology value",
      "wifiMac": "Wifi Mac value",
      "operatingSystemLanguage": "Operating System Language value",
      "isSupervised": true,
      "isEncrypted": true,
      "isSharedDevice": true,
      "sharedDeviceCachedUsers": [
        {
          "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
          "userPrincipalName": "User Principal Name value",
          "dataToSync": true,
          "dataQuota": 9,
          "dataUsed": 8
        }
      ],
      "tpmSpecificationVersion": "Tpm Specification Version value",
      "operatingSystemEdition": "Operating System Edition value",
      "deviceFullQualifiedDomainName": "Device Full Qualified Domain Name value",
      "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "secureBootRequired",
      "deviceGuardVirtualizationBasedSecurityState": "rebootRequired",
      "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired"
    },
    "ownerType": "company",
    "managedDeviceOwnerType": "company",
    "deviceActionResults": [
      {
        "@odata.type": "microsoft.graph.deviceActionResult",
        "actionName": "Action Name value",
        "actionState": "pending",
        "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
        "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
      }
    ],
    "managementState": "retirePending",
    "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
    "chassisType": "desktop",
    "operatingSystem": "Operating System value",
    "deviceType": "windowsRT",
    "complianceState": "compliant",
    "jailBroken": "Jail Broken value",
    "managementAgent": "mdm",
    "osVersion": "Os Version value",
    "easActivated": true,
    "easDeviceId": "Eas Device Id value",
    "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
    "aadRegistered": true,
    "azureADRegistered": true,
    "deviceEnrollmentType": "userEnrollment",
    "lostModeState": "enabled",
    "activationLockBypassCode": "Activation Lock Bypass Code value",
    "emailAddress": "Email Address value",
    "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
    "azureADDeviceId": "Azure ADDevice Id value",
    "deviceRegistrationState": "registered",
    "deviceCategoryDisplayName": "Device Category Display Name value",
    "isSupervised": true,
    "exchangeLastSuccessfulSyncDateTime": "2017-01-01T00:00:45.8803083-08:00",
    "exchangeAccessState": "unknown",
    "exchangeAccessStateReason": "unknown",
    "remoteAssistanceSessionUrl": "https://example.com/remoteAssistanceSessionUrl/",
    "remoteAssistanceSessionErrorDetails": "Remote Assistance Session Error Details value",
    "isEncrypted": true,
    "userPrincipalName": "User Principal Name value",
    "model": "Model value",
    "manufacturer": "Manufacturer value",
    "imei": "Imei value",
    "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
    "serialNumber": "Serial Number value",
    "phoneNumber": "Phone Number value",
    "androidSecurityPatchLevel": "Android Security Patch Level value",
    "userDisplayName": "User Display Name value",
    "configurationManagerClientEnabledFeatures": {
      "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
      "inventory": true,
      "modernApps": true,
      "resourceAccess": true,
      "deviceConfiguration": true,
      "compliancePolicy": true,
      "windowsUpdateForBusiness": true
    },
    "wiFiMacAddress": "Wi Fi Mac Address value",
    "deviceHealthAttestationState": {
      "@odata.type": "microsoft.graph.deviceHealthAttestationState",
      "lastUpdateDateTime": "Last Update Date Time value",
      "contentNamespaceUrl": "https://example.com/contentNamespaceUrl/",
      "deviceHealthAttestationStatus": "Device Health Attestation Status value",
      "contentVersion": "Content Version value",
      "issuedDateTime": "2016-12-31T23:58:22.1231038-08:00",
      "attestationIdentityKey": "Attestation Identity Key value",
      "resetCount": 10,
      "restartCount": 12,
      "dataExcutionPolicy": "Data Excution Policy value",
      "bitLockerStatus": "Bit Locker Status value",
      "bootManagerVersion": "Boot Manager Version value",
      "codeIntegrityCheckVersion": "Code Integrity Check Version value",
      "secureBoot": "Secure Boot value",
      "bootDebugging": "Boot Debugging value",
      "operatingSystemKernelDebugging": "Operating System Kernel Debugging value",
      "codeIntegrity": "Code Integrity value",
      "testSigning": "Test Signing value",
      "safeMode": "Safe Mode value",
      "windowsPE": "Windows PE value",
      "earlyLaunchAntiMalwareDriverProtection": "Early Launch Anti Malware Driver Protection value",
      "virtualSecureMode": "Virtual Secure Mode value",
      "pcrHashAlgorithm": "Pcr Hash Algorithm value",
      "bootAppSecurityVersion": "Boot App Security Version value",
      "bootManagerSecurityVersion": "Boot Manager Security Version value",
      "tpmVersion": "Tpm Version value",
      "pcr0": "Pcr0 value",
      "secureBootConfigurationPolicyFingerPrint": "Secure Boot Configuration Policy Finger Print value",
      "codeIntegrityPolicy": "Code Integrity Policy value",
      "bootRevisionListInfo": "Boot Revision List Info value",
      "operatingSystemRevListInfo": "Operating System Rev List Info value",
      "healthStatusMismatchInfo": "Health Status Mismatch Info value",
      "healthAttestationSupportedStatus": "Health Attestation Supported Status value"
    },
    "subscriberCarrier": "Subscriber Carrier value",
    "meid": "Meid value",
    "totalStorageSpaceInBytes": 8,
    "freeStorageSpaceInBytes": 7,
    "managedDeviceName": "Managed Device Name value",
    "partnerReportedThreatState": "activated",
    "usersLoggedOn": [
      {
        "@odata.type": "microsoft.graph.loggedOnUser",
        "userId": "User Id value",
        "lastLogOnDateTime": "2016-12-31T23:58:37.4262708-08:00"
      }
    ],
    "preferMdmOverGroupPolicyAppliedDateTime": "2016-12-31T23:57:34.4649887-08:00",
    "autopilotEnrolled": true,
    "requireUserEnrollmentApproval": true,
    "managementCertificateExpirationDate": "2016-12-31T23:57:59.9789653-08:00",
    "iccid": "Iccid value",
    "udid": "Udid value",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "windowsActiveMalwareCount": 9,
    "windowsRemediatedMalwareCount": 13,
    "notes": "Notes value",
    "configurationManagerClientHealthState": {
      "@odata.type": "microsoft.graph.configurationManagerClientHealthState",
      "state": "installed",
      "errorCode": 9,
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
    }
  }
}
```





