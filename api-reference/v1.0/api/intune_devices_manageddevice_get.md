# <a name="get-manageddevice"></a><span data-ttu-id="58cc6-101">managedDevice abrufen</span><span class="sxs-lookup"><span data-stu-id="58cc6-101">Get managedDevice</span></span>

> <span data-ttu-id="58cc6-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="58cc6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="58cc6-103">Lesen von Eigenschaften und Beziehungen des [managedDevice](../resources/intune_devices_manageddevice.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="58cc6-103">Read properties and relationships of the [managedDevice](../resources/intune_devices_manageddevice.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="58cc6-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="58cc6-104">Prerequisites</span></span>
<span data-ttu-id="58cc6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="58cc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="58cc6-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="58cc6-107">Permission type</span></span>|<span data-ttu-id="58cc6-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="58cc6-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58cc6-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="58cc6-109">Delegated (work or school account)</span></span>|<span data-ttu-id="58cc6-110">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="58cc6-110">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="58cc6-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="58cc6-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58cc6-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="58cc6-112">Not supported.</span></span>|
|<span data-ttu-id="58cc6-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="58cc6-113">Application</span></span>|<span data-ttu-id="58cc6-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="58cc6-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58cc6-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="58cc6-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/managedDevices/{managedDeviceId}
GET /deviceManagement/managedDevices/{managedDeviceId}
GET /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="58cc6-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="58cc6-116">Optional query parameters</span></span>
<span data-ttu-id="58cc6-117">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="58cc6-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="58cc6-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="58cc6-118">Request headers</span></span>
|<span data-ttu-id="58cc6-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="58cc6-119">Header</span></span>|<span data-ttu-id="58cc6-120">Wert</span><span class="sxs-lookup"><span data-stu-id="58cc6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58cc6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="58cc6-121">Authorization</span></span>|<span data-ttu-id="58cc6-122">Bearer &lt;token&gt;. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="58cc6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58cc6-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="58cc6-123">Accept</span></span>|<span data-ttu-id="58cc6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="58cc6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58cc6-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="58cc6-125">Request body</span></span>
<span data-ttu-id="58cc6-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="58cc6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58cc6-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="58cc6-127">Response</span></span>
<span data-ttu-id="58cc6-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [managedDevice](../resources/intune_devices_manageddevice.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="58cc6-128">If successful, this method returns a `200 OK` response code and [managedDevice](../resources/intune_devices_manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58cc6-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="58cc6-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="58cc6-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="58cc6-130">Request</span></span>
<span data-ttu-id="58cc6-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="58cc6-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}
```

### <a name="response"></a><span data-ttu-id="58cc6-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="58cc6-132">Response</span></span>
<span data-ttu-id="58cc6-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="58cc6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4920

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDevice",
    "id": "705c034c-034c-705c-4c03-5c704c035c70",
    "userId": "User Id value",
    "deviceName": "Device Name value",
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
    "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
    "operatingSystem": "Operating System value",
    "complianceState": "compliant",
    "jailBroken": "Jail Broken value",
    "managementAgent": "mdm",
    "osVersion": "Os Version value",
    "easActivated": true,
    "easDeviceId": "Eas Device Id value",
    "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
    "azureADRegistered": true,
    "deviceEnrollmentType": "userEnrollment",
    "activationLockBypassCode": "Activation Lock Bypass Code value",
    "emailAddress": "Email Address value",
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
    "partnerReportedThreatState": "activated"
  }
}
```



