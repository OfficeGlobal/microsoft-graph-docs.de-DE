# <a name="get-iosmanagedappprotection"></a><span data-ttu-id="3ab91-101">Abrufen von „iosManagedAppProtection“</span><span class="sxs-lookup"><span data-stu-id="3ab91-101">Get iosManagedAppProtection</span></span>

> <span data-ttu-id="3ab91-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3ab91-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3ab91-103">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="3ab91-103">Read properties and relationships of the [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3ab91-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3ab91-104">Prerequisites</span></span>
<span data-ttu-id="3ab91-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3ab91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3ab91-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3ab91-107">Permission type</span></span>|<span data-ttu-id="3ab91-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3ab91-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ab91-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3ab91-109">Delegated (work or school account)</span></span>|<span data-ttu-id="3ab91-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ab91-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3ab91-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3ab91-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ab91-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3ab91-112">Not supported.</span></span>|
|<span data-ttu-id="3ab91-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3ab91-113">Application</span></span>|<span data-ttu-id="3ab91-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3ab91-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ab91-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3ab91-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3ab91-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3ab91-116">Optional query parameters</span></span>
<span data-ttu-id="3ab91-117">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3ab91-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3ab91-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3ab91-118">Request headers</span></span>
|<span data-ttu-id="3ab91-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3ab91-119">Header</span></span>|<span data-ttu-id="3ab91-120">Wert</span><span class="sxs-lookup"><span data-stu-id="3ab91-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ab91-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="3ab91-121">Authorization</span></span>|<span data-ttu-id="3ab91-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3ab91-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ab91-123">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="3ab91-123">Accept</span></span>|<span data-ttu-id="3ab91-124">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="3ab91-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ab91-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3ab91-125">Request body</span></span>
<span data-ttu-id="3ab91-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3ab91-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ab91-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="3ab91-127">Response</span></span>
<span data-ttu-id="3ab91-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3ab91-128">If successful, this method returns a `200 OK` response code and [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ab91-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3ab91-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="3ab91-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3ab91-130">Request</span></span>
<span data-ttu-id="3ab91-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3ab91-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="3ab91-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="3ab91-132">Response</span></span>
<span data-ttu-id="3ab91-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3ab91-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1839

{
  "value": {
    "@odata.type": "#microsoft.graph.iosManagedAppProtection",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "id": "5bc789cb-89cb-5bc7-cb89-c75bcb89c75b",
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
    "appDataEncryptionType": "afterDeviceRestart",
    "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
    "deployedAppCount": 0,
    "faceIdBlocked": true
  }
}
```








