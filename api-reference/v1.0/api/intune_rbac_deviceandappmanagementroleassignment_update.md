# <a name="update-deviceandappmanagementroleassignment"></a><span data-ttu-id="8e081-101">DeviceAndAppManagementRoleAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="8e081-101">Update deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="8e081-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8e081-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e081-103">Aktualisieren der Eigenschaften eines [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8e081-103">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8e081-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8e081-104">Prerequisites</span></span>
<span data-ttu-id="8e081-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8e081-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8e081-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8e081-107">Permission type</span></span>|<span data-ttu-id="8e081-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8e081-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e081-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8e081-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8e081-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e081-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="8e081-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8e081-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e081-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8e081-112">Not supported.</span></span>|
|<span data-ttu-id="8e081-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8e081-113">Application</span></span>|<span data-ttu-id="8e081-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8e081-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e081-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8e081-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="8e081-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8e081-116">Request headers</span></span>
|<span data-ttu-id="8e081-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8e081-117">Header</span></span>|<span data-ttu-id="8e081-118">Wert</span><span class="sxs-lookup"><span data-stu-id="8e081-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e081-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="8e081-119">Authorization</span></span>|<span data-ttu-id="8e081-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8e081-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e081-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="8e081-121">Accept</span></span>|<span data-ttu-id="8e081-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="8e081-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e081-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8e081-123">Request body</span></span>
<span data-ttu-id="8e081-124">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="8e081-124">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) object.</span></span>

<span data-ttu-id="8e081-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="8e081-125">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md).</span></span>

|<span data-ttu-id="8e081-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8e081-126">Property</span></span>|<span data-ttu-id="8e081-127">Typ</span><span class="sxs-lookup"><span data-stu-id="8e081-127">Type</span></span>|<span data-ttu-id="8e081-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8e081-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e081-129">ID</span><span class="sxs-lookup"><span data-stu-id="8e081-129">id</span></span>|<span data-ttu-id="8e081-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8e081-130">String</span></span>|<span data-ttu-id="8e081-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8e081-131">Key of the entity.</span></span> <span data-ttu-id="8e081-132">Dies ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="8e081-132">This is read-only and automatically generated.</span></span> <span data-ttu-id="8e081-133">Geerbt von [RoleAssignment](../resources/intune_rbac_roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8e081-133">Inherited from [roleAssignment](../resources/intune_rbac_roleassignment.md)</span></span>|
|<span data-ttu-id="8e081-134">displayName</span><span class="sxs-lookup"><span data-stu-id="8e081-134">displayName</span></span>|<span data-ttu-id="8e081-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8e081-135">String</span></span>|<span data-ttu-id="8e081-136">Der Anzeigename der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="8e081-136">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="8e081-137">Geerbt von [RoleAssignment](../resources/intune_rbac_roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8e081-137">Inherited from [roleAssignment](../resources/intune_rbac_roleassignment.md)</span></span>|
|<span data-ttu-id="8e081-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8e081-138">description</span></span>|<span data-ttu-id="8e081-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8e081-139">String</span></span>|<span data-ttu-id="8e081-140">Beschreibung der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="8e081-140">Description of the Role Assignment.</span></span> <span data-ttu-id="8e081-141">Geerbt von [RoleAssignment](../resources/intune_rbac_roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8e081-141">Inherited from [roleAssignment](../resources/intune_rbac_roleassignment.md)</span></span>|
|<span data-ttu-id="8e081-142">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="8e081-142">resourceScopes</span></span>|<span data-ttu-id="8e081-143">Zeichenfolgen-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8e081-143">String collection</span></span>|<span data-ttu-id="8e081-144">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="8e081-144">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="8e081-145">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8e081-145">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="8e081-146">Geerbt von [RoleAssignment](../resources/intune_rbac_roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8e081-146">Inherited from [roleAssignment](../resources/intune_rbac_roleassignment.md)</span></span>|
|<span data-ttu-id="8e081-147">Elemente</span><span class="sxs-lookup"><span data-stu-id="8e081-147">members</span></span>|<span data-ttu-id="8e081-148">Zeichenfolgen-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8e081-148">String collection</span></span>|<span data-ttu-id="8e081-149">Die Liste der IDs der Rollenmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="8e081-149">The list of ids of role member security groups.</span></span> <span data-ttu-id="8e081-150">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8e081-150">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="8e081-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="8e081-151">Response</span></span>
<span data-ttu-id="8e081-152">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8e081-152">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e081-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8e081-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="8e081-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8e081-154">Request</span></span>
<span data-ttu-id="8e081-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8e081-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
Content-type: application/json
Content-length: 183

{
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

### <a name="response"></a><span data-ttu-id="8e081-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="8e081-156">Response</span></span>
<span data-ttu-id="8e081-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8e081-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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








