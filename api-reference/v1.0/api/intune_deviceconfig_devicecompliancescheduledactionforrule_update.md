# <a name="update-devicecompliancescheduledactionforrule"></a><span data-ttu-id="00963-101">Aktualisieren von „deviceComplianceScheduledActionForRule“</span><span class="sxs-lookup"><span data-stu-id="00963-101">Update deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="00963-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="00963-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="00963-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="00963-103">Update the properties of a [calendar](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="00963-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="00963-104">Prerequisites</span></span>
<span data-ttu-id="00963-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="00963-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="00963-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="00963-107">Permission type</span></span>|<span data-ttu-id="00963-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="00963-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00963-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="00963-109">Delegated (work or school account)</span></span>|<span data-ttu-id="00963-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00963-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="00963-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="00963-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00963-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="00963-112">Not supported.</span></span>|
|<span data-ttu-id="00963-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="00963-113">Application</span></span>|<span data-ttu-id="00963-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="00963-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="00963-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="00963-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="00963-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="00963-116">Request headers</span></span>
|<span data-ttu-id="00963-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="00963-117">Header</span></span>|<span data-ttu-id="00963-118">Wert</span><span class="sxs-lookup"><span data-stu-id="00963-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00963-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="00963-119">Authorization</span></span>|<span data-ttu-id="00963-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="00963-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="00963-121">Accept</span><span class="sxs-lookup"><span data-stu-id="00963-121">Accept</span></span>|<span data-ttu-id="00963-122">application/json</span><span class="sxs-lookup"><span data-stu-id="00963-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00963-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="00963-123">Request body</span></span>
<span data-ttu-id="00963-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) an.</span><span class="sxs-lookup"><span data-stu-id="00963-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) object.</span></span>

<span data-ttu-id="00963-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="00963-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="00963-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="00963-126">Property</span></span>|<span data-ttu-id="00963-127">Typ</span><span class="sxs-lookup"><span data-stu-id="00963-127">Type</span></span>|<span data-ttu-id="00963-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="00963-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00963-129">id</span><span class="sxs-lookup"><span data-stu-id="00963-129">id</span></span>|<span data-ttu-id="00963-130">String</span><span class="sxs-lookup"><span data-stu-id="00963-130">String</span></span>|<span data-ttu-id="00963-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="00963-131">Key of the setting.</span></span>|
|<span data-ttu-id="00963-132">ruleName</span><span class="sxs-lookup"><span data-stu-id="00963-132">ruleName</span></span>|<span data-ttu-id="00963-133">String</span><span class="sxs-lookup"><span data-stu-id="00963-133">String</span></span>|<span data-ttu-id="00963-134">Name der Regel, auf die die geplante Aktion angewendet wird</span><span class="sxs-lookup"><span data-stu-id="00963-134">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="00963-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="00963-135">Response</span></span>
<span data-ttu-id="00963-136">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="00963-136">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00963-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="00963-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="00963-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="00963-138">Request</span></span>
<span data-ttu-id="00963-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="00963-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
Content-type: application/json
Content-length: 37

{
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="00963-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="00963-140">Response</span></span>
<span data-ttu-id="00963-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="00963-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 163

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "id": "f0075d5e-5d5e-f007-5e5d-07f05e5d07f0",
  "ruleName": "Rule Name value"
}
```



