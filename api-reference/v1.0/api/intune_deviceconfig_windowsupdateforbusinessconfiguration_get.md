# <a name="get-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="44851-101">Abrufen von „windowsUpdateForBusinessConfiguration“</span><span class="sxs-lookup"><span data-stu-id="44851-101">Get windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="44851-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="44851-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="44851-103">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="44851-103">Read properties and relationships of the [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="44851-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="44851-104">Prerequisites</span></span>
<span data-ttu-id="44851-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="44851-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="44851-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="44851-107">Permission type</span></span>|<span data-ttu-id="44851-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="44851-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44851-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="44851-109">Delegated (work or school account)</span></span>|<span data-ttu-id="44851-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="44851-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="44851-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="44851-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44851-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="44851-112">Not supported.</span></span>|
|<span data-ttu-id="44851-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="44851-113">Application</span></span>|<span data-ttu-id="44851-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="44851-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44851-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="44851-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="44851-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="44851-116">Optional query parameters</span></span>
<span data-ttu-id="44851-117">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="44851-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="44851-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="44851-118">Request headers</span></span>
|<span data-ttu-id="44851-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="44851-119">Header</span></span>|<span data-ttu-id="44851-120">Wert</span><span class="sxs-lookup"><span data-stu-id="44851-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44851-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="44851-121">Authorization</span></span>|<span data-ttu-id="44851-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="44851-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44851-123">Accept</span><span class="sxs-lookup"><span data-stu-id="44851-123">Accept</span></span>|<span data-ttu-id="44851-124">application/json</span><span class="sxs-lookup"><span data-stu-id="44851-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44851-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="44851-125">Request body</span></span>
<span data-ttu-id="44851-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="44851-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44851-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="44851-127">Response</span></span>
<span data-ttu-id="44851-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="44851-128">If successful, this method returns a `200 OK` response code and [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44851-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="44851-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="44851-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="44851-130">Request</span></span>
<span data-ttu-id="44851-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="44851-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="44851-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="44851-132">Response</span></span>
<span data-ttu-id="44851-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="44851-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1149

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
    "id": "4928dd6a-dd6a-4928-6add-28496add2849",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "deliveryOptimizationMode": "httpOnly",
    "prereleaseFeatures": "settingsOnly",
    "automaticUpdateMode": "notifyDownload",
    "microsoftUpdateServiceAllowed": true,
    "driversExcluded": true,
    "installationSchedule": {
      "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
      "scheduledInstallDay": "everyday",
      "scheduledInstallTime": "11:59:31.3170000"
    },
    "qualityUpdatesDeferralPeriodInDays": 2,
    "featureUpdatesDeferralPeriodInDays": 2,
    "qualityUpdatesPaused": true,
    "featureUpdatesPaused": true,
    "qualityUpdatesPauseExpiryDateTime": "2017-01-01T00:00:22.9594683-08:00",
    "featureUpdatesPauseExpiryDateTime": "2016-12-31T23:58:08.068669-08:00",
    "businessReadyUpdatesOnly": "all"
  }
}
```



