# <a name="get-iosdevicefeaturesconfiguration"></a><span data-ttu-id="711a2-101">Abrufen von „iosDeviceFeaturesConfiguration“</span><span class="sxs-lookup"><span data-stu-id="711a2-101">Get iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="711a2-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="711a2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="711a2-103">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="711a2-103">Read properties and relationships of [plannerTaskDetails](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="711a2-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="711a2-104">Prerequisites</span></span>
<span data-ttu-id="711a2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="711a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="711a2-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="711a2-107">Permission type</span></span>|<span data-ttu-id="711a2-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="711a2-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="711a2-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="711a2-109">Delegated (work or school account)</span></span>|<span data-ttu-id="711a2-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="711a2-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="711a2-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="711a2-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="711a2-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="711a2-112">Not supported.</span></span>|
|<span data-ttu-id="711a2-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="711a2-113">Application</span></span>|<span data-ttu-id="711a2-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="711a2-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="711a2-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="711a2-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="711a2-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="711a2-116">Optional query parameters</span></span>
<span data-ttu-id="711a2-117">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="711a2-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="711a2-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="711a2-118">Request headers</span></span>
|<span data-ttu-id="711a2-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="711a2-119">Header</span></span>|<span data-ttu-id="711a2-120">Wert</span><span class="sxs-lookup"><span data-stu-id="711a2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="711a2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="711a2-121">Authorization</span></span>|<span data-ttu-id="711a2-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="711a2-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="711a2-123">Accept</span><span class="sxs-lookup"><span data-stu-id="711a2-123">Accept</span></span>|<span data-ttu-id="711a2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="711a2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="711a2-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="711a2-125">Request body</span></span>
<span data-ttu-id="711a2-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="711a2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="711a2-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="711a2-127">Response</span></span>
<span data-ttu-id="711a2-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="711a2-128">If successful, this method returns a `200 OK` response code and a [section](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="711a2-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="711a2-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="711a2-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="711a2-130">Request</span></span>
<span data-ttu-id="711a2-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="711a2-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="711a2-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="711a2-132">Response</span></span>
<span data-ttu-id="711a2-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="711a2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2313

{
  "value": {
    "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
    "id": "651e0ab3-0ab3-651e-b30a-1e65b30a1e65",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "assetTagTemplate": "Asset Tag Template value",
    "lockScreenFootnote": "Lock Screen Footnote value",
    "homeScreenDockIcons": [
      {
        "@odata.type": "microsoft.graph.iosHomeScreenFolder",
        "displayName": "Display Name value",
        "pages": [
          {
            "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
            "displayName": "Display Name value",
            "apps": [
              {
                "@odata.type": "microsoft.graph.iosHomeScreenApp",
                "displayName": "Display Name value",
                "bundleID": "Bundle ID value"
              }
            ]
          }
        ]
      }
    ],
    "homeScreenPages": [
      {
        "@odata.type": "microsoft.graph.iosHomeScreenPage",
        "displayName": "Display Name value",
        "icons": [
          {
            "@odata.type": "microsoft.graph.iosHomeScreenFolder",
            "displayName": "Display Name value",
            "pages": [
              {
                "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
                "displayName": "Display Name value",
                "apps": [
                  {
                    "@odata.type": "microsoft.graph.iosHomeScreenApp",
                    "displayName": "Display Name value",
                    "bundleID": "Bundle ID value"
                  }
                ]
              }
            ]
          }
        ]
      }
    ],
    "notificationSettings": [
      {
        "@odata.type": "microsoft.graph.iosNotificationSettings",
        "bundleID": "Bundle ID value",
        "appName": "App Name value",
        "publisher": "Publisher value",
        "enabled": true,
        "showInNotificationCenter": true,
        "showOnLockScreen": true,
        "alertType": "banner",
        "badgesEnabled": true,
        "soundsEnabled": true
      }
    ]
  }
}
```



