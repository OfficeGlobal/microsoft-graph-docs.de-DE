# <a name="create-targetedmanagedapppolicyassignment"></a><span data-ttu-id="afbac-101">targetedManagedAppPolicyAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="afbac-101">Create targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="afbac-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="afbac-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="afbac-103">Erstellen eines neuen [TargetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="afbac-103">Create a new [plannerBucket](../resources/intune_mam_targetedmanagedapppolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="afbac-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="afbac-104">Prerequisites</span></span>
<span data-ttu-id="afbac-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="afbac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="afbac-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="afbac-107">Permission type</span></span>|<span data-ttu-id="afbac-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="afbac-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="afbac-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="afbac-109">Delegated (work or school account)</span></span>|<span data-ttu-id="afbac-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afbac-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="afbac-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="afbac-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="afbac-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="afbac-112">Not supported.</span></span>|
|<span data-ttu-id="afbac-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="afbac-113">Application</span></span>|<span data-ttu-id="afbac-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="afbac-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="afbac-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="afbac-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments
POST /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/assignments
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assignments
POST /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/assignments
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="afbac-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="afbac-116">Request headers</span></span>
|<span data-ttu-id="afbac-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="afbac-117">Header</span></span>|<span data-ttu-id="afbac-118">Wert</span><span class="sxs-lookup"><span data-stu-id="afbac-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="afbac-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="afbac-119">Authorization</span></span>|<span data-ttu-id="afbac-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="afbac-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="afbac-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="afbac-121">Accept</span></span>|<span data-ttu-id="afbac-122">application/json</span><span class="sxs-lookup"><span data-stu-id="afbac-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="afbac-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="afbac-123">Request body</span></span>
<span data-ttu-id="afbac-124">Geben Sie im Anforderungstext eine JSON-Darstellung des targetedManagedAppPolicyAssignment-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="afbac-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="afbac-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs targetedManagedAppPolicyAssignment erstellen.</span><span class="sxs-lookup"><span data-stu-id="afbac-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="afbac-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="afbac-126">Property</span></span>|<span data-ttu-id="afbac-127">Typ</span><span class="sxs-lookup"><span data-stu-id="afbac-127">Type</span></span>|<span data-ttu-id="afbac-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="afbac-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afbac-129">id</span><span class="sxs-lookup"><span data-stu-id="afbac-129">id</span></span>|<span data-ttu-id="afbac-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="afbac-130">String</span></span>|<span data-ttu-id="afbac-131">Id</span><span class="sxs-lookup"><span data-stu-id="afbac-131">Id</span></span>|
|<span data-ttu-id="afbac-132">target</span><span class="sxs-lookup"><span data-stu-id="afbac-132">target</span></span>|[<span data-ttu-id="afbac-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="afbac-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_mam_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="afbac-134">Bezeichner für die Bereitstellung einer Gruppe oder App</span><span class="sxs-lookup"><span data-stu-id="afbac-134">Identifier for deployment of a group or app</span></span>|



## <a name="response"></a><span data-ttu-id="afbac-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="afbac-135">Response</span></span>
<span data-ttu-id="afbac-136">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="afbac-136">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_mam_targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afbac-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="afbac-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="afbac-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="afbac-138">Request</span></span>
<span data-ttu-id="afbac-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="afbac-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments
Content-type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="afbac-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="afbac-140">Response</span></span>
<span data-ttu-id="afbac-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="afbac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 223

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



