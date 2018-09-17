# <a name="create-deviceconfigurationuserstatus"></a><span data-ttu-id="c9421-101">Erstellen von „deviceConfigurationUserStatus“</span><span class="sxs-lookup"><span data-stu-id="c9421-101">Create deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="c9421-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c9421-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c9421-103">Diese Methode erstellt ein neues Objekt des Typs [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="c9421-103">Create a new [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c9421-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c9421-104">Prerequisites</span></span>
<span data-ttu-id="c9421-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c9421-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c9421-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c9421-107">Permission type</span></span>|<span data-ttu-id="c9421-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c9421-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9421-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c9421-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c9421-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9421-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c9421-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c9421-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9421-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c9421-112">Not supported.</span></span>|
|<span data-ttu-id="c9421-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c9421-113">Application</span></span>|<span data-ttu-id="c9421-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c9421-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9421-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c9421-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="c9421-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c9421-116">Request headers</span></span>
|<span data-ttu-id="c9421-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c9421-117">Header</span></span>|<span data-ttu-id="c9421-118">Wert</span><span class="sxs-lookup"><span data-stu-id="c9421-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9421-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c9421-119">Authorization</span></span>|<span data-ttu-id="c9421-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c9421-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9421-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="c9421-121">Accept</span></span>|<span data-ttu-id="c9421-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="c9421-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9421-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c9421-123">Request body</span></span>
<span data-ttu-id="c9421-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceConfigurationUserStatus“ an.</span><span class="sxs-lookup"><span data-stu-id="c9421-124">In the request body, supply a JSON representation for the deviceConfigurationUserStatus object.</span></span>

<span data-ttu-id="c9421-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceConfigurationUserStatus“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="c9421-125">The following table shows the properties that are required when you create the deviceConfigurationUserStatus.</span></span>

|<span data-ttu-id="c9421-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c9421-126">Property</span></span>|<span data-ttu-id="c9421-127">Typ</span><span class="sxs-lookup"><span data-stu-id="c9421-127">Type</span></span>|<span data-ttu-id="c9421-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c9421-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9421-129">ID</span><span class="sxs-lookup"><span data-stu-id="c9421-129">id</span></span>|<span data-ttu-id="c9421-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c9421-130">String</span></span>|<span data-ttu-id="c9421-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c9421-131">Key of the entity.</span></span>|
|<span data-ttu-id="c9421-132">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="c9421-132">userDisplayName</span></span>|<span data-ttu-id="c9421-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c9421-133">String</span></span>|<span data-ttu-id="c9421-134">Benutzername, der zu dem Objekt des Typs „DevicePolicyStatus“ gehört</span><span class="sxs-lookup"><span data-stu-id="c9421-134">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="c9421-135">devicesCount</span><span class="sxs-lookup"><span data-stu-id="c9421-135">devicesCount</span></span>|<span data-ttu-id="c9421-136">Int32</span><span class="sxs-lookup"><span data-stu-id="c9421-136">Int32</span></span>|<span data-ttu-id="c9421-137">Geräteanzahl für den Benutzer</span><span class="sxs-lookup"><span data-stu-id="c9421-137">Devices count for that user.</span></span>|
|<span data-ttu-id="c9421-138">Status</span><span class="sxs-lookup"><span data-stu-id="c9421-138">status</span></span>|[<span data-ttu-id="c9421-139">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="c9421-139">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="c9421-p102">Compliance-Status des Richtlinienberichts. Mögliche Werte: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="c9421-p102">Compliance status of the policy report. The possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="c9421-142">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9421-142">lastReportedDateTime</span></span>|<span data-ttu-id="c9421-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9421-143">DateTimeOffset</span></span>|<span data-ttu-id="c9421-144">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="c9421-144">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="c9421-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c9421-145">userPrincipalName</span></span>|<span data-ttu-id="c9421-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c9421-146">String</span></span>|<span data-ttu-id="c9421-147">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="c9421-147">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="c9421-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="c9421-148">Response</span></span>
<span data-ttu-id="c9421-149">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c9421-149">If successful, this method returns a `201 Created` response code and a [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9421-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c9421-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="c9421-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c9421-151">Request</span></span>
<span data-ttu-id="c9421-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c9421-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
Content-type: application/json
Content-length: 290

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="c9421-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="c9421-153">Response</span></span>
<span data-ttu-id="c9421-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c9421-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 339

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
  "id": "7e323db2-3db2-7e32-b23d-327eb23d327e",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```








