# <a name="update-reportroot"></a><span data-ttu-id="fde0e-101">Aktualisieren von „reportRoot“</span><span class="sxs-lookup"><span data-stu-id="fde0e-101">Update reportRoot</span></span>

> <span data-ttu-id="fde0e-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fde0e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fde0e-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [reportRoot](../resources/intune_shared_reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="fde0e-103">Update the properties of a [reportRoot](../resources/intune_shared_reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fde0e-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fde0e-104">Prerequisites</span></span>
<span data-ttu-id="fde0e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fde0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fde0e-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fde0e-107">Permission type</span></span>|<span data-ttu-id="fde0e-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fde0e-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fde0e-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fde0e-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="fde0e-110">&nbsp; &nbsp; Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="fde0e-110">&nbsp; &nbsp;Device Configuration.</span></span> | <span data-ttu-id="fde0e-111">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fde0e-111">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="fde0e-112">&nbsp; &nbsp; Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="fde0e-112">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="fde0e-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fde0e-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fde0e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fde0e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fde0e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fde0e-115">Not supported.</span></span>|
|<span data-ttu-id="fde0e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fde0e-116">Application</span></span>|<span data-ttu-id="fde0e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fde0e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fde0e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fde0e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="fde0e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fde0e-119">Request headers</span></span>
|<span data-ttu-id="fde0e-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="fde0e-120">Header</span></span>|<span data-ttu-id="fde0e-121">Wert</span><span class="sxs-lookup"><span data-stu-id="fde0e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fde0e-122">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="fde0e-122">Authorization</span></span>|<span data-ttu-id="fde0e-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fde0e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fde0e-124">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="fde0e-124">Accept</span></span>|<span data-ttu-id="fde0e-125">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="fde0e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fde0e-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fde0e-126">Request body</span></span>
<span data-ttu-id="fde0e-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [reportRoot](../resources/intune_shared_reportroot.md) an.</span><span class="sxs-lookup"><span data-stu-id="fde0e-127">In the request body, supply a JSON representation for the [reportRoot](../resources/intune_shared_reportroot.md) object.</span></span>

<span data-ttu-id="fde0e-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [reportRoot](../resources/intune_shared_reportroot.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="fde0e-128">The following table shows the properties that are required when you create the [reportRoot](../resources/intune_shared_reportroot.md).</span></span>

|<span data-ttu-id="fde0e-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fde0e-129">Property</span></span>|<span data-ttu-id="fde0e-130">Typ</span><span class="sxs-lookup"><span data-stu-id="fde0e-130">Type</span></span>|<span data-ttu-id="fde0e-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fde0e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fde0e-132">ID</span><span class="sxs-lookup"><span data-stu-id="fde0e-132">id</span></span>|<span data-ttu-id="fde0e-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fde0e-133">String</span></span>|<span data-ttu-id="fde0e-134">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="fde0e-134">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="fde0e-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="fde0e-135">Response</span></span>
<span data-ttu-id="fde0e-136">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [reportRoot](../resources/intune_shared_reportroot.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="fde0e-136">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune_shared_reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fde0e-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fde0e-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="fde0e-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fde0e-138">Request</span></span>
<span data-ttu-id="fde0e-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fde0e-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="fde0e-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="fde0e-140">Response</span></span>
<span data-ttu-id="fde0e-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fde0e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```








