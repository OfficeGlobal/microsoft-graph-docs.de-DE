# <a name="update-managedappoperation"></a><span data-ttu-id="ec76c-101">Aktualisieren von „managedAppOperation“</span><span class="sxs-lookup"><span data-stu-id="ec76c-101">Update managedAppOperation</span></span>

> <span data-ttu-id="ec76c-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ec76c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ec76c-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedAppOperation](../resources/intune_mam_managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="ec76c-103">Update the properties of a [calendar](../resources/intune_mam_managedappoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ec76c-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ec76c-104">Prerequisites</span></span>
<span data-ttu-id="ec76c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ec76c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ec76c-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ec76c-107">Permission type</span></span>|<span data-ttu-id="ec76c-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ec76c-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec76c-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ec76c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ec76c-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec76c-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ec76c-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ec76c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec76c-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ec76c-112">Not supported.</span></span>|
|<span data-ttu-id="ec76c-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ec76c-113">Application</span></span>|<span data-ttu-id="ec76c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ec76c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec76c-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ec76c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="ec76c-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ec76c-116">Request headers</span></span>
|<span data-ttu-id="ec76c-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ec76c-117">Header</span></span>|<span data-ttu-id="ec76c-118">Wert</span><span class="sxs-lookup"><span data-stu-id="ec76c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec76c-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec76c-119">Authorization</span></span>|<span data-ttu-id="ec76c-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ec76c-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ec76c-121">Accept</span><span class="sxs-lookup"><span data-stu-id="ec76c-121">Accept</span></span>|<span data-ttu-id="ec76c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ec76c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec76c-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ec76c-123">Request body</span></span>
<span data-ttu-id="ec76c-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedAppOperation](../resources/intune_mam_managedappoperation.md) an.</span><span class="sxs-lookup"><span data-stu-id="ec76c-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_mam_managedappoperation.md) object.</span></span>

<span data-ttu-id="ec76c-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedAppOperation](../resources/intune_mam_managedappoperation.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="ec76c-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="ec76c-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ec76c-126">Property</span></span>|<span data-ttu-id="ec76c-127">Typ</span><span class="sxs-lookup"><span data-stu-id="ec76c-127">Type</span></span>|<span data-ttu-id="ec76c-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ec76c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec76c-129">displayName</span><span class="sxs-lookup"><span data-stu-id="ec76c-129">displayName</span></span>|<span data-ttu-id="ec76c-130">String</span><span class="sxs-lookup"><span data-stu-id="ec76c-130">String</span></span>|<span data-ttu-id="ec76c-131">Name des Vorgangs</span><span class="sxs-lookup"><span data-stu-id="ec76c-131">The operation name.</span></span>|
|<span data-ttu-id="ec76c-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ec76c-132">lastModifiedDateTime</span></span>|<span data-ttu-id="ec76c-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec76c-133">DateTimeOffset</span></span>|<span data-ttu-id="ec76c-134">Datum und Uhrzeit der letzten Änderung des App-Vorgangs</span><span class="sxs-lookup"><span data-stu-id="ec76c-134">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="ec76c-135">state</span><span class="sxs-lookup"><span data-stu-id="ec76c-135">state</span></span>|<span data-ttu-id="ec76c-136">String</span><span class="sxs-lookup"><span data-stu-id="ec76c-136">String</span></span>|<span data-ttu-id="ec76c-137">Aktueller Status des Vorgangs</span><span class="sxs-lookup"><span data-stu-id="ec76c-137">The current state of the operation</span></span>|
|<span data-ttu-id="ec76c-138">id</span><span class="sxs-lookup"><span data-stu-id="ec76c-138">id</span></span>|<span data-ttu-id="ec76c-139">String</span><span class="sxs-lookup"><span data-stu-id="ec76c-139">String</span></span>|<span data-ttu-id="ec76c-140">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ec76c-140">Key of the setting.</span></span>|
|<span data-ttu-id="ec76c-141">version</span><span class="sxs-lookup"><span data-stu-id="ec76c-141">version</span></span>|<span data-ttu-id="ec76c-142">String</span><span class="sxs-lookup"><span data-stu-id="ec76c-142">String</span></span>|<span data-ttu-id="ec76c-143">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="ec76c-143">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="ec76c-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="ec76c-144">Response</span></span>
<span data-ttu-id="ec76c-145">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedAppOperation](../resources/intune_mam_managedappoperation.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ec76c-145">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_mam_managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec76c-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ec76c-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="ec76c-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ec76c-147">Request</span></span>
<span data-ttu-id="ec76c-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ec76c-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
Content-type: application/json
Content-length: 165

{
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "State value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="ec76c-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="ec76c-149">Response</span></span>
<span data-ttu-id="ec76c-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ec76c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 272

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "State value",
  "id": "f2867b06-7b06-f286-067b-86f2067b86f2",
  "version": "Version value"
}
```



