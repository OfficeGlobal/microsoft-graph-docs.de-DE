# <a name="update-deviceandappmanagementroledefinition"></a><span data-ttu-id="7cd09-101">deviceAndAppManagementRoleDefinition aktualisieren</span><span class="sxs-lookup"><span data-stu-id="7cd09-101">Update deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="7cd09-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7cd09-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7cd09-103">Aktualisieren der Eigenschaften eines [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="7cd09-103">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7cd09-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7cd09-104">Prerequisites</span></span>
<span data-ttu-id="7cd09-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7cd09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7cd09-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7cd09-107">Permission type</span></span>|<span data-ttu-id="7cd09-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7cd09-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7cd09-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7cd09-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7cd09-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cd09-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="7cd09-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7cd09-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7cd09-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7cd09-112">Not supported.</span></span>|
|<span data-ttu-id="7cd09-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7cd09-113">Application</span></span>|<span data-ttu-id="7cd09-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7cd09-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7cd09-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7cd09-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="7cd09-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7cd09-116">Request headers</span></span>
|<span data-ttu-id="7cd09-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7cd09-117">Header</span></span>|<span data-ttu-id="7cd09-118">Wert</span><span class="sxs-lookup"><span data-stu-id="7cd09-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7cd09-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="7cd09-119">Authorization</span></span>|<span data-ttu-id="7cd09-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7cd09-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7cd09-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7cd09-121">Accept</span></span>|<span data-ttu-id="7cd09-122">application/json</span><span class="sxs-lookup"><span data-stu-id="7cd09-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7cd09-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7cd09-123">Request body</span></span>
<span data-ttu-id="7cd09-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="7cd09-124">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) object.</span></span>

<span data-ttu-id="7cd09-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="7cd09-125">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md).</span></span>

|<span data-ttu-id="7cd09-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7cd09-126">Property</span></span>|<span data-ttu-id="7cd09-127">Typ</span><span class="sxs-lookup"><span data-stu-id="7cd09-127">Type</span></span>|<span data-ttu-id="7cd09-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7cd09-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7cd09-129">id</span><span class="sxs-lookup"><span data-stu-id="7cd09-129">id</span></span>|<span data-ttu-id="7cd09-130">String</span><span class="sxs-lookup"><span data-stu-id="7cd09-130">String</span></span>|<span data-ttu-id="7cd09-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="7cd09-131">Key of the entity.</span></span> <span data-ttu-id="7cd09-132">Dies ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="7cd09-132">This is read-only and automatically generated.</span></span> <span data-ttu-id="7cd09-133">Geerbt von [roleDefinition](../resources/intune_rbac_roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7cd09-133">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|
|<span data-ttu-id="7cd09-134">displayName</span><span class="sxs-lookup"><span data-stu-id="7cd09-134">displayName</span></span>|<span data-ttu-id="7cd09-135">String</span><span class="sxs-lookup"><span data-stu-id="7cd09-135">String</span></span>|<span data-ttu-id="7cd09-136">Anzeigename der Rollendefinition.</span><span class="sxs-lookup"><span data-stu-id="7cd09-136">Display Name of the Role definition.</span></span> <span data-ttu-id="7cd09-137">Geerbt von [roleDefinition](../resources/intune_rbac_roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7cd09-137">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|
|<span data-ttu-id="7cd09-138">description</span><span class="sxs-lookup"><span data-stu-id="7cd09-138">description</span></span>|<span data-ttu-id="7cd09-139">String</span><span class="sxs-lookup"><span data-stu-id="7cd09-139">String</span></span>|<span data-ttu-id="7cd09-140">Beschreibung der Rollendefinition.</span><span class="sxs-lookup"><span data-stu-id="7cd09-140">Description of the Role definition.</span></span> <span data-ttu-id="7cd09-141">Geerbt von [roleDefinition](../resources/intune_rbac_roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7cd09-141">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|
|<span data-ttu-id="7cd09-142">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="7cd09-142">rolePermissions</span></span>|<span data-ttu-id="7cd09-143">Sammlung von Objekten des Typs [rolePermission](../resources/intune_rbac_rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="7cd09-143">[rolePermission](../resources/intune_rbac_rolepermission.md) collection</span></span>|<span data-ttu-id="7cd09-144">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="7cd09-144">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="7cd09-145">Diese müssen mit dem actionName übereinstimmen, der als Teil der rolePermission definiert ist.</span><span class="sxs-lookup"><span data-stu-id="7cd09-145">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="7cd09-146">Geerbt von [roleDefinition](../resources/intune_rbac_roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7cd09-146">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|
|<span data-ttu-id="7cd09-147">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="7cd09-147">isBuiltIn</span></span>|<span data-ttu-id="7cd09-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="7cd09-148">Boolean</span></span>|<span data-ttu-id="7cd09-149">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="7cd09-149">Type of Role.</span></span> <span data-ttu-id="7cd09-150">Wird auf „true“ festgelegt, wenn es sich um eine integrierte, oder auf „false“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="7cd09-150">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="7cd09-151">Geerbt von [roleDefinition](../resources/intune_rbac_roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7cd09-151">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="7cd09-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="7cd09-152">Response</span></span>
<span data-ttu-id="7cd09-153">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7cd09-153">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7cd09-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7cd09-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="7cd09-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7cd09-155">Request</span></span>
<span data-ttu-id="7cd09-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7cd09-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}
Content-type: application/json
Content-length: 602

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "displayName": "Display Name value",
  "description": "Description value",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="7cd09-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="7cd09-157">Response</span></span>
<span data-ttu-id="7cd09-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7cd09-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 651

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "id": "bca1dfb5-dfb5-bca1-b5df-a1bcb5dfa1bc",
  "displayName": "Display Name value",
  "description": "Description value",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "isBuiltIn": true
}
```



