# <a name="update-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="4c17d-101">windowsInformationProtectionAppLockerFile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="4c17d-101">Update windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="4c17d-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4c17d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4c17d-103">Aktualisieren der Eigenschaften eines [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="4c17d-103">Update the properties of a [calendar](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4c17d-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4c17d-104">Prerequisites</span></span>
<span data-ttu-id="4c17d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4c17d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4c17d-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4c17d-107">Permission type</span></span>|<span data-ttu-id="4c17d-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4c17d-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c17d-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4c17d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4c17d-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c17d-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4c17d-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4c17d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c17d-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4c17d-112">Not supported.</span></span>|
|<span data-ttu-id="4c17d-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4c17d-113">Application</span></span>|<span data-ttu-id="4c17d-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4c17d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c17d-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4c17d-115">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="4c17d-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4c17d-116">Request headers</span></span>
|<span data-ttu-id="4c17d-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4c17d-117">Header</span></span>|<span data-ttu-id="4c17d-118">Wert</span><span class="sxs-lookup"><span data-stu-id="4c17d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c17d-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c17d-119">Authorization</span></span>|<span data-ttu-id="4c17d-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4c17d-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4c17d-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4c17d-121">Accept</span></span>|<span data-ttu-id="4c17d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4c17d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c17d-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4c17d-123">Request body</span></span>
<span data-ttu-id="4c17d-124">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md)-Objekt ein.</span><span class="sxs-lookup"><span data-stu-id="4c17d-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) object.</span></span>

<span data-ttu-id="4c17d-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="4c17d-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="4c17d-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4c17d-126">Property</span></span>|<span data-ttu-id="4c17d-127">Typ</span><span class="sxs-lookup"><span data-stu-id="4c17d-127">Type</span></span>|<span data-ttu-id="4c17d-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4c17d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c17d-129">displayName</span><span class="sxs-lookup"><span data-stu-id="4c17d-129">displayName</span></span>|<span data-ttu-id="4c17d-130">String</span><span class="sxs-lookup"><span data-stu-id="4c17d-130">String</span></span>|<span data-ttu-id="4c17d-131">Der Anzeigename</span><span class="sxs-lookup"><span data-stu-id="4c17d-131">The friendly name of the picture provider.</span></span>|
|<span data-ttu-id="4c17d-132">fileHash</span><span class="sxs-lookup"><span data-stu-id="4c17d-132">fileHash</span></span>|<span data-ttu-id="4c17d-133">String</span><span class="sxs-lookup"><span data-stu-id="4c17d-133">String</span></span>|<span data-ttu-id="4c17d-134">SHA256-Hash der Datei</span><span class="sxs-lookup"><span data-stu-id="4c17d-134">SHA256 hash of the file</span></span>|
|<span data-ttu-id="4c17d-135">file</span><span class="sxs-lookup"><span data-stu-id="4c17d-135">file</span></span>|<span data-ttu-id="4c17d-136">Binär</span><span class="sxs-lookup"><span data-stu-id="4c17d-136">Binary</span></span>|<span data-ttu-id="4c17d-137">Datei als Bytearray</span><span class="sxs-lookup"><span data-stu-id="4c17d-137">File as a byte array</span></span>|
|<span data-ttu-id="4c17d-138">id</span><span class="sxs-lookup"><span data-stu-id="4c17d-138">id</span></span>|<span data-ttu-id="4c17d-139">String</span><span class="sxs-lookup"><span data-stu-id="4c17d-139">String</span></span>|<span data-ttu-id="4c17d-140">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="4c17d-140">Key of the setting.</span></span>|
|<span data-ttu-id="4c17d-141">Version</span><span class="sxs-lookup"><span data-stu-id="4c17d-141">version</span></span>|<span data-ttu-id="4c17d-142">String</span><span class="sxs-lookup"><span data-stu-id="4c17d-142">String</span></span>|<span data-ttu-id="4c17d-143">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="4c17d-143">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="4c17d-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="4c17d-144">Response</span></span>
<span data-ttu-id="4c17d-145">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4c17d-145">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c17d-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4c17d-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="4c17d-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4c17d-147">Request</span></span>
<span data-ttu-id="4c17d-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4c17d-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
Content-type: application/json
Content-length: 131

{
  "displayName": "Display Name value",
  "fileHash": "File Hash value",
  "file": "ZmlsZQ==",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="4c17d-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="4c17d-149">Response</span></span>
<span data-ttu-id="4c17d-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4c17d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



