# <a name="list-auditevents"></a><span data-ttu-id="ef969-101">Auflisten von „auditEvent“</span><span class="sxs-lookup"><span data-stu-id="ef969-101">List auditEvents</span></span>

> <span data-ttu-id="ef969-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ef969-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ef969-103">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [auditEvent](../resources/intune_auditing_auditevent.md) auf.</span><span class="sxs-lookup"><span data-stu-id="ef969-103">List properties and relationships of the [auditEvent](../resources/intune_auditing_auditevent.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ef969-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ef969-104">Prerequisites</span></span>
<span data-ttu-id="ef969-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ef969-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ef969-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ef969-107">Permission type</span></span>|<span data-ttu-id="ef969-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ef969-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef969-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ef969-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ef969-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef969-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ef969-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ef969-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef969-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ef969-112">Not supported.</span></span>|
|<span data-ttu-id="ef969-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ef969-113">Application</span></span>|<span data-ttu-id="ef969-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ef969-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef969-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ef969-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="ef969-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ef969-116">Request headers</span></span>
|<span data-ttu-id="ef969-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ef969-117">Header</span></span>|<span data-ttu-id="ef969-118">Wert</span><span class="sxs-lookup"><span data-stu-id="ef969-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef969-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef969-119">Authorization</span></span>|<span data-ttu-id="ef969-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ef969-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef969-121">Accept</span><span class="sxs-lookup"><span data-stu-id="ef969-121">Accept</span></span>|<span data-ttu-id="ef969-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ef969-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef969-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ef969-123">Request body</span></span>
<span data-ttu-id="ef969-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ef969-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef969-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="ef969-125">Response</span></span>
<span data-ttu-id="ef969-126">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [auditEvent](../resources/intune_auditing_auditevent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ef969-126">If successful, this method returns a `200 OK` response code and a collection of [auditEvent](../resources/intune_auditing_auditevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef969-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ef969-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="ef969-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ef969-128">Request</span></span>
<span data-ttu-id="ef969-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ef969-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents
```

### <a name="response"></a><span data-ttu-id="ef969-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="ef969-130">Response</span></span>
<span data-ttu-id="ef969-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ef969-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1632

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.auditEvent",
      "id": "59653ce8-3ce8-5965-e83c-6559e83c6559",
      "displayName": "Display Name value",
      "componentName": "Component Name value",
      "actor": {
        "@odata.type": "microsoft.graph.auditActor",
        "type": "Type value",
        "userPermissions": [
          "User Permissions value"
        ],
        "applicationId": "Application Id value",
        "applicationDisplayName": "Application Display Name value",
        "userPrincipalName": "User Principal Name value",
        "servicePrincipalName": "Service Principal Name value",
        "ipAddress": "Ip Address value",
        "userId": "User Id value"
      },
      "activity": "Activity value",
      "activityDateTime": "2016-12-31T23:59:51.6363086-08:00",
      "activityType": "Activity Type value",
      "activityOperationType": "Activity Operation Type value",
      "activityResult": "Activity Result value",
      "correlationId": "52effe71-fe71-52ef-71fe-ef5271feef52",
      "resources": [
        {
          "@odata.type": "microsoft.graph.auditResource",
          "displayName": "Display Name value",
          "modifiedProperties": [
            {
              "@odata.type": "microsoft.graph.auditProperty",
              "displayName": "Display Name value",
              "oldValue": "Old Value value",
              "newValue": "New Value value"
            }
          ],
          "type": "Type value",
          "resourceId": "Resource Id value"
        }
      ],
      "category": "Category value"
    }
  ]
}
```



