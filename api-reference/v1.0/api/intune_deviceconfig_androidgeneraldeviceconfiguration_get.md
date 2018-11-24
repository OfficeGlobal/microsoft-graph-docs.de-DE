# <a name="get-androidgeneraldeviceconfiguration"></a><span data-ttu-id="095da-101">androidGeneralDeviceConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="095da-101">Get androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="095da-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="095da-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="095da-103">Lesen von Eigenschaften und Beziehungen des [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="095da-103">Read properties and relationships of the [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="095da-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="095da-104">Prerequisites</span></span>
<span data-ttu-id="095da-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="095da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="095da-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="095da-107">Permission type</span></span>|<span data-ttu-id="095da-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="095da-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="095da-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="095da-109">Delegated (work or school account)</span></span>|<span data-ttu-id="095da-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="095da-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="095da-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="095da-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="095da-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="095da-112">Not supported.</span></span>|
|<span data-ttu-id="095da-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="095da-113">Application</span></span>|<span data-ttu-id="095da-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="095da-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="095da-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="095da-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="095da-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="095da-116">Optional query parameters</span></span>
<span data-ttu-id="095da-117">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="095da-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="095da-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="095da-118">Request headers</span></span>
|<span data-ttu-id="095da-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="095da-119">Header</span></span>|<span data-ttu-id="095da-120">Wert</span><span class="sxs-lookup"><span data-stu-id="095da-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="095da-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="095da-121">Authorization</span></span>|<span data-ttu-id="095da-122">Bearer &lt;token&gt;. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="095da-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="095da-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="095da-123">Accept</span></span>|<span data-ttu-id="095da-124">application/json</span><span class="sxs-lookup"><span data-stu-id="095da-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="095da-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="095da-125">Request body</span></span>
<span data-ttu-id="095da-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="095da-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="095da-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="095da-127">Response</span></span>
<span data-ttu-id="095da-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="095da-128">If successful, this method returns a `200 OK` response code and [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="095da-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="095da-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="095da-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="095da-130">Request</span></span>
<span data-ttu-id="095da-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="095da-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="095da-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="095da-132">Response</span></span>
<span data-ttu-id="095da-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="095da-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3414

{
  "value": {
    "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
    "id": "9e00d534-d534-9e00-34d5-009e34d5009e",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "appsBlockClipboardSharing": true,
    "appsBlockCopyPaste": true,
    "appsBlockYouTube": true,
    "bluetoothBlocked": true,
    "cameraBlocked": true,
    "cellularBlockDataRoaming": true,
    "cellularBlockMessaging": true,
    "cellularBlockVoiceRoaming": true,
    "cellularBlockWiFiTethering": true,
    "compliantAppsList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "compliantAppListType": "appsInListCompliant",
    "diagnosticDataBlockSubmission": true,
    "locationServicesBlocked": true,
    "googleAccountBlockAutoSync": true,
    "googlePlayStoreBlocked": true,
    "kioskModeBlockSleepButton": true,
    "kioskModeBlockVolumeButtons": true,
    "kioskModeApps": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "nfcBlocked": true,
    "passwordBlockFingerprintUnlock": true,
    "passwordBlockTrustAgents": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordSignInFailureCountBeforeFactoryReset": 12,
    "passwordRequiredType": "alphabetic",
    "passwordRequired": true,
    "powerOffBlocked": true,
    "factoryResetBlocked": true,
    "screenCaptureBlocked": true,
    "deviceSharingAllowed": true,
    "storageBlockGoogleBackup": true,
    "storageBlockRemovableStorage": true,
    "storageRequireDeviceEncryption": true,
    "storageRequireRemovableStorageEncryption": true,
    "voiceAssistantBlocked": true,
    "voiceDialingBlocked": true,
    "webBrowserBlockPopups": true,
    "webBrowserBlockAutofill": true,
    "webBrowserBlockJavaScript": true,
    "webBrowserBlocked": true,
    "webBrowserCookieSettings": "blockAlways",
    "wiFiBlocked": true,
    "appsInstallAllowList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "appsLaunchBlockList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "appsHideList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "securityRequireVerifyApps": true
  }
}
```



