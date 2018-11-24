# <a name="create-deviceandappmanagementroleassignment"></a><span data-ttu-id="fd5b6-101">DeviceAndAppManagementRoleAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="fd5b6-101">Create deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="fd5b6-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fd5b6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fd5b6-103">Erstellen eines neuen [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="fd5b6-103">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fd5b6-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fd5b6-104">Prerequisites</span></span>
<span data-ttu-id="fd5b6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fd5b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fd5b6-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fd5b6-107">Permission type</span></span>|<span data-ttu-id="fd5b6-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fd5b6-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd5b6-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fd5b6-109">Delegated (work or school account)</span></span>|<span data-ttu-id="fd5b6-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd5b6-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="fd5b6-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fd5b6-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd5b6-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fd5b6-112">Not supported.</span></span>|
|<span data-ttu-id="fd5b6-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fd5b6-113">Application</span></span>|<span data-ttu-id="fd5b6-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fd5b6-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd5b6-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd5b6-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="fd5b6-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fd5b6-116">Request headers</span></span>
|<span data-ttu-id="fd5b6-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="fd5b6-117">Header</span></span>|<span data-ttu-id="fd5b6-118">Wert</span><span class="sxs-lookup"><span data-stu-id="fd5b6-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd5b6-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd5b6-119">Authorization</span></span>|<span data-ttu-id="fd5b6-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fd5b6-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd5b6-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fd5b6-121">Accept</span></span>|<span data-ttu-id="fd5b6-122">application/json</span><span class="sxs-lookup"><span data-stu-id="fd5b6-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd5b6-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fd5b6-123">Request body</span></span>
<span data-ttu-id="fd5b6-124">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs deviceAndAppManagementRoleAssignment an.</span><span class="sxs-lookup"><span data-stu-id="fd5b6-124">In the request body, supply a JSON representation for the deviceAndAppManagementRoleAssignment object.</span></span>

<span data-ttu-id="fd5b6-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceAndAppManagementRoleAssignment erstellen.</span><span class="sxs-lookup"><span data-stu-id="fd5b6-125">The following table shows the properties that are required when you create the deviceAndAppManagementRoleAssignment.</span></span>

|<span data-ttu-id="fd5b6-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fd5b6-126">Property</span></span>|<span data-ttu-id="fd5b6-127">Typ</span><span class="sxs-lookup"><span data-stu-id="fd5b6-127">Type</span></span>|<span data-ttu-id="fd5b6-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fd5b6-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd5b6-129">id</span><span class="sxs-lookup"><span data-stu-id="fd5b6-129">id</span></span>|<span data-ttu-id="fd5b6-130">String</span><span class="sxs-lookup"><span data-stu-id="fd5b6-130">String</span></span>|<span data-ttu-id="fd5b6-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="fd5b6-131">Key of the entity.</span></span> <span data-ttu-id="fd5b6-132">Dies ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="fd5b6-132">This is read-only and automatically generated.</span></span> <span data-ttu-id="fd5b6-133">Geerbt von [RoleAssignment](../resources/intune_rbac_roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="fd5b6-133">Inherited from [roleAssignment](../resources/intune_rbac_roleassignment.md)</span></span>|
|<span data-ttu-id="fd5b6-134">displayName</span><span class="sxs-lookup"><span data-stu-id="fd5b6-134">displayName</span></span>|<span data-ttu-id="fd5b6-135">String</span><span class="sxs-lookup"><span data-stu-id="fd5b6-135">String</span></span>|<span data-ttu-id="fd5b6-136">Der Anzeigename der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="fd5b6-136">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="fd5b6-137">Geerbt von [RoleAssignment](../resources/intune_rbac_roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="fd5b6-137">Inherited from [roleAssignment](../resources/intune_rbac_roleassignment.md)</span></span>|
|<span data-ttu-id="fd5b6-138">description</span><span class="sxs-lookup"><span data-stu-id="fd5b6-138">description</span></span>|<span data-ttu-id="fd5b6-139">String</span><span class="sxs-lookup"><span data-stu-id="fd5b6-139">String</span></span>|<span data-ttu-id="fd5b6-140">Beschreibung der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="fd5b6-140">Description of the Role Assignment.</span></span> <span data-ttu-id="fd5b6-141">Geerbt von [RoleAssignment](../resources/intune_rbac_roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="fd5b6-141">Inherited from [roleAssignment](../resources/intune_rbac_roleassignment.md)</span></span>|
|<span data-ttu-id="fd5b6-142">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="fd5b6-142">resourceScopes</span></span>|<span data-ttu-id="fd5b6-143">String collection</span><span class="sxs-lookup"><span data-stu-id="fd5b6-143">String collection</span></span>|<span data-ttu-id="fd5b6-144">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="fd5b6-144">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="fd5b6-145">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fd5b6-145">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="fd5b6-146">Geerbt von [RoleAssignment](../resources/intune_rbac_roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="fd5b6-146">Inherited from [roleAssignment](../resources/intune_rbac_roleassignment.md)</span></span>|
|<span data-ttu-id="fd5b6-147">Elemente</span><span class="sxs-lookup"><span data-stu-id="fd5b6-147">members</span></span>|<span data-ttu-id="fd5b6-148">String collection</span><span class="sxs-lookup"><span data-stu-id="fd5b6-148">String collection</span></span>|<span data-ttu-id="fd5b6-149">Die Liste der IDs der Rollenmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="fd5b6-149">The list of ids of role member security groups.</span></span> <span data-ttu-id="fd5b6-150">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fd5b6-150">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="fd5b6-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd5b6-151">Response</span></span>
<span data-ttu-id="fd5b6-152">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="fd5b6-152">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd5b6-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fd5b6-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="fd5b6-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd5b6-154">Request</span></span>
<span data-ttu-id="fd5b6-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fd5b6-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments
Content-type: application/json
Content-length: 258

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="fd5b6-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd5b6-156">Response</span></span>
<span data-ttu-id="fd5b6-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fd5b6-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 307

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```



