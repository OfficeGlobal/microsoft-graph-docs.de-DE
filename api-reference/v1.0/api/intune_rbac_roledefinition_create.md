# <a name="create-roledefinition"></a><span data-ttu-id="5af6b-101">roleDefinition erstellen</span><span class="sxs-lookup"><span data-stu-id="5af6b-101">Create roleDefinition</span></span>

> <span data-ttu-id="5af6b-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5af6b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5af6b-103">Erstellt neue Objekte des Typs [roleDefinition](../resources/intune_rbac_roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5af6b-103">Create a new [plannerBucket](../resources/intune_rbac_roledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5af6b-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5af6b-104">Prerequisites</span></span>
<span data-ttu-id="5af6b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5af6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5af6b-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5af6b-107">Permission type</span></span>|<span data-ttu-id="5af6b-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5af6b-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5af6b-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5af6b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5af6b-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5af6b-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="5af6b-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5af6b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5af6b-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5af6b-112">Not supported.</span></span>|
|<span data-ttu-id="5af6b-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5af6b-113">Application</span></span>|<span data-ttu-id="5af6b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5af6b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5af6b-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5af6b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="5af6b-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5af6b-116">Request headers</span></span>
|<span data-ttu-id="5af6b-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5af6b-117">Header</span></span>|<span data-ttu-id="5af6b-118">Wert</span><span class="sxs-lookup"><span data-stu-id="5af6b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5af6b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="5af6b-119">Authorization</span></span>|<span data-ttu-id="5af6b-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5af6b-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5af6b-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5af6b-121">Accept</span></span>|<span data-ttu-id="5af6b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5af6b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5af6b-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5af6b-123">Request body</span></span>
<span data-ttu-id="5af6b-124">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs roleDefinition an.</span><span class="sxs-lookup"><span data-stu-id="5af6b-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="5af6b-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der roleDefinition erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="5af6b-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="5af6b-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5af6b-126">Property</span></span>|<span data-ttu-id="5af6b-127">Typ</span><span class="sxs-lookup"><span data-stu-id="5af6b-127">Type</span></span>|<span data-ttu-id="5af6b-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5af6b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5af6b-129">id</span><span class="sxs-lookup"><span data-stu-id="5af6b-129">id</span></span>|<span data-ttu-id="5af6b-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5af6b-130">String</span></span>|<span data-ttu-id="5af6b-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="5af6b-131">Key of the setting.</span></span> <span data-ttu-id="5af6b-132">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="5af6b-132">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="5af6b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="5af6b-133">displayName</span></span>|<span data-ttu-id="5af6b-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5af6b-134">String</span></span>|<span data-ttu-id="5af6b-135">Anzeigename der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="5af6b-135">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="5af6b-136">description</span><span class="sxs-lookup"><span data-stu-id="5af6b-136">description</span></span>|<span data-ttu-id="5af6b-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5af6b-137">String</span></span>|<span data-ttu-id="5af6b-138">Beschreibung der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="5af6b-138">Description of the Role definition.</span></span>|
|<span data-ttu-id="5af6b-139">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="5af6b-139">rolePermissions</span></span>|<span data-ttu-id="5af6b-140">Sammlung von Objekten des Typs [rolePermission](../resources/intune_rbac_rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="5af6b-140">[rolePermission](../resources/intune_rbac_rolepermission.md) collection</span></span>|<span data-ttu-id="5af6b-141">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="5af6b-141">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="5af6b-142">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="5af6b-142">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="5af6b-143">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="5af6b-143">isBuiltIn</span></span>|<span data-ttu-id="5af6b-144">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="5af6b-144">Boolean</span></span>|<span data-ttu-id="5af6b-145">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="5af6b-145">Type of Role.</span></span> <span data-ttu-id="5af6b-146">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="5af6b-146">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|



## <a name="response"></a><span data-ttu-id="5af6b-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="5af6b-147">Response</span></span>
<span data-ttu-id="5af6b-148">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [roleDefinition](../resources/intune_rbac_roledefinition.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5af6b-148">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_rbac_roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5af6b-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5af6b-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="5af6b-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5af6b-150">Request</span></span>
<span data-ttu-id="5af6b-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5af6b-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions
Content-type: application/json
Content-length: 580

{
  "@odata.type": "#microsoft.graph.roleDefinition",
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

### <a name="response"></a><span data-ttu-id="5af6b-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="5af6b-152">Response</span></span>
<span data-ttu-id="5af6b-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5af6b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 629

{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "id": "70fdcd08-cd08-70fd-08cd-fd7008cdfd70",
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



