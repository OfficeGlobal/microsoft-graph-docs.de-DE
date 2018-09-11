# <a name="create-telecomexpensemanagementpartner"></a><span data-ttu-id="8e38a-101">telecomExpenseManagementPartner erstellen</span><span class="sxs-lookup"><span data-stu-id="8e38a-101">Create telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="8e38a-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8e38a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e38a-103">Erstellen eines neuen [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8e38a-103">Create a new [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8e38a-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8e38a-104">Prerequisites</span></span>
<span data-ttu-id="8e38a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8e38a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8e38a-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8e38a-107">Permission type</span></span>|<span data-ttu-id="8e38a-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8e38a-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e38a-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8e38a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8e38a-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e38a-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8e38a-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8e38a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e38a-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8e38a-112">Not supported.</span></span>|
|<span data-ttu-id="8e38a-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8e38a-113">Application</span></span>|<span data-ttu-id="8e38a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8e38a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e38a-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8e38a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="8e38a-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8e38a-116">Request headers</span></span>
|<span data-ttu-id="8e38a-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8e38a-117">Header</span></span>|<span data-ttu-id="8e38a-118">Wert</span><span class="sxs-lookup"><span data-stu-id="8e38a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e38a-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="8e38a-119">Authorization</span></span>|<span data-ttu-id="8e38a-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8e38a-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e38a-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="8e38a-121">Accept</span></span>|<span data-ttu-id="8e38a-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="8e38a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e38a-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8e38a-123">Request body</span></span>
<span data-ttu-id="8e38a-124">Geben Sie im Anforderungstext eine JSON-Darstellung des telecomExpenseManagementPartner-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="8e38a-124">In the request body, supply a JSON representation for the telecomExpenseManagementPartner object.</span></span>

<span data-ttu-id="8e38a-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs telecomExpenseManagementPartner erstellen.</span><span class="sxs-lookup"><span data-stu-id="8e38a-125">The following table shows the properties that are required when you create the telecomExpenseManagementPartner.</span></span>

|<span data-ttu-id="8e38a-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8e38a-126">Property</span></span>|<span data-ttu-id="8e38a-127">Typ</span><span class="sxs-lookup"><span data-stu-id="8e38a-127">Type</span></span>|<span data-ttu-id="8e38a-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8e38a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e38a-129">ID</span><span class="sxs-lookup"><span data-stu-id="8e38a-129">id</span></span>|<span data-ttu-id="8e38a-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8e38a-130">String</span></span>|<span data-ttu-id="8e38a-131">Eindeutiger Bezeichner des TEM-Partners</span><span class="sxs-lookup"><span data-stu-id="8e38a-131">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="8e38a-132">displayName</span><span class="sxs-lookup"><span data-stu-id="8e38a-132">displayName</span></span>|<span data-ttu-id="8e38a-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8e38a-133">String</span></span>|<span data-ttu-id="8e38a-134">Anzeigename des TEM-Partners</span><span class="sxs-lookup"><span data-stu-id="8e38a-134">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="8e38a-135">url</span><span class="sxs-lookup"><span data-stu-id="8e38a-135">url</span></span>|<span data-ttu-id="8e38a-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8e38a-136">String</span></span>|<span data-ttu-id="8e38a-137">Die URL für die Verwaltungssteuerung des TEM-Partners, mit der ein Administrator den TEM-Dienst konfigurieren kann.</span><span class="sxs-lookup"><span data-stu-id="8e38a-137">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="8e38a-138">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="8e38a-138">appAuthorized</span></span>|<span data-ttu-id="8e38a-139">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8e38a-139">Boolean</span></span>|<span data-ttu-id="8e38a-140">Gibt an, ob die AAD-App des Partners für den Zugriff auf Intune autorisiert wurde.</span><span class="sxs-lookup"><span data-stu-id="8e38a-140">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="8e38a-141">enabled</span><span class="sxs-lookup"><span data-stu-id="8e38a-141">enabled</span></span>|<span data-ttu-id="8e38a-142">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8e38a-142">Boolean</span></span>|<span data-ttu-id="8e38a-143">Gibt an, ob die Intune-Verbindung mit dem TEM-Dienst derzeit aktiviert oder deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="8e38a-143">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="8e38a-144">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="8e38a-144">lastConnectionDateTime</span></span>|<span data-ttu-id="8e38a-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e38a-145">DateTimeOffset</span></span>|<span data-ttu-id="8e38a-146">Zeitstempel der letzten vom TEM-Partner an Intune gesendeten Anforderung</span><span class="sxs-lookup"><span data-stu-id="8e38a-146">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="8e38a-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="8e38a-147">Response</span></span>
<span data-ttu-id="8e38a-148">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8e38a-148">If successful, this method returns a `201 Created` response code and a [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e38a-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8e38a-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="8e38a-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8e38a-150">Request</span></span>
<span data-ttu-id="8e38a-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8e38a-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners
Content-type: application/json
Content-length: 248

{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="8e38a-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="8e38a-152">Response</span></span>
<span data-ttu-id="8e38a-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8e38a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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








