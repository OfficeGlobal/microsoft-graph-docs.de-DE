# <a name="update-devicemanagement"></a><span data-ttu-id="43377-101">Aktualisieren von „deviceManagement“</span><span class="sxs-lookup"><span data-stu-id="43377-101">Update deviceManagement</span></span>

> <span data-ttu-id="43377-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="43377-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="43377-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceManagement](../resources/intune_deviceconfig_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="43377-103">Update the properties of a [calendar](../resources/intune_deviceconfig_devicemanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="43377-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="43377-104">Prerequisites</span></span>
<span data-ttu-id="43377-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="43377-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="43377-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="43377-107">Permission type</span></span>|<span data-ttu-id="43377-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="43377-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43377-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="43377-109">Delegated (work or school account)</span></span>|<span data-ttu-id="43377-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43377-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="43377-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="43377-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43377-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="43377-112">Not supported.</span></span>|
|<span data-ttu-id="43377-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="43377-113">Application</span></span>|<span data-ttu-id="43377-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="43377-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43377-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="43377-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="43377-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="43377-116">Request headers</span></span>
|<span data-ttu-id="43377-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="43377-117">Header</span></span>|<span data-ttu-id="43377-118">Wert</span><span class="sxs-lookup"><span data-stu-id="43377-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43377-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="43377-119">Authorization</span></span>|<span data-ttu-id="43377-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="43377-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="43377-121">Accept</span><span class="sxs-lookup"><span data-stu-id="43377-121">Accept</span></span>|<span data-ttu-id="43377-122">application/json</span><span class="sxs-lookup"><span data-stu-id="43377-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43377-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="43377-123">Request body</span></span>
<span data-ttu-id="43377-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceManagement](../resources/intune_deviceconfig_devicemanagement.md) an.</span><span class="sxs-lookup"><span data-stu-id="43377-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_devicemanagement.md) object.</span></span>

<span data-ttu-id="43377-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceManagement](../resources/intune_deviceconfig_devicemanagement.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="43377-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="43377-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="43377-126">Property</span></span>|<span data-ttu-id="43377-127">Typ</span><span class="sxs-lookup"><span data-stu-id="43377-127">Type</span></span>|<span data-ttu-id="43377-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="43377-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43377-129">id</span><span class="sxs-lookup"><span data-stu-id="43377-129">id</span></span>|<span data-ttu-id="43377-130">String</span><span class="sxs-lookup"><span data-stu-id="43377-130">String</span></span>|<span data-ttu-id="43377-131">Eindeutiger Bezeichner</span><span class="sxs-lookup"><span data-stu-id="43377-131">Unique Identifier</span></span>|
|<span data-ttu-id="43377-132">settings</span><span class="sxs-lookup"><span data-stu-id="43377-132">settings</span></span>|[<span data-ttu-id="43377-133">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="43377-133">deviceManagementSettings</span></span>](../resources/intune_deviceconfig_devicemanagementsettings.md)|<span data-ttu-id="43377-134">Einstellungen auf Kontoebene</span><span class="sxs-lookup"><span data-stu-id="43377-134">Account level settings.</span></span>|



## <a name="response"></a><span data-ttu-id="43377-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="43377-135">Response</span></span>
<span data-ttu-id="43377-136">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceManagement](../resources/intune_deviceconfig_devicemanagement.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="43377-136">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43377-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="43377-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="43377-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="43377-138">Request</span></span>
<span data-ttu-id="43377-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="43377-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement
Content-type: application/json
Content-length: 206

{
  "settings": {
    "@odata.type": "microsoft.graph.deviceManagementSettings",
    "deviceComplianceCheckinThresholdDays": 4,
    "isScheduledActionEnabled": true,
    "secureByDefault": true
  }
}
```

### <a name="response"></a><span data-ttu-id="43377-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="43377-140">Response</span></span>
<span data-ttu-id="43377-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="43377-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 310

{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "0b283420-3420-0b28-2034-280b2034280b",
  "settings": {
    "@odata.type": "microsoft.graph.deviceManagementSettings",
    "deviceComplianceCheckinThresholdDays": 4,
    "isScheduledActionEnabled": true,
    "secureByDefault": true
  }
}
```



