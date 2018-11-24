# <a name="update-roleassignment"></a><span data-ttu-id="61c79-101">roleAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="61c79-101">Update roleAssignment</span></span>

> <span data-ttu-id="61c79-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="61c79-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="61c79-103">Aktualisieren der Eigenschaften eines [roleAssignment](../resources/intune_rbac_roleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="61c79-103">Update the properties of a [roleAssignment](../resources/intune_rbac_roleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="61c79-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="61c79-104">Prerequisites</span></span>
<span data-ttu-id="61c79-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="61c79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="61c79-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="61c79-107">Permission type</span></span>|<span data-ttu-id="61c79-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="61c79-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61c79-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="61c79-109">Delegated (work or school account)</span></span>|<span data-ttu-id="61c79-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61c79-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="61c79-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="61c79-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61c79-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="61c79-112">Not supported.</span></span>|
|<span data-ttu-id="61c79-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="61c79-113">Application</span></span>|<span data-ttu-id="61c79-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="61c79-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="61c79-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="61c79-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="61c79-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="61c79-116">Request headers</span></span>
|<span data-ttu-id="61c79-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="61c79-117">Header</span></span>|<span data-ttu-id="61c79-118">Wert</span><span class="sxs-lookup"><span data-stu-id="61c79-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61c79-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="61c79-119">Authorization</span></span>|<span data-ttu-id="61c79-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="61c79-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61c79-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="61c79-121">Accept</span></span>|<span data-ttu-id="61c79-122">application/json</span><span class="sxs-lookup"><span data-stu-id="61c79-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61c79-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="61c79-123">Request body</span></span>
<span data-ttu-id="61c79-124">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [roleAssignment](../resources/intune_rbac_roleassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="61c79-124">In the request body, supply a JSON representation for the [roleAssignment](../resources/intune_rbac_roleassignment.md) object.</span></span>

<span data-ttu-id="61c79-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [roleAssignment](../resources/intune_rbac_roleassignment.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="61c79-125">The following table shows the properties that are required when you create the [roleAssignment](../resources/intune_rbac_roleassignment.md).</span></span>

|<span data-ttu-id="61c79-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="61c79-126">Property</span></span>|<span data-ttu-id="61c79-127">Typ</span><span class="sxs-lookup"><span data-stu-id="61c79-127">Type</span></span>|<span data-ttu-id="61c79-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="61c79-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61c79-129">id</span><span class="sxs-lookup"><span data-stu-id="61c79-129">id</span></span>|<span data-ttu-id="61c79-130">String</span><span class="sxs-lookup"><span data-stu-id="61c79-130">String</span></span>|<span data-ttu-id="61c79-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="61c79-131">Key of the entity.</span></span> <span data-ttu-id="61c79-132">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="61c79-132">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="61c79-133">displayName</span><span class="sxs-lookup"><span data-stu-id="61c79-133">displayName</span></span>|<span data-ttu-id="61c79-134">String</span><span class="sxs-lookup"><span data-stu-id="61c79-134">String</span></span>|<span data-ttu-id="61c79-135">Der Anzeigename der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="61c79-135">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="61c79-136">description</span><span class="sxs-lookup"><span data-stu-id="61c79-136">description</span></span>|<span data-ttu-id="61c79-137">String</span><span class="sxs-lookup"><span data-stu-id="61c79-137">String</span></span>|<span data-ttu-id="61c79-138">Beschreibung der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="61c79-138">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="61c79-139">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="61c79-139">resourceScopes</span></span>|<span data-ttu-id="61c79-140">String collection</span><span class="sxs-lookup"><span data-stu-id="61c79-140">String collection</span></span>|<span data-ttu-id="61c79-141">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="61c79-141">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="61c79-142">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="61c79-142">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="61c79-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="61c79-143">Response</span></span>
<span data-ttu-id="61c79-144">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [roleAssignment](../resources/intune_rbac_roleassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="61c79-144">If successful, this method returns a `200 OK` response code and an updated [roleAssignment](../resources/intune_rbac_roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61c79-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="61c79-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="61c79-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="61c79-146">Request</span></span>
<span data-ttu-id="61c79-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="61c79-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
Content-type: application/json
Content-length: 193

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="61c79-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="61c79-148">Response</span></span>
<span data-ttu-id="61c79-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="61c79-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 242

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "b3234d24-4d24-b323-244d-23b3244d23b3",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```



