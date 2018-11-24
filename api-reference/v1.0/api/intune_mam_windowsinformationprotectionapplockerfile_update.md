# <a name="update-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="e4352-101">windowsInformationProtectionAppLockerFile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e4352-101">Update windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="e4352-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e4352-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e4352-103">Aktualisieren der Eigenschaften eines [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e4352-103">Update the properties of a [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e4352-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e4352-104">Prerequisites</span></span>
<span data-ttu-id="e4352-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e4352-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e4352-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e4352-107">Permission type</span></span>|<span data-ttu-id="e4352-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e4352-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4352-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e4352-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e4352-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4352-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e4352-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e4352-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4352-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e4352-112">Not supported.</span></span>|
|<span data-ttu-id="e4352-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e4352-113">Application</span></span>|<span data-ttu-id="e4352-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e4352-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4352-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e4352-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
```

## <a name="request-headers"></a><span data-ttu-id="e4352-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e4352-116">Request headers</span></span>
|<span data-ttu-id="e4352-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e4352-117">Header</span></span>|<span data-ttu-id="e4352-118">Wert</span><span class="sxs-lookup"><span data-stu-id="e4352-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4352-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4352-119">Authorization</span></span>|<span data-ttu-id="e4352-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e4352-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4352-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e4352-121">Accept</span></span>|<span data-ttu-id="e4352-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e4352-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4352-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e4352-123">Request body</span></span>
<span data-ttu-id="e4352-124">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md)-Objekt ein.</span><span class="sxs-lookup"><span data-stu-id="e4352-124">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) object.</span></span>

<span data-ttu-id="e4352-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="e4352-125">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md).</span></span>

|<span data-ttu-id="e4352-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e4352-126">Property</span></span>|<span data-ttu-id="e4352-127">Typ</span><span class="sxs-lookup"><span data-stu-id="e4352-127">Type</span></span>|<span data-ttu-id="e4352-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e4352-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4352-129">displayName</span><span class="sxs-lookup"><span data-stu-id="e4352-129">displayName</span></span>|<span data-ttu-id="e4352-130">String</span><span class="sxs-lookup"><span data-stu-id="e4352-130">String</span></span>|<span data-ttu-id="e4352-131">Der Anzeigename</span><span class="sxs-lookup"><span data-stu-id="e4352-131">The friendly name</span></span>|
|<span data-ttu-id="e4352-132">fileHash</span><span class="sxs-lookup"><span data-stu-id="e4352-132">fileHash</span></span>|<span data-ttu-id="e4352-133">String</span><span class="sxs-lookup"><span data-stu-id="e4352-133">String</span></span>|<span data-ttu-id="e4352-134">SHA256-Hash der Datei</span><span class="sxs-lookup"><span data-stu-id="e4352-134">SHA256 hash of the file</span></span>|
|<span data-ttu-id="e4352-135">file</span><span class="sxs-lookup"><span data-stu-id="e4352-135">file</span></span>|<span data-ttu-id="e4352-136">Binär</span><span class="sxs-lookup"><span data-stu-id="e4352-136">Binary</span></span>|<span data-ttu-id="e4352-137">Datei als Bytearray</span><span class="sxs-lookup"><span data-stu-id="e4352-137">File as a byte array</span></span>|
|<span data-ttu-id="e4352-138">id</span><span class="sxs-lookup"><span data-stu-id="e4352-138">id</span></span>|<span data-ttu-id="e4352-139">String</span><span class="sxs-lookup"><span data-stu-id="e4352-139">String</span></span>|<span data-ttu-id="e4352-140">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="e4352-140">Key of the entity.</span></span>|
|<span data-ttu-id="e4352-141">Version</span><span class="sxs-lookup"><span data-stu-id="e4352-141">version</span></span>|<span data-ttu-id="e4352-142">String</span><span class="sxs-lookup"><span data-stu-id="e4352-142">String</span></span>|<span data-ttu-id="e4352-143">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="e4352-143">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="e4352-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="e4352-144">Response</span></span>
<span data-ttu-id="e4352-145">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e4352-145">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4352-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e4352-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="e4352-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e4352-147">Request</span></span>
<span data-ttu-id="e4352-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e4352-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
  "displayName": "Display Name value",
  "fileHash": "File Hash value",
  "file": "ZmlsZQ==",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="e4352-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="e4352-149">Response</span></span>
<span data-ttu-id="e4352-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e4352-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
  "displayName": "Display Name value",
  "fileHash": "File Hash value",
  "file": "ZmlsZQ==",
  "id": "d81f0e40-0e40-d81f-400e-1fd8400e1fd8",
  "version": "Version value"
}
```



