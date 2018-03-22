# <a name="update-telecomexpensemanagementpartner"></a><span data-ttu-id="54d57-101">telecomExpenseManagementPartner aktualisieren</span><span class="sxs-lookup"><span data-stu-id="54d57-101">Update telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="54d57-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="54d57-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="54d57-103">Aktualisieren der Eigenschaften eines [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="54d57-103">Update the properties of a [calendar](../resources/intune_tem_telecomexpensemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="54d57-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="54d57-104">Prerequisites</span></span>
<span data-ttu-id="54d57-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="54d57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="54d57-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="54d57-107">Permission type</span></span>|<span data-ttu-id="54d57-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="54d57-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54d57-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="54d57-109">Delegated (work or school account)</span></span>|<span data-ttu-id="54d57-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54d57-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="54d57-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="54d57-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54d57-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="54d57-112">Not supported.</span></span>|
|<span data-ttu-id="54d57-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="54d57-113">Application</span></span>|<span data-ttu-id="54d57-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="54d57-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54d57-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="54d57-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="54d57-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="54d57-116">Request headers</span></span>
|<span data-ttu-id="54d57-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="54d57-117">Header</span></span>|<span data-ttu-id="54d57-118">Wert</span><span class="sxs-lookup"><span data-stu-id="54d57-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54d57-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="54d57-119">Authorization</span></span>|<span data-ttu-id="54d57-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="54d57-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="54d57-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="54d57-121">Accept</span></span>|<span data-ttu-id="54d57-122">application/json</span><span class="sxs-lookup"><span data-stu-id="54d57-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54d57-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="54d57-123">Request body</span></span>
<span data-ttu-id="54d57-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="54d57-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_tem_telecomexpensemanagementpartner.md) object.</span></span>

<span data-ttu-id="54d57-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="54d57-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="54d57-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="54d57-126">Property</span></span>|<span data-ttu-id="54d57-127">Typ</span><span class="sxs-lookup"><span data-stu-id="54d57-127">Type</span></span>|<span data-ttu-id="54d57-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="54d57-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54d57-129">id</span><span class="sxs-lookup"><span data-stu-id="54d57-129">id</span></span>|<span data-ttu-id="54d57-130">String</span><span class="sxs-lookup"><span data-stu-id="54d57-130">String</span></span>|<span data-ttu-id="54d57-131">Eindeutiger Bezeichner des TEM-Partners</span><span class="sxs-lookup"><span data-stu-id="54d57-131">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="54d57-132">displayName</span><span class="sxs-lookup"><span data-stu-id="54d57-132">displayName</span></span>|<span data-ttu-id="54d57-133">String</span><span class="sxs-lookup"><span data-stu-id="54d57-133">String</span></span>|<span data-ttu-id="54d57-134">Anzeigename des TEM-Partners</span><span class="sxs-lookup"><span data-stu-id="54d57-134">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="54d57-135">url</span><span class="sxs-lookup"><span data-stu-id="54d57-135">url</span></span>|<span data-ttu-id="54d57-136">String</span><span class="sxs-lookup"><span data-stu-id="54d57-136">String</span></span>|<span data-ttu-id="54d57-137">Die URL für die Verwaltungssteuerung des TEM-Partners, mit der ein Administrator den TEM-Dienst konfigurieren kann.</span><span class="sxs-lookup"><span data-stu-id="54d57-137">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="54d57-138">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="54d57-138">appAuthorized</span></span>|<span data-ttu-id="54d57-139">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="54d57-139">Boolean</span></span>|<span data-ttu-id="54d57-140">Gibt an, ob die AAD-App des Partners für den Zugriff auf Intune autorisiert wurde.</span><span class="sxs-lookup"><span data-stu-id="54d57-140">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="54d57-141">aktiviert</span><span class="sxs-lookup"><span data-stu-id="54d57-141">enabled</span></span>|<span data-ttu-id="54d57-142">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="54d57-142">Boolean</span></span>|<span data-ttu-id="54d57-143">Gibt an, ob die Intune-Verbindung mit dem TEM-Dienst derzeit aktiviert oder deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="54d57-143">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="54d57-144">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="54d57-144">lastConnectionDateTime</span></span>|<span data-ttu-id="54d57-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54d57-145">DateTimeOffset</span></span>|<span data-ttu-id="54d57-146">Zeitstempel der letzten vom TEM-Partner an Intune gesendeten Anforderung</span><span class="sxs-lookup"><span data-stu-id="54d57-146">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="54d57-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="54d57-147">Response</span></span>
<span data-ttu-id="54d57-148">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="54d57-148">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_tem_telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54d57-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="54d57-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="54d57-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="54d57-150">Request</span></span>
<span data-ttu-id="54d57-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="54d57-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
Content-type: application/json
Content-length: 178

{
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="54d57-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="54d57-152">Response</span></span>
<span data-ttu-id="54d57-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="54d57-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 297

{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "id": "47a3b399-b399-47a3-99b3-a34799b3a347",
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```



