# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="5d964-101">windowsInformationProtectionAppLearningSummary erstellen</span><span class="sxs-lookup"><span data-stu-id="5d964-101">Create windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="5d964-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5d964-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5d964-103">Erstellen eines neuen [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="5d964-103">Create a new [plannerBucket](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5d964-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5d964-104">Prerequisites</span></span>
<span data-ttu-id="5d964-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5d964-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5d964-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5d964-107">Permission type</span></span>|<span data-ttu-id="5d964-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5d964-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d964-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5d964-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5d964-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d964-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5d964-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5d964-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d964-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5d964-112">Not supported.</span></span>|
|<span data-ttu-id="5d964-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5d964-113">Application</span></span>|<span data-ttu-id="5d964-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5d964-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d964-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d964-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="5d964-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5d964-116">Request headers</span></span>
|<span data-ttu-id="5d964-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5d964-117">Header</span></span>|<span data-ttu-id="5d964-118">Wert</span><span class="sxs-lookup"><span data-stu-id="5d964-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d964-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d964-119">Authorization</span></span>|<span data-ttu-id="5d964-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5d964-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5d964-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5d964-121">Accept</span></span>|<span data-ttu-id="5d964-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5d964-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d964-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5d964-123">Request body</span></span>
<span data-ttu-id="5d964-124">Geben Sie im Anforderungstext eine JSON-Darstellung des windowsInformationProtectionAppLearningSummary-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="5d964-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="5d964-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsInformationProtectionAppLearningSummary erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="5d964-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="5d964-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5d964-126">Property</span></span>|<span data-ttu-id="5d964-127">Typ</span><span class="sxs-lookup"><span data-stu-id="5d964-127">Type</span></span>|<span data-ttu-id="5d964-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5d964-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d964-129">id</span><span class="sxs-lookup"><span data-stu-id="5d964-129">id</span></span>|<span data-ttu-id="5d964-130">String</span><span class="sxs-lookup"><span data-stu-id="5d964-130">String</span></span>|<span data-ttu-id="5d964-131">Eindeutiger Bezeichner für die WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="5d964-131">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="5d964-132">applicationName</span><span class="sxs-lookup"><span data-stu-id="5d964-132">applicationName</span></span>|<span data-ttu-id="5d964-133">String</span><span class="sxs-lookup"><span data-stu-id="5d964-133">String</span></span>|<span data-ttu-id="5d964-134">Name der Anwendung</span><span class="sxs-lookup"><span data-stu-id="5d964-134">Application Name</span></span>|
|<span data-ttu-id="5d964-135">applicationType</span><span class="sxs-lookup"><span data-stu-id="5d964-135">applicationType</span></span>|<span data-ttu-id="5d964-136">String</span><span class="sxs-lookup"><span data-stu-id="5d964-136">String</span></span>|<span data-ttu-id="5d964-137">Typ der Anwendung. Mögliche Werte sind: `universal`, `desktop`.</span><span class="sxs-lookup"><span data-stu-id="5d964-137">Application Type Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="5d964-138">deviceCount</span><span class="sxs-lookup"><span data-stu-id="5d964-138">deviceCount</span></span>|<span data-ttu-id="5d964-139">Int32</span><span class="sxs-lookup"><span data-stu-id="5d964-139">Int32</span></span>|<span data-ttu-id="5d964-140">Geräteanzahl</span><span class="sxs-lookup"><span data-stu-id="5d964-140">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="5d964-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d964-141">Response</span></span>
<span data-ttu-id="5d964-142">Wenn erfolgreich, gibt diese Methode den `201 Created`-Antwortcode und das [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5d964-142">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d964-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5d964-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="5d964-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d964-144">Request</span></span>
<span data-ttu-id="5d964-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5d964-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionAppLearningSummaries
Content-type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="5d964-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d964-146">Response</span></span>
<span data-ttu-id="5d964-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5d964-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 240

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "id": "063baf50-af50-063b-50af-3b0650af3b06",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```



