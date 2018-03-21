# <a name="create-remoteassistancepartner"></a><span data-ttu-id="570b5-101">remoteAssistancePartner erstellen</span><span class="sxs-lookup"><span data-stu-id="570b5-101">Create remoteAssistancePartner</span></span>

> <span data-ttu-id="570b5-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="570b5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="570b5-103">Erstellen eines neuen [RemoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="570b5-103">Create a new [plannerBucket](../resources/intune_remoteassistance_remoteassistancepartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="570b5-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="570b5-104">Prerequisites</span></span>
<span data-ttu-id="570b5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="570b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="570b5-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="570b5-107">Permission type</span></span>|<span data-ttu-id="570b5-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="570b5-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="570b5-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="570b5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="570b5-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="570b5-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="570b5-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="570b5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="570b5-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="570b5-112">Not supported.</span></span>|
|<span data-ttu-id="570b5-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="570b5-113">Application</span></span>|<span data-ttu-id="570b5-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="570b5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="570b5-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="570b5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="570b5-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="570b5-116">Request headers</span></span>
|<span data-ttu-id="570b5-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="570b5-117">Header</span></span>|<span data-ttu-id="570b5-118">Wert</span><span class="sxs-lookup"><span data-stu-id="570b5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="570b5-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="570b5-119">Authorization</span></span>|<span data-ttu-id="570b5-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="570b5-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="570b5-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="570b5-121">Accept</span></span>|<span data-ttu-id="570b5-122">application/json</span><span class="sxs-lookup"><span data-stu-id="570b5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="570b5-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="570b5-123">Request body</span></span>
<span data-ttu-id="570b5-124">Geben Sie im Anforderungstext eine JSON-Darstellung des remoteAssistancePartner-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="570b5-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="570b5-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des remoteAssistancePartner erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="570b5-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="570b5-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="570b5-126">Property</span></span>|<span data-ttu-id="570b5-127">Typ</span><span class="sxs-lookup"><span data-stu-id="570b5-127">Type</span></span>|<span data-ttu-id="570b5-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="570b5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="570b5-129">id</span><span class="sxs-lookup"><span data-stu-id="570b5-129">id</span></span>|<span data-ttu-id="570b5-130">String</span><span class="sxs-lookup"><span data-stu-id="570b5-130">String</span></span>|<span data-ttu-id="570b5-131">Der eindeutige Bezeichner des Partners.</span><span class="sxs-lookup"><span data-stu-id="570b5-131">Unique identifier of the folder.</span></span>|
|<span data-ttu-id="570b5-132">displayName</span><span class="sxs-lookup"><span data-stu-id="570b5-132">displayName</span></span>|<span data-ttu-id="570b5-133">String</span><span class="sxs-lookup"><span data-stu-id="570b5-133">String</span></span>|<span data-ttu-id="570b5-134">Der Anzeigename des Partners.</span><span class="sxs-lookup"><span data-stu-id="570b5-134">Display name of the template.</span></span>|
|<span data-ttu-id="570b5-135">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="570b5-135">onboardingUrl</span></span>|<span data-ttu-id="570b5-136">String</span><span class="sxs-lookup"><span data-stu-id="570b5-136">String</span></span>|<span data-ttu-id="570b5-137">Die URL des Onboarding-Portals des Partners, in dem ein Administrator den Remoteunterstützungsdienst konfigurieren kann.</span><span class="sxs-lookup"><span data-stu-id="570b5-137">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="570b5-138">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="570b5-138">onboardingStatus</span></span>|<span data-ttu-id="570b5-139">String</span><span class="sxs-lookup"><span data-stu-id="570b5-139">String</span></span>|<span data-ttu-id="570b5-140">Noch nicht festgelegt; mögliche Werte: `notOnboarded`, `onboarding`, `onboarded`.</span><span class="sxs-lookup"><span data-stu-id="570b5-140">Possible values are: `notOnboarded`, `onboarding`, `onboarded`, .</span></span>|
|<span data-ttu-id="570b5-141">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="570b5-141">lastConnectionDateTime</span></span>|<span data-ttu-id="570b5-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="570b5-142">DateTimeOffset</span></span>|<span data-ttu-id="570b5-143">Zeitstempel der letzten vom TEM-Partner an Intune gesendeten Anforderung</span><span class="sxs-lookup"><span data-stu-id="570b5-143">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="570b5-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="570b5-144">Response</span></span>
<span data-ttu-id="570b5-145">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="570b5-145">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_remoteassistance_remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="570b5-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="570b5-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="570b5-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="570b5-147">Request</span></span>
<span data-ttu-id="570b5-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="570b5-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners
Content-type: application/json
Content-length: 266

{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="570b5-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="570b5-149">Response</span></span>
<span data-ttu-id="570b5-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="570b5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 315

{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "7443c8b9-c8b9-7443-b9c8-4374b9c84374",
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```



