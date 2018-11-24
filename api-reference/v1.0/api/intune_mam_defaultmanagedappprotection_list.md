# <a name="list-defaultmanagedappprotections"></a><span data-ttu-id="81622-101">Auflisten von „defaultManagedAppProtection“</span><span class="sxs-lookup"><span data-stu-id="81622-101">List defaultManagedAppProtections</span></span>

> <span data-ttu-id="81622-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="81622-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81622-103">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md) auf.</span><span class="sxs-lookup"><span data-stu-id="81622-103">List properties and relationships of the [defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="81622-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="81622-104">Prerequisites</span></span>
<span data-ttu-id="81622-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="81622-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="81622-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="81622-107">Permission type</span></span>|<span data-ttu-id="81622-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="81622-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81622-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="81622-109">Delegated (work or school account)</span></span>|<span data-ttu-id="81622-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="81622-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="81622-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="81622-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81622-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="81622-112">Not supported.</span></span>|
|<span data-ttu-id="81622-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="81622-113">Application</span></span>|<span data-ttu-id="81622-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="81622-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81622-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="81622-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/defaultManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="81622-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="81622-116">Request headers</span></span>
|<span data-ttu-id="81622-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="81622-117">Header</span></span>|<span data-ttu-id="81622-118">Wert</span><span class="sxs-lookup"><span data-stu-id="81622-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81622-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="81622-119">Authorization</span></span>|<span data-ttu-id="81622-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="81622-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81622-121">Accept</span><span class="sxs-lookup"><span data-stu-id="81622-121">Accept</span></span>|<span data-ttu-id="81622-122">application/json</span><span class="sxs-lookup"><span data-stu-id="81622-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81622-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="81622-123">Request body</span></span>
<span data-ttu-id="81622-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="81622-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81622-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="81622-125">Response</span></span>
<span data-ttu-id="81622-126">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="81622-126">If successful, this method returns a `200 OK` response code and a collection of [defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81622-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="81622-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="81622-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="81622-128">Request</span></span>
<span data-ttu-id="81622-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="81622-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/defaultManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="81622-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="81622-130">Response</span></span>
<span data-ttu-id="81622-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="81622-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2380

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "77064c51-4c51-7706-514c-0677514c0677",
      "version": "Version value",
      "periodOfflineBeforeAccessCheck": "-PT17.1357909S",
      "periodOnlineBeforeAccessCheck": "PT35.0018757S",
      "allowedInboundDataTransferSources": "managedApps",
      "allowedOutboundDataTransferDestinations": "managedApps",
      "organizationalCredentialsRequired": true,
      "allowedOutboundClipboardSharingLevel": "managedAppsWithPasteIn",
      "dataBackupBlocked": true,
      "deviceComplianceRequired": true,
      "managedBrowserToOpenLinksRequired": true,
      "saveAsBlocked": true,
      "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
      "pinRequired": true,
      "maximumPinRetries": 1,
      "simplePinBlocked": true,
      "minimumPinLength": 0,
      "pinCharacterSet": "alphanumericAndSymbol",
      "periodBeforePinReset": "PT3M29.6631862S",
      "allowedDataStorageLocations": [
        "sharePoint"
      ],
      "contactSyncBlocked": true,
      "printBlocked": true,
      "fingerprintBlocked": true,
      "disableAppPinIfDevicePinIsSet": true,
      "minimumRequiredOsVersion": "Minimum Required Os Version value",
      "minimumWarningOsVersion": "Minimum Warning Os Version value",
      "minimumRequiredAppVersion": "Minimum Required App Version value",
      "minimumWarningAppVersion": "Minimum Warning App Version value",
      "appDataEncryptionType": "afterDeviceRestart",
      "screenCaptureBlocked": true,
      "encryptAppData": true,
      "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
      "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
      "customSettings": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "deployedAppCount": 0,
      "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
      "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
      "faceIdBlocked": true
    }
  ]
}
```



