# <a name="update-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="c3008-101">windowsInformationProtectionAppLearningSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c3008-101">Update windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="c3008-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c3008-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c3008-103">Aktualisieren der Eigenschaften eines [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c3008-103">Update the properties of a [calendar](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c3008-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c3008-104">Prerequisites</span></span>
<span data-ttu-id="c3008-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c3008-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c3008-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c3008-107">Permission type</span></span>|<span data-ttu-id="c3008-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c3008-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3008-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c3008-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c3008-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3008-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c3008-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c3008-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3008-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c3008-112">Not supported.</span></span>|
|<span data-ttu-id="c3008-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c3008-113">Application</span></span>|<span data-ttu-id="c3008-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c3008-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3008-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c3008-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="c3008-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c3008-116">Request headers</span></span>
|<span data-ttu-id="c3008-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c3008-117">Header</span></span>|<span data-ttu-id="c3008-118">Wert</span><span class="sxs-lookup"><span data-stu-id="c3008-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3008-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3008-119">Authorization</span></span>|<span data-ttu-id="c3008-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c3008-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c3008-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c3008-121">Accept</span></span>|<span data-ttu-id="c3008-122">application/json</span><span class="sxs-lookup"><span data-stu-id="c3008-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3008-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c3008-123">Request body</span></span>
<span data-ttu-id="c3008-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="c3008-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) object.</span></span>

<span data-ttu-id="c3008-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c3008-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="c3008-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c3008-126">Property</span></span>|<span data-ttu-id="c3008-127">Typ</span><span class="sxs-lookup"><span data-stu-id="c3008-127">Type</span></span>|<span data-ttu-id="c3008-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c3008-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3008-129">id</span><span class="sxs-lookup"><span data-stu-id="c3008-129">id</span></span>|<span data-ttu-id="c3008-130">String</span><span class="sxs-lookup"><span data-stu-id="c3008-130">String</span></span>|<span data-ttu-id="c3008-131">Eindeutiger Bezeichner für die WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="c3008-131">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="c3008-132">applicationName</span><span class="sxs-lookup"><span data-stu-id="c3008-132">applicationName</span></span>|<span data-ttu-id="c3008-133">String</span><span class="sxs-lookup"><span data-stu-id="c3008-133">String</span></span>|<span data-ttu-id="c3008-134">Name der Anwendung</span><span class="sxs-lookup"><span data-stu-id="c3008-134">Application Name</span></span>|
|<span data-ttu-id="c3008-135">applicationType</span><span class="sxs-lookup"><span data-stu-id="c3008-135">applicationType</span></span>|<span data-ttu-id="c3008-136">String</span><span class="sxs-lookup"><span data-stu-id="c3008-136">String</span></span>|<span data-ttu-id="c3008-137">Typ der Anwendung. Mögliche Werte sind: `universal`, `desktop`.</span><span class="sxs-lookup"><span data-stu-id="c3008-137">Application Type Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="c3008-138">deviceCount</span><span class="sxs-lookup"><span data-stu-id="c3008-138">deviceCount</span></span>|<span data-ttu-id="c3008-139">Int32</span><span class="sxs-lookup"><span data-stu-id="c3008-139">Int32</span></span>|<span data-ttu-id="c3008-140">Geräteanzahl</span><span class="sxs-lookup"><span data-stu-id="c3008-140">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="c3008-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="c3008-141">Response</span></span>
<span data-ttu-id="c3008-142">Wenn erfolgreich, gibt diese Methode den `200 OK`-Antwortcode und das aktualisierte [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c3008-142">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3008-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c3008-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="c3008-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c3008-144">Request</span></span>
<span data-ttu-id="c3008-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c3008-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c3008-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="c3008-146">Response</span></span>
<span data-ttu-id="c3008-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c3008-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



