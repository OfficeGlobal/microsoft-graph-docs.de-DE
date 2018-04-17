# <a name="update-devicemanagement"></a><span data-ttu-id="bf3dc-101">Aktualisieren von „deviceManagement“</span><span class="sxs-lookup"><span data-stu-id="bf3dc-101">Update deviceManagement</span></span>

> <span data-ttu-id="bf3dc-102">**Wichtig:** Die APIs der /beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bf3dc-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf3dc-103">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bf3dc-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bf3dc-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bf3dc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bf3dc-105">Aktualisieren der Eigenschaften eines [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="bf3dc-105">Update the properties of a [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bf3dc-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bf3dc-106">Prerequisites</span></span>
<span data-ttu-id="bf3dc-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bf3dc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bf3dc-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bf3dc-109">Permission type</span></span>|<span data-ttu-id="bf3dc-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bf3dc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf3dc-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bf3dc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bf3dc-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf3dc-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="bf3dc-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bf3dc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf3dc-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bf3dc-114">Not supported.</span></span>|
|<span data-ttu-id="bf3dc-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bf3dc-115">Application</span></span>|<span data-ttu-id="bf3dc-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bf3dc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf3dc-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bf3dc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="bf3dc-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bf3dc-118">Request headers</span></span>
|<span data-ttu-id="bf3dc-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bf3dc-119">Header</span></span>|<span data-ttu-id="bf3dc-120">Wert</span><span class="sxs-lookup"><span data-stu-id="bf3dc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf3dc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf3dc-121">Authorization</span></span>|<span data-ttu-id="bf3dc-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bf3dc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf3dc-123">Accept</span><span class="sxs-lookup"><span data-stu-id="bf3dc-123">Accept</span></span>|<span data-ttu-id="bf3dc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bf3dc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf3dc-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bf3dc-125">Request body</span></span>
<span data-ttu-id="bf3dc-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) an.</span><span class="sxs-lookup"><span data-stu-id="bf3dc-126">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) object.</span></span>

<span data-ttu-id="bf3dc-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="bf3dc-127">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md).</span></span>

|<span data-ttu-id="bf3dc-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bf3dc-128">Property</span></span>|<span data-ttu-id="bf3dc-129">Typ</span><span class="sxs-lookup"><span data-stu-id="bf3dc-129">Type</span></span>|<span data-ttu-id="bf3dc-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bf3dc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf3dc-131">id</span><span class="sxs-lookup"><span data-stu-id="bf3dc-131">id</span></span>|<span data-ttu-id="bf3dc-132">String</span><span class="sxs-lookup"><span data-stu-id="bf3dc-132">String</span></span>|<span data-ttu-id="bf3dc-133">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="bf3dc-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="bf3dc-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="bf3dc-134">Response</span></span>
<span data-ttu-id="bf3dc-135">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="bf3dc-135">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf3dc-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bf3dc-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="bf3dc-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bf3dc-137">Request</span></span>
<span data-ttu-id="bf3dc-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bf3dc-138">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="bf3dc-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="bf3dc-139">Response</span></span>
<span data-ttu-id="bf3dc-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bf3dc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "0b283420-3420-0b28-2034-280b2034280b"
}
```



