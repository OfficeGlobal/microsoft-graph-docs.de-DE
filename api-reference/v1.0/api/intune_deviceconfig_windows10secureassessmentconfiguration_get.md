# <a name="get-windows10secureassessmentconfiguration"></a><span data-ttu-id="1c5c5-101">windows10SecureAssessmentConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="1c5c5-101">Get windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="1c5c5-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1c5c5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1c5c5-103">Liest die Eigenschaften und Beziehungen von Objekten des Typs [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c5c5-103">Read properties and relationships of the [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1c5c5-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1c5c5-104">Prerequisites</span></span>
<span data-ttu-id="1c5c5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1c5c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1c5c5-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1c5c5-107">Permission type</span></span>|<span data-ttu-id="1c5c5-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1c5c5-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c5c5-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1c5c5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1c5c5-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c5c5-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1c5c5-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1c5c5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c5c5-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1c5c5-112">Not supported.</span></span>|
|<span data-ttu-id="1c5c5-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1c5c5-113">Application</span></span>|<span data-ttu-id="1c5c5-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1c5c5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c5c5-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1c5c5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1c5c5-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1c5c5-116">Optional query parameters</span></span>
<span data-ttu-id="1c5c5-117">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1c5c5-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1c5c5-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1c5c5-118">Request headers</span></span>
|<span data-ttu-id="1c5c5-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1c5c5-119">Header</span></span>|<span data-ttu-id="1c5c5-120">Wert</span><span class="sxs-lookup"><span data-stu-id="1c5c5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c5c5-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1c5c5-121">Authorization</span></span>|<span data-ttu-id="1c5c5-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1c5c5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c5c5-123">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="1c5c5-123">Accept</span></span>|<span data-ttu-id="1c5c5-124">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="1c5c5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c5c5-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1c5c5-125">Request body</span></span>
<span data-ttu-id="1c5c5-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1c5c5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c5c5-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="1c5c5-127">Response</span></span>
<span data-ttu-id="1c5c5-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1c5c5-128">If successful, this method returns a `200 OK` response code and [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c5c5-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1c5c5-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="1c5c5-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1c5c5-130">Request</span></span>
<span data-ttu-id="1c5c5-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1c5c5-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="1c5c5-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="1c5c5-132">Response</span></span>
<span data-ttu-id="1c5c5-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1c5c5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 574

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
    "id": "f60d71be-71be-f60d-be71-0df6be710df6",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "launchUri": "Launch Uri value",
    "configurationAccount": "Configuration Account value",
    "allowPrinting": true,
    "allowScreenCapture": true,
    "allowTextSuggestion": true
  }
}
```








