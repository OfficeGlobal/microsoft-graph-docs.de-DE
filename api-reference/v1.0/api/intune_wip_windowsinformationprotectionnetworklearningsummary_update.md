# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="6dc31-101">windowsInformationProtectionNetworkLearningSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6dc31-101">Update windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="6dc31-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6dc31-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6dc31-103">Aktualisieren der Eigenschaften eines [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6dc31-103">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6dc31-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6dc31-104">Prerequisites</span></span>
<span data-ttu-id="6dc31-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6dc31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6dc31-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6dc31-107">Permission type</span></span>|<span data-ttu-id="6dc31-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6dc31-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6dc31-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6dc31-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6dc31-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dc31-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6dc31-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6dc31-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6dc31-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6dc31-112">Not supported.</span></span>|
|<span data-ttu-id="6dc31-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6dc31-113">Application</span></span>|<span data-ttu-id="6dc31-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6dc31-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6dc31-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6dc31-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="6dc31-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6dc31-116">Request headers</span></span>
|<span data-ttu-id="6dc31-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6dc31-117">Header</span></span>|<span data-ttu-id="6dc31-118">Wert</span><span class="sxs-lookup"><span data-stu-id="6dc31-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6dc31-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="6dc31-119">Authorization</span></span>|<span data-ttu-id="6dc31-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6dc31-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6dc31-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6dc31-121">Accept</span></span>|<span data-ttu-id="6dc31-122">application/json</span><span class="sxs-lookup"><span data-stu-id="6dc31-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6dc31-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6dc31-123">Request body</span></span>
<span data-ttu-id="6dc31-124">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md)-Objekt ein.</span><span class="sxs-lookup"><span data-stu-id="6dc31-124">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="6dc31-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="6dc31-125">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="6dc31-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6dc31-126">Property</span></span>|<span data-ttu-id="6dc31-127">Typ</span><span class="sxs-lookup"><span data-stu-id="6dc31-127">Type</span></span>|<span data-ttu-id="6dc31-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6dc31-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6dc31-129">id</span><span class="sxs-lookup"><span data-stu-id="6dc31-129">id</span></span>|<span data-ttu-id="6dc31-130">String</span><span class="sxs-lookup"><span data-stu-id="6dc31-130">String</span></span>|<span data-ttu-id="6dc31-131">Eindeutiger Bezeichner für die WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="6dc31-131">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="6dc31-132">url</span><span class="sxs-lookup"><span data-stu-id="6dc31-132">url</span></span>|<span data-ttu-id="6dc31-133">String</span><span class="sxs-lookup"><span data-stu-id="6dc31-133">String</span></span>|<span data-ttu-id="6dc31-134">Website-URL</span><span class="sxs-lookup"><span data-stu-id="6dc31-134">Website url</span></span>|
|<span data-ttu-id="6dc31-135">deviceCount</span><span class="sxs-lookup"><span data-stu-id="6dc31-135">deviceCount</span></span>|<span data-ttu-id="6dc31-136">Int32</span><span class="sxs-lookup"><span data-stu-id="6dc31-136">Int32</span></span>|<span data-ttu-id="6dc31-137">Geräteanzahl</span><span class="sxs-lookup"><span data-stu-id="6dc31-137">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="6dc31-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="6dc31-138">Response</span></span>
<span data-ttu-id="6dc31-139">Wenn erfolgreich, gibt diese Methode den `200 OK`-Antwortcode und das aktualisierte [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6dc31-139">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6dc31-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6dc31-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="6dc31-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6dc31-141">Request</span></span>
<span data-ttu-id="6dc31-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6dc31-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="6dc31-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="6dc31-143">Response</span></span>
<span data-ttu-id="6dc31-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6dc31-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 186

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "242108f7-08f7-2421-f708-2124f7082124",
  "url": "Url value",
  "deviceCount": 11
}
```



