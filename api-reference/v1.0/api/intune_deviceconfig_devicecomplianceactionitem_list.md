# <a name="list-devicecomplianceactionitems"></a><span data-ttu-id="aa3d0-101">Auflisten von „deviceComplianceActionItem“</span><span class="sxs-lookup"><span data-stu-id="aa3d0-101">List deviceComplianceActionItems</span></span>

> <span data-ttu-id="aa3d0-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="aa3d0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aa3d0-103">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) auf.</span><span class="sxs-lookup"><span data-stu-id="aa3d0-103">List properties and relationships of the [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aa3d0-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="aa3d0-104">Prerequisites</span></span>
<span data-ttu-id="aa3d0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="aa3d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="aa3d0-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="aa3d0-107">Permission type</span></span>|<span data-ttu-id="aa3d0-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="aa3d0-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa3d0-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="aa3d0-109">Delegated (work or school account)</span></span>|<span data-ttu-id="aa3d0-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="aa3d0-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="aa3d0-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="aa3d0-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa3d0-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aa3d0-112">Not supported.</span></span>|
|<span data-ttu-id="aa3d0-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="aa3d0-113">Application</span></span>|<span data-ttu-id="aa3d0-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aa3d0-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa3d0-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aa3d0-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="aa3d0-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="aa3d0-116">Request headers</span></span>
|<span data-ttu-id="aa3d0-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="aa3d0-117">Header</span></span>|<span data-ttu-id="aa3d0-118">Wert</span><span class="sxs-lookup"><span data-stu-id="aa3d0-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa3d0-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa3d0-119">Authorization</span></span>|<span data-ttu-id="aa3d0-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="aa3d0-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="aa3d0-121">Accept</span><span class="sxs-lookup"><span data-stu-id="aa3d0-121">Accept</span></span>|<span data-ttu-id="aa3d0-122">application/json</span><span class="sxs-lookup"><span data-stu-id="aa3d0-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa3d0-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="aa3d0-123">Request body</span></span>
<span data-ttu-id="aa3d0-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="aa3d0-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa3d0-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="aa3d0-125">Response</span></span>
<span data-ttu-id="aa3d0-126">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="aa3d0-126">If successful, this method returns a `200 OK` response code and collection of [workbookRangeView](../resources/intune_deviceconfig_devicecomplianceactionitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa3d0-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="aa3d0-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="aa3d0-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aa3d0-128">Request</span></span>
<span data-ttu-id="aa3d0-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="aa3d0-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

### <a name="response"></a><span data-ttu-id="aa3d0-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="aa3d0-130">Response</span></span>
<span data-ttu-id="aa3d0-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aa3d0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 385

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
      "id": "e01a1893-1893-e01a-9318-1ae093181ae0",
      "gracePeriodHours": 0,
      "actionType": "notification",
      "notificationTemplateId": "Notification Template Id value",
      "notificationMessageCCList": [
        "Notification Message CCList value"
      ]
    }
  ]
}
```



