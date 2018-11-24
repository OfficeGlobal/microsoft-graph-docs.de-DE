# <a name="list-androidmanagedappprotections"></a><span data-ttu-id="0254e-101">Auflisten von „androidManagedAppProtection“</span><span class="sxs-lookup"><span data-stu-id="0254e-101">List androidManagedAppProtections</span></span>

> <span data-ttu-id="0254e-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0254e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0254e-103">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md) auf.</span><span class="sxs-lookup"><span data-stu-id="0254e-103">List properties and relationships of the [androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0254e-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0254e-104">Prerequisites</span></span>
<span data-ttu-id="0254e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0254e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0254e-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0254e-107">Permission type</span></span>|<span data-ttu-id="0254e-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0254e-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0254e-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0254e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0254e-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0254e-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0254e-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0254e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0254e-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0254e-112">Not supported.</span></span>|
|<span data-ttu-id="0254e-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0254e-113">Application</span></span>|<span data-ttu-id="0254e-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0254e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0254e-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0254e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/androidManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="0254e-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0254e-116">Request headers</span></span>
|<span data-ttu-id="0254e-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0254e-117">Header</span></span>|<span data-ttu-id="0254e-118">Wert</span><span class="sxs-lookup"><span data-stu-id="0254e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0254e-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="0254e-119">Authorization</span></span>|<span data-ttu-id="0254e-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0254e-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0254e-121">Accept</span><span class="sxs-lookup"><span data-stu-id="0254e-121">Accept</span></span>|<span data-ttu-id="0254e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="0254e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0254e-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0254e-123">Request body</span></span>
<span data-ttu-id="0254e-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0254e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0254e-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="0254e-125">Response</span></span>
<span data-ttu-id="0254e-126">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0254e-126">If successful, this method returns a `200 OK` response code and a collection of [androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0254e-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0254e-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="0254e-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0254e-128">Request</span></span>
<span data-ttu-id="0254e-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0254e-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/androidManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="0254e-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="0254e-130">Response</span></span>
<span data-ttu-id="0254e-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0254e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2065

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidManagedAppProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "cf517ced-7ced-cf51-ed7c-51cfed7c51cf",
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
      "isAssigned": true,
      "screenCaptureBlocked": true,
      "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
      "encryptAppData": true,
      "deployedAppCount": 0,
      "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
      "minimumWarningPatchVersion": "Minimum Warning Patch Version value"
    }
  ]
}
```



