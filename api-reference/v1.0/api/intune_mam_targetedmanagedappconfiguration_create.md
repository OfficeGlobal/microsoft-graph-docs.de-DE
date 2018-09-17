# <a name="create-targetedmanagedappconfiguration"></a><span data-ttu-id="279a7-101">targetedManagedAppConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="279a7-101">Create targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="279a7-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="279a7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="279a7-103">Erstellen eines neuen [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="279a7-103">Create a new [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="279a7-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="279a7-104">Prerequisites</span></span>
<span data-ttu-id="279a7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="279a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="279a7-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="279a7-107">Permission type</span></span>|<span data-ttu-id="279a7-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="279a7-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="279a7-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="279a7-109">Delegated (work or school account)</span></span>|<span data-ttu-id="279a7-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="279a7-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="279a7-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="279a7-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="279a7-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="279a7-112">Not supported.</span></span>|
|<span data-ttu-id="279a7-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="279a7-113">Application</span></span>|<span data-ttu-id="279a7-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="279a7-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="279a7-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="279a7-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="279a7-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="279a7-116">Request headers</span></span>
|<span data-ttu-id="279a7-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="279a7-117">Header</span></span>|<span data-ttu-id="279a7-118">Wert</span><span class="sxs-lookup"><span data-stu-id="279a7-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="279a7-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="279a7-119">Authorization</span></span>|<span data-ttu-id="279a7-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="279a7-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="279a7-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="279a7-121">Accept</span></span>|<span data-ttu-id="279a7-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="279a7-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="279a7-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="279a7-123">Request body</span></span>
<span data-ttu-id="279a7-124">Geben Sie im Anforderungstext eine JSON-Darstellung des targetedManagedAppConfiguration-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="279a7-124">In the request body, supply a JSON representation for the targetedManagedAppConfiguration object.</span></span>

<span data-ttu-id="279a7-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs targetedManagedAppConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="279a7-125">The following table shows the properties that are required when you create the targetedManagedAppConfiguration.</span></span>

|<span data-ttu-id="279a7-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="279a7-126">Property</span></span>|<span data-ttu-id="279a7-127">Typ</span><span class="sxs-lookup"><span data-stu-id="279a7-127">Type</span></span>|<span data-ttu-id="279a7-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="279a7-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="279a7-129">displayName</span><span class="sxs-lookup"><span data-stu-id="279a7-129">displayName</span></span>|<span data-ttu-id="279a7-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="279a7-130">String</span></span>|<span data-ttu-id="279a7-131">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="279a7-131">Policy display name.</span></span> <span data-ttu-id="279a7-132">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="279a7-132">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="279a7-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="279a7-133">description</span></span>|<span data-ttu-id="279a7-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="279a7-134">String</span></span>|<span data-ttu-id="279a7-135">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="279a7-135">The policy's description.</span></span> <span data-ttu-id="279a7-136">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="279a7-136">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="279a7-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="279a7-137">createdDateTime</span></span>|<span data-ttu-id="279a7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="279a7-138">DateTimeOffset</span></span>|<span data-ttu-id="279a7-139">Datum und Uhrzeit der Erstellung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="279a7-139">The date and time the policy was created.</span></span> <span data-ttu-id="279a7-140">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="279a7-140">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="279a7-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="279a7-141">lastModifiedDateTime</span></span>|<span data-ttu-id="279a7-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="279a7-142">DateTimeOffset</span></span>|<span data-ttu-id="279a7-143">Datum und Uhrzeit der letzten Änderung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="279a7-143">Last time the policy was modified.</span></span> <span data-ttu-id="279a7-144">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="279a7-144">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="279a7-145">ID</span><span class="sxs-lookup"><span data-stu-id="279a7-145">id</span></span>|<span data-ttu-id="279a7-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="279a7-146">String</span></span>|<span data-ttu-id="279a7-147">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="279a7-147">Key of the entity.</span></span> <span data-ttu-id="279a7-148">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="279a7-148">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="279a7-149">Version</span><span class="sxs-lookup"><span data-stu-id="279a7-149">version</span></span>|<span data-ttu-id="279a7-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="279a7-150">String</span></span>|<span data-ttu-id="279a7-151">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="279a7-151">Version of the entity.</span></span> <span data-ttu-id="279a7-152">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="279a7-152">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="279a7-153">customSettings</span><span class="sxs-lookup"><span data-stu-id="279a7-153">customSettings</span></span>|<span data-ttu-id="279a7-154">[keyValuePair](../resources/intune_mam_keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="279a7-154">[keyValuePair](../resources/intune_mam_keyvaluepair.md) collection</span></span>|<span data-ttu-id="279a7-155">Eine Gruppe von Paaren aus Schlüsselzeichenfolge und Wertzeichenfolge, die an Apps für Benutzer im Bereich der Konfiguration gesendet werden sollen, und zwar ohne Veränderungen durch den Dienst. Geerbt von [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="279a7-155">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md)</span></span>|
|<span data-ttu-id="279a7-156">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="279a7-156">deployedAppCount</span></span>|<span data-ttu-id="279a7-157">Int32</span><span class="sxs-lookup"><span data-stu-id="279a7-157">Int32</span></span>|<span data-ttu-id="279a7-158">Anzahl der Apps, für die die aktuelle Richtlinie bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="279a7-158">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="279a7-159">isAssigned</span><span class="sxs-lookup"><span data-stu-id="279a7-159">isAssigned</span></span>|<span data-ttu-id="279a7-160">Boolesch</span><span class="sxs-lookup"><span data-stu-id="279a7-160">Boolean</span></span>|<span data-ttu-id="279a7-161">Gibt an, ob die Richtlinie für eine oder mehrere Einschlussgruppen bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="279a7-161">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="279a7-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="279a7-162">Response</span></span>
<span data-ttu-id="279a7-163">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="279a7-163">If successful, this method returns a `201 Created` response code and a [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="279a7-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="279a7-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="279a7-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="279a7-165">Request</span></span>
<span data-ttu-id="279a7-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="279a7-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations
Content-type: application/json
Content-length: 452

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": "Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "isAssigned": true
}
```

### <a name="response"></a><span data-ttu-id="279a7-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="279a7-167">Response</span></span>
<span data-ttu-id="279a7-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="279a7-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 560

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "id": "2444e029-e029-2444-29e0-442429e04424",
  "version": "Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "isAssigned": true
}
```








