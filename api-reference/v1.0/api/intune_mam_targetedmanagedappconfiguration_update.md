# <a name="update-targetedmanagedappconfiguration"></a><span data-ttu-id="2e10a-101">targetedManagedAppConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2e10a-101">Update targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="2e10a-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2e10a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2e10a-103">Aktualisieren der Eigenschaften eines [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md)- Objekts.</span><span class="sxs-lookup"><span data-stu-id="2e10a-103">Update the properties of a [calendar](../resources/intune_mam_targetedmanagedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2e10a-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2e10a-104">Prerequisites</span></span>
<span data-ttu-id="2e10a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2e10a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2e10a-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2e10a-107">Permission type</span></span>|<span data-ttu-id="2e10a-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2e10a-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e10a-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2e10a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2e10a-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e10a-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2e10a-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2e10a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e10a-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2e10a-112">Not supported.</span></span>|
|<span data-ttu-id="2e10a-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2e10a-113">Application</span></span>|<span data-ttu-id="2e10a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2e10a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e10a-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2e10a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2e10a-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2e10a-116">Request headers</span></span>
|<span data-ttu-id="2e10a-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2e10a-117">Header</span></span>|<span data-ttu-id="2e10a-118">Wert</span><span class="sxs-lookup"><span data-stu-id="2e10a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e10a-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e10a-119">Authorization</span></span>|<span data-ttu-id="2e10a-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2e10a-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2e10a-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2e10a-121">Accept</span></span>|<span data-ttu-id="2e10a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2e10a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e10a-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2e10a-123">Request body</span></span>
<span data-ttu-id="2e10a-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="2e10a-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_mam_targetedmanagedappconfiguration.md) object.</span></span>

<span data-ttu-id="2e10a-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="2e10a-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="2e10a-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2e10a-126">Property</span></span>|<span data-ttu-id="2e10a-127">Typ</span><span class="sxs-lookup"><span data-stu-id="2e10a-127">Type</span></span>|<span data-ttu-id="2e10a-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2e10a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e10a-129">displayName</span><span class="sxs-lookup"><span data-stu-id="2e10a-129">displayName</span></span>|<span data-ttu-id="2e10a-130">String</span><span class="sxs-lookup"><span data-stu-id="2e10a-130">String</span></span>|<span data-ttu-id="2e10a-131">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="2e10a-131">Policy display name.</span></span> <span data-ttu-id="2e10a-132">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2e10a-132">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="2e10a-133">description</span><span class="sxs-lookup"><span data-stu-id="2e10a-133">description</span></span>|<span data-ttu-id="2e10a-134">String</span><span class="sxs-lookup"><span data-stu-id="2e10a-134">String</span></span>|<span data-ttu-id="2e10a-135">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="2e10a-135">The policy's description.</span></span> <span data-ttu-id="2e10a-136">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2e10a-136">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="2e10a-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2e10a-137">createdDateTime</span></span>|<span data-ttu-id="2e10a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e10a-138">DateTimeOffset</span></span>|<span data-ttu-id="2e10a-139">Datum und Uhrzeit der Erstellung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="2e10a-139">The date and time the group was created.</span></span> <span data-ttu-id="2e10a-140">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2e10a-140">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="2e10a-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2e10a-141">lastModifiedDateTime</span></span>|<span data-ttu-id="2e10a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e10a-142">DateTimeOffset</span></span>|<span data-ttu-id="2e10a-143">Datum und Uhrzeit der letzten Änderung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="2e10a-143">Last time the policy was modified.</span></span> <span data-ttu-id="2e10a-144">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2e10a-144">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="2e10a-145">id</span><span class="sxs-lookup"><span data-stu-id="2e10a-145">id</span></span>|<span data-ttu-id="2e10a-146">String</span><span class="sxs-lookup"><span data-stu-id="2e10a-146">String</span></span>|<span data-ttu-id="2e10a-147">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="2e10a-147">Key of the setting.</span></span> <span data-ttu-id="2e10a-148">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2e10a-148">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="2e10a-149">Version</span><span class="sxs-lookup"><span data-stu-id="2e10a-149">version</span></span>|<span data-ttu-id="2e10a-150">String</span><span class="sxs-lookup"><span data-stu-id="2e10a-150">String</span></span>|<span data-ttu-id="2e10a-151">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="2e10a-151">Version of the entity.</span></span> <span data-ttu-id="2e10a-152">Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2e10a-152">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="2e10a-153">customSettings</span><span class="sxs-lookup"><span data-stu-id="2e10a-153">customSettings</span></span>|<span data-ttu-id="2e10a-154">[keyValuePair](../resources/intune_mam_keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="2e10a-154">[keyValuePair](../resources/intune_mam_keyvaluepair.md) collection</span></span>|<span data-ttu-id="2e10a-155">Eine Gruppe von Paaren aus Schlüsselzeichenfolge und Wertzeichenfolge, die an Apps für Benutzer im Bereich der Konfiguration gesendet werden sollen, und zwar ohne Veränderungen durch den Dienst. Geerbt von [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2e10a-155">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md)</span></span>|
|<span data-ttu-id="2e10a-156">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="2e10a-156">deployedAppCount</span></span>|<span data-ttu-id="2e10a-157">Int32</span><span class="sxs-lookup"><span data-stu-id="2e10a-157">Int32</span></span>|<span data-ttu-id="2e10a-158">Anzahl der Apps, für die die aktuelle Richtlinie bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="2e10a-158">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="2e10a-159">isAssigned</span><span class="sxs-lookup"><span data-stu-id="2e10a-159">isAssigned</span></span>|<span data-ttu-id="2e10a-160">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2e10a-160">Boolean</span></span>|<span data-ttu-id="2e10a-161">Gibt an, ob die Richtlinie für eine oder mehrere Einschlussgruppen bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="2e10a-161">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="2e10a-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="2e10a-162">Response</span></span>
<span data-ttu-id="2e10a-163">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2e10a-163">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_mam_targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e10a-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2e10a-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="2e10a-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2e10a-165">Request</span></span>
<span data-ttu-id="2e10a-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2e10a-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
Content-type: application/json
Content-length: 382

{
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

### <a name="response"></a><span data-ttu-id="2e10a-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="2e10a-167">Response</span></span>
<span data-ttu-id="2e10a-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2e10a-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



