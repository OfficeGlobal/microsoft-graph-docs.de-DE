# <a name="create-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="16dd1-101">windowsInformationProtectionNetworkLearningSummary erstellen</span><span class="sxs-lookup"><span data-stu-id="16dd1-101">Create windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="16dd1-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="16dd1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16dd1-103">Erstellen eines neuen [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="16dd1-103">Create a new [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="16dd1-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="16dd1-104">Prerequisites</span></span>
<span data-ttu-id="16dd1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="16dd1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="16dd1-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="16dd1-107">Permission type</span></span>|<span data-ttu-id="16dd1-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="16dd1-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16dd1-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="16dd1-109">Delegated (work or school account)</span></span>|<span data-ttu-id="16dd1-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16dd1-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="16dd1-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="16dd1-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16dd1-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="16dd1-112">Not supported.</span></span>|
|<span data-ttu-id="16dd1-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="16dd1-113">Application</span></span>|<span data-ttu-id="16dd1-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="16dd1-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16dd1-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="16dd1-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="16dd1-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="16dd1-116">Request headers</span></span>
|<span data-ttu-id="16dd1-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="16dd1-117">Header</span></span>|<span data-ttu-id="16dd1-118">Wert</span><span class="sxs-lookup"><span data-stu-id="16dd1-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16dd1-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="16dd1-119">Authorization</span></span>|<span data-ttu-id="16dd1-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="16dd1-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16dd1-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="16dd1-121">Accept</span></span>|<span data-ttu-id="16dd1-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="16dd1-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16dd1-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="16dd1-123">Request body</span></span>
<span data-ttu-id="16dd1-124">Geben Sie im Anforderungstext eine JSON-Darstellung für das windowsInformationProtectionNetworkLearningSummary-Objekt ein.</span><span class="sxs-lookup"><span data-stu-id="16dd1-124">In the request body, supply a JSON representation for the windowsInformationProtectionNetworkLearningSummary object.</span></span>

<span data-ttu-id="16dd1-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsInformationProtectionNetworkLearningSummary erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="16dd1-125">The following table shows the properties that are required when you create the windowsInformationProtectionNetworkLearningSummary.</span></span>

|<span data-ttu-id="16dd1-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="16dd1-126">Property</span></span>|<span data-ttu-id="16dd1-127">Typ</span><span class="sxs-lookup"><span data-stu-id="16dd1-127">Type</span></span>|<span data-ttu-id="16dd1-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="16dd1-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16dd1-129">ID</span><span class="sxs-lookup"><span data-stu-id="16dd1-129">id</span></span>|<span data-ttu-id="16dd1-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="16dd1-130">String</span></span>|<span data-ttu-id="16dd1-131">Eindeutiger Bezeichner für die WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="16dd1-131">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="16dd1-132">URL</span><span class="sxs-lookup"><span data-stu-id="16dd1-132">url</span></span>|<span data-ttu-id="16dd1-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="16dd1-133">String</span></span>|<span data-ttu-id="16dd1-134">Website-URL</span><span class="sxs-lookup"><span data-stu-id="16dd1-134">Website url</span></span>|
|<span data-ttu-id="16dd1-135">deviceCount</span><span class="sxs-lookup"><span data-stu-id="16dd1-135">deviceCount</span></span>|<span data-ttu-id="16dd1-136">Int32</span><span class="sxs-lookup"><span data-stu-id="16dd1-136">Int32</span></span>|<span data-ttu-id="16dd1-137">Geräteanzahl</span><span class="sxs-lookup"><span data-stu-id="16dd1-137">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="16dd1-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="16dd1-138">Response</span></span>
<span data-ttu-id="16dd1-139">Wenn erfolgreich, gibt diese Methode den `201 Created`-Antwortcode und das [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="16dd1-139">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16dd1-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="16dd1-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="16dd1-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="16dd1-141">Request</span></span>
<span data-ttu-id="16dd1-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="16dd1-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionNetworkLearningSummaries
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="16dd1-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="16dd1-143">Response</span></span>
<span data-ttu-id="16dd1-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="16dd1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 186

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "242108f7-08f7-2421-f708-2124f7082124",
  "url": "Url value",
  "deviceCount": 11
}
```








