# <a name="update-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="be795-101">windowsInformationProtectionAppLearningSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="be795-101">Update windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="be795-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="be795-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be795-103">Aktualisieren der Eigenschaften eines [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="be795-103">Update the properties of a [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="be795-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="be795-104">Prerequisites</span></span>
<span data-ttu-id="be795-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="be795-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="be795-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="be795-107">Permission type</span></span>|<span data-ttu-id="be795-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="be795-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be795-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="be795-109">Delegated (work or school account)</span></span>|<span data-ttu-id="be795-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be795-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="be795-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="be795-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be795-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="be795-112">Not supported.</span></span>|
|<span data-ttu-id="be795-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="be795-113">Application</span></span>|<span data-ttu-id="be795-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="be795-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be795-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="be795-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="be795-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="be795-116">Request headers</span></span>
|<span data-ttu-id="be795-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="be795-117">Header</span></span>|<span data-ttu-id="be795-118">Wert</span><span class="sxs-lookup"><span data-stu-id="be795-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be795-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="be795-119">Authorization</span></span>|<span data-ttu-id="be795-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="be795-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be795-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="be795-121">Accept</span></span>|<span data-ttu-id="be795-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="be795-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be795-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="be795-123">Request body</span></span>
<span data-ttu-id="be795-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="be795-124">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) object.</span></span>

<span data-ttu-id="be795-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="be795-125">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md).</span></span>

|<span data-ttu-id="be795-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="be795-126">Property</span></span>|<span data-ttu-id="be795-127">Typ</span><span class="sxs-lookup"><span data-stu-id="be795-127">Type</span></span>|<span data-ttu-id="be795-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="be795-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be795-129">ID</span><span class="sxs-lookup"><span data-stu-id="be795-129">id</span></span>|<span data-ttu-id="be795-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="be795-130">String</span></span>|<span data-ttu-id="be795-131">Eindeutiger Bezeichner für die WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="be795-131">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="be795-132">applicationName</span><span class="sxs-lookup"><span data-stu-id="be795-132">applicationName</span></span>|<span data-ttu-id="be795-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="be795-133">String</span></span>|<span data-ttu-id="be795-134">Name der Anwendung</span><span class="sxs-lookup"><span data-stu-id="be795-134">Application Name</span></span>|
|<span data-ttu-id="be795-135">applicationType</span><span class="sxs-lookup"><span data-stu-id="be795-135">applicationType</span></span>|[<span data-ttu-id="be795-136">applicationType</span><span class="sxs-lookup"><span data-stu-id="be795-136">applicationType</span></span>](../resources/intune_wip_applicationtype.md)|<span data-ttu-id="be795-137">Anwendungstyp.</span><span class="sxs-lookup"><span data-stu-id="be795-137">Target Application Type</span></span> <span data-ttu-id="be795-138">Mögliche Werte sind: `universal` und `desktop`.</span><span class="sxs-lookup"><span data-stu-id="be795-138">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="be795-139">deviceCount</span><span class="sxs-lookup"><span data-stu-id="be795-139">deviceCount</span></span>|<span data-ttu-id="be795-140">Int32</span><span class="sxs-lookup"><span data-stu-id="be795-140">Int32</span></span>|<span data-ttu-id="be795-141">Geräteanzahl</span><span class="sxs-lookup"><span data-stu-id="be795-141">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="be795-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="be795-142">Response</span></span>
<span data-ttu-id="be795-143">Wenn erfolgreich, gibt diese Methode den `200 OK`-Antwortcode und das aktualisierte [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="be795-143">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be795-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="be795-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="be795-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="be795-145">Request</span></span>
<span data-ttu-id="be795-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="be795-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
Content-type: application/json
Content-length: 106

{
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="be795-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="be795-147">Response</span></span>
<span data-ttu-id="be795-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="be795-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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








