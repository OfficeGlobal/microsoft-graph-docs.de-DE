# <a name="scheduleactionsforrules-action"></a><span data-ttu-id="f1864-101">scheduleActionsForRules-Aktion</span><span class="sxs-lookup"><span data-stu-id="f1864-101">scheduleActionsForRules action</span></span>

> <span data-ttu-id="f1864-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f1864-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1864-103">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="f1864-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f1864-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f1864-104">Prerequisites</span></span>
<span data-ttu-id="f1864-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f1864-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f1864-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f1864-107">Permission type</span></span>|<span data-ttu-id="f1864-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f1864-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1864-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f1864-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f1864-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1864-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f1864-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f1864-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1864-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f1864-112">Not supported.</span></span>|
|<span data-ttu-id="f1864-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f1864-113">Application</span></span>|<span data-ttu-id="f1864-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f1864-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1864-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f1864-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduleActionsForRules
```

## <a name="request-headers"></a><span data-ttu-id="f1864-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f1864-116">Request headers</span></span>
|<span data-ttu-id="f1864-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f1864-117">Header</span></span>|<span data-ttu-id="f1864-118">Wert</span><span class="sxs-lookup"><span data-stu-id="f1864-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1864-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1864-119">Authorization</span></span>|<span data-ttu-id="f1864-120">Bearer &lt;token&gt;. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f1864-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1864-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f1864-121">Accept</span></span>|<span data-ttu-id="f1864-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f1864-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1864-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f1864-123">Request body</span></span>
<span data-ttu-id="f1864-124">Geben Sie im Anforderungstext eine JSON-Darstellung des Parameters an.</span><span class="sxs-lookup"><span data-stu-id="f1864-124">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f1864-125">Die folgende Tabelle zeigt die Parameter, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="f1864-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f1864-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f1864-126">Property</span></span>|<span data-ttu-id="f1864-127">Typ</span><span class="sxs-lookup"><span data-stu-id="f1864-127">Type</span></span>|<span data-ttu-id="f1864-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f1864-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1864-129">deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="f1864-129">deviceComplianceScheduledActionForRules</span></span>|<span data-ttu-id="f1864-130">Sammlung von Objekten des Typs [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md)</span><span class="sxs-lookup"><span data-stu-id="f1864-130">[deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="f1864-131">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="f1864-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f1864-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="f1864-132">Response</span></span>
<span data-ttu-id="f1864-133">Wenn die Aktion erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f1864-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f1864-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f1864-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="f1864-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f1864-135">Request</span></span>
<span data-ttu-id="f1864-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f1864-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduleActionsForRules

Content-type: application/json
Content-length: 242

{
  "deviceComplianceScheduledActionForRules": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
      "id": "f0075d5e-5d5e-f007-5e5d-07f05e5d07f0",
      "ruleName": "Rule Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="f1864-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="f1864-137">Response</span></span>
<span data-ttu-id="f1864-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f1864-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



