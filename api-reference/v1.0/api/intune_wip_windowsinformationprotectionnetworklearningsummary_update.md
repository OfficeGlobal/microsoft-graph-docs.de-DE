# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="aae16-101">windowsInformationProtectionNetworkLearningSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="aae16-101">Update windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="aae16-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="aae16-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aae16-103">Aktualisieren der Eigenschaften eines [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="aae16-103">Update the properties of a [calendar](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aae16-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="aae16-104">Prerequisites</span></span>
<span data-ttu-id="aae16-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="aae16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="aae16-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="aae16-107">Permission type</span></span>|<span data-ttu-id="aae16-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="aae16-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aae16-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="aae16-109">Delegated (work or school account)</span></span>|<span data-ttu-id="aae16-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aae16-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="aae16-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="aae16-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aae16-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aae16-112">Not supported.</span></span>|
|<span data-ttu-id="aae16-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="aae16-113">Application</span></span>|<span data-ttu-id="aae16-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aae16-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aae16-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aae16-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="aae16-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="aae16-116">Request headers</span></span>
|<span data-ttu-id="aae16-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="aae16-117">Header</span></span>|<span data-ttu-id="aae16-118">Wert</span><span class="sxs-lookup"><span data-stu-id="aae16-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aae16-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="aae16-119">Authorization</span></span>|<span data-ttu-id="aae16-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="aae16-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="aae16-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="aae16-121">Accept</span></span>|<span data-ttu-id="aae16-122">application/json</span><span class="sxs-lookup"><span data-stu-id="aae16-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aae16-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="aae16-123">Request body</span></span>
<span data-ttu-id="aae16-124">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md)-Objekt ein.</span><span class="sxs-lookup"><span data-stu-id="aae16-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="aae16-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="aae16-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="aae16-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="aae16-126">Property</span></span>|<span data-ttu-id="aae16-127">Typ</span><span class="sxs-lookup"><span data-stu-id="aae16-127">Type</span></span>|<span data-ttu-id="aae16-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aae16-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aae16-129">id</span><span class="sxs-lookup"><span data-stu-id="aae16-129">id</span></span>|<span data-ttu-id="aae16-130">String</span><span class="sxs-lookup"><span data-stu-id="aae16-130">String</span></span>|<span data-ttu-id="aae16-131">Eindeutiger Bezeichner für die WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="aae16-131">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="aae16-132">url</span><span class="sxs-lookup"><span data-stu-id="aae16-132">url</span></span>|<span data-ttu-id="aae16-133">String</span><span class="sxs-lookup"><span data-stu-id="aae16-133">String</span></span>|<span data-ttu-id="aae16-134">Website-URL</span><span class="sxs-lookup"><span data-stu-id="aae16-134">Website url</span></span>|
|<span data-ttu-id="aae16-135">deviceCount</span><span class="sxs-lookup"><span data-stu-id="aae16-135">deviceCount</span></span>|<span data-ttu-id="aae16-136">Int32</span><span class="sxs-lookup"><span data-stu-id="aae16-136">Int32</span></span>|<span data-ttu-id="aae16-137">Geräteanzahl</span><span class="sxs-lookup"><span data-stu-id="aae16-137">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="aae16-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="aae16-138">Response</span></span>
<span data-ttu-id="aae16-139">Wenn erfolgreich, gibt diese Methode den `200 OK`-Antwortcode und das aktualisierte [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="aae16-139">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aae16-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="aae16-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="aae16-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aae16-141">Request</span></span>
<span data-ttu-id="aae16-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="aae16-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
Content-type: application/json
Content-length: 48

{
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="aae16-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="aae16-143">Response</span></span>
<span data-ttu-id="aae16-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aae16-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



