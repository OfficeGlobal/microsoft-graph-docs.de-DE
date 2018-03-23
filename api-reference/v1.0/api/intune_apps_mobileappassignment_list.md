# <a name="list-mobileappassignments"></a><span data-ttu-id="13d96-101">Auflisten von „mobileAppAssignment“</span><span class="sxs-lookup"><span data-stu-id="13d96-101">List mobileAppAssignments</span></span>

> <span data-ttu-id="13d96-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="13d96-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="13d96-103">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) auf.</span><span class="sxs-lookup"><span data-stu-id="13d96-103">List properties and relationships of the [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="13d96-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="13d96-104">Prerequisites</span></span>
<span data-ttu-id="13d96-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="13d96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="13d96-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="13d96-107">Permission type</span></span>|<span data-ttu-id="13d96-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="13d96-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13d96-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="13d96-109">Delegated (work or school account)</span></span>|<span data-ttu-id="13d96-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="13d96-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="13d96-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="13d96-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13d96-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="13d96-112">Not supported.</span></span>|
|<span data-ttu-id="13d96-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="13d96-113">Application</span></span>|<span data-ttu-id="13d96-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="13d96-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13d96-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="13d96-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="13d96-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="13d96-116">Request headers</span></span>
|<span data-ttu-id="13d96-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="13d96-117">Header</span></span>|<span data-ttu-id="13d96-118">Wert</span><span class="sxs-lookup"><span data-stu-id="13d96-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13d96-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="13d96-119">Authorization</span></span>|<span data-ttu-id="13d96-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="13d96-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="13d96-121">Accept</span><span class="sxs-lookup"><span data-stu-id="13d96-121">Accept</span></span>|<span data-ttu-id="13d96-122">application/json</span><span class="sxs-lookup"><span data-stu-id="13d96-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13d96-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="13d96-123">Request body</span></span>
<span data-ttu-id="13d96-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="13d96-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13d96-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="13d96-125">Response</span></span>
<span data-ttu-id="13d96-126">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="13d96-126">If successful, this method returns a `200 OK` response code and collection of [workbookPivotTable](../resources/intune_apps_mobileappassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13d96-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="13d96-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="13d96-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="13d96-128">Request</span></span>
<span data-ttu-id="13d96-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="13d96-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

### <a name="response"></a><span data-ttu-id="13d96-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="13d96-130">Response</span></span>
<span data-ttu-id="13d96-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="13d96-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 391

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppAssignment",
      "id": "591620b7-20b7-5916-b720-1659b7201659",
      "intent": "required",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "settings": {
        "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
      }
    }
  ]
}
```



