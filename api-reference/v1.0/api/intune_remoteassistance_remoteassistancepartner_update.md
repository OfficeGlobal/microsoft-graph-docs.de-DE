# <a name="update-remoteassistancepartner"></a><span data-ttu-id="b5db1-101">remoteAssistancePartner aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b5db1-101">Update remoteAssistancePartner</span></span>

> <span data-ttu-id="b5db1-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b5db1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b5db1-103">Aktualisieren der Eigenschaften eines [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b5db1-103">Update the properties of a [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b5db1-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b5db1-104">Prerequisites</span></span>
<span data-ttu-id="b5db1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b5db1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b5db1-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b5db1-107">Permission type</span></span>|<span data-ttu-id="b5db1-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b5db1-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5db1-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b5db1-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b5db1-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5db1-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b5db1-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b5db1-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5db1-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b5db1-112">Not supported.</span></span>|
|<span data-ttu-id="b5db1-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b5db1-113">Application</span></span>|<span data-ttu-id="b5db1-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b5db1-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5db1-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b5db1-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="b5db1-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b5db1-116">Request headers</span></span>
|<span data-ttu-id="b5db1-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b5db1-117">Header</span></span>|<span data-ttu-id="b5db1-118">Wert</span><span class="sxs-lookup"><span data-stu-id="b5db1-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5db1-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5db1-119">Authorization</span></span>|<span data-ttu-id="b5db1-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5db1-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5db1-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b5db1-121">Accept</span></span>|<span data-ttu-id="b5db1-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b5db1-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5db1-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b5db1-123">Request body</span></span>
<span data-ttu-id="b5db1-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="b5db1-124">In the request body, supply a JSON representation for the [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) object.</span></span>

<span data-ttu-id="b5db1-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b5db1-125">The following table shows the properties that are required when you create the [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md).</span></span>

|<span data-ttu-id="b5db1-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b5db1-126">Property</span></span>|<span data-ttu-id="b5db1-127">Typ</span><span class="sxs-lookup"><span data-stu-id="b5db1-127">Type</span></span>|<span data-ttu-id="b5db1-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b5db1-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5db1-129">id</span><span class="sxs-lookup"><span data-stu-id="b5db1-129">id</span></span>|<span data-ttu-id="b5db1-130">String</span><span class="sxs-lookup"><span data-stu-id="b5db1-130">String</span></span>|<span data-ttu-id="b5db1-131">Der eindeutige Bezeichner des Partners.</span><span class="sxs-lookup"><span data-stu-id="b5db1-131">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="b5db1-132">displayName</span><span class="sxs-lookup"><span data-stu-id="b5db1-132">displayName</span></span>|<span data-ttu-id="b5db1-133">String</span><span class="sxs-lookup"><span data-stu-id="b5db1-133">String</span></span>|<span data-ttu-id="b5db1-134">Der Anzeigename des Partners.</span><span class="sxs-lookup"><span data-stu-id="b5db1-134">Display name of the partner.</span></span>|
|<span data-ttu-id="b5db1-135">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="b5db1-135">onboardingUrl</span></span>|<span data-ttu-id="b5db1-136">String</span><span class="sxs-lookup"><span data-stu-id="b5db1-136">String</span></span>|<span data-ttu-id="b5db1-137">Die URL des Onboarding-Portals des Partners, in dem ein Administrator den Remoteunterstützungsdienst konfigurieren kann.</span><span class="sxs-lookup"><span data-stu-id="b5db1-137">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="b5db1-138">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="b5db1-138">onboardingStatus</span></span>|[<span data-ttu-id="b5db1-139">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="b5db1-139">remoteAssistanceOnboardingStatus</span></span>](../resources/intune_remoteassistance_remoteassistanceonboardingstatus.md)|<span data-ttu-id="b5db1-140">TBD.</span><span class="sxs-lookup"><span data-stu-id="b5db1-140">TBD.</span></span> <span data-ttu-id="b5db1-141">Mögliche Werte sind: `notOnboarded`, `onboarding` und `onboarded`.</span><span class="sxs-lookup"><span data-stu-id="b5db1-141">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="b5db1-142">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="b5db1-142">lastConnectionDateTime</span></span>|<span data-ttu-id="b5db1-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5db1-143">DateTimeOffset</span></span>|<span data-ttu-id="b5db1-144">Zeitstempel der letzten vom TEM-Partner an Intune gesendeten Anforderung</span><span class="sxs-lookup"><span data-stu-id="b5db1-144">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="b5db1-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="b5db1-145">Response</span></span>
<span data-ttu-id="b5db1-146">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b5db1-146">If successful, this method returns a `200 OK` response code and an updated [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5db1-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b5db1-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="b5db1-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b5db1-148">Request</span></span>
<span data-ttu-id="b5db1-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b5db1-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
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

### <a name="response"></a><span data-ttu-id="b5db1-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="b5db1-150">Response</span></span>
<span data-ttu-id="b5db1-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b5db1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



