# <a name="assign-action"></a><span data-ttu-id="4fcdf-101">Aktion „assign“</span><span class="sxs-lookup"><span data-stu-id="4fcdf-101">assign action</span></span>

> <span data-ttu-id="4fcdf-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4fcdf-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4fcdf-103">Diese Aktion ist noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="4fcdf-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4fcdf-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4fcdf-104">Prerequisites</span></span>
<span data-ttu-id="4fcdf-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4fcdf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4fcdf-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4fcdf-107">Permission type</span></span>|<span data-ttu-id="4fcdf-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4fcdf-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4fcdf-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4fcdf-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4fcdf-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fcdf-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4fcdf-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4fcdf-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4fcdf-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4fcdf-112">Not supported.</span></span>|
|<span data-ttu-id="4fcdf-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4fcdf-113">Application</span></span>|<span data-ttu-id="4fcdf-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4fcdf-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4fcdf-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4fcdf-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="4fcdf-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4fcdf-116">Request headers</span></span>
|<span data-ttu-id="4fcdf-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4fcdf-117">Header</span></span>|<span data-ttu-id="4fcdf-118">Wert</span><span class="sxs-lookup"><span data-stu-id="4fcdf-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4fcdf-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="4fcdf-119">Authorization</span></span>|<span data-ttu-id="4fcdf-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4fcdf-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4fcdf-121">Accept</span><span class="sxs-lookup"><span data-stu-id="4fcdf-121">Accept</span></span>|<span data-ttu-id="4fcdf-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4fcdf-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fcdf-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4fcdf-123">Request body</span></span>
<span data-ttu-id="4fcdf-124">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="4fcdf-124">In the request body, supply a JSON representation of the Contact object.</span></span>

<span data-ttu-id="4fcdf-125">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="4fcdf-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4fcdf-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4fcdf-126">Property</span></span>|<span data-ttu-id="4fcdf-127">Typ</span><span class="sxs-lookup"><span data-stu-id="4fcdf-127">Type</span></span>|<span data-ttu-id="4fcdf-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4fcdf-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fcdf-129">assignments</span><span class="sxs-lookup"><span data-stu-id="4fcdf-129">assignments</span></span>|<span data-ttu-id="4fcdf-130">Collection von Objekten des Typs [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="4fcdf-130">[deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="4fcdf-131">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="4fcdf-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4fcdf-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="4fcdf-132">Response</span></span>
<span data-ttu-id="4fcdf-133">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4fcdf-133">If successful, this method returns a `200 OK` response code and collection of [workbookRangeView](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fcdf-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4fcdf-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="4fcdf-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4fcdf-135">Request</span></span>
<span data-ttu-id="4fcdf-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4fcdf-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign

Content-type: application/json
Content-length: 280

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
      "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="4fcdf-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="4fcdf-137">Response</span></span>
<span data-ttu-id="4fcdf-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4fcdf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 274

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
      "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```



