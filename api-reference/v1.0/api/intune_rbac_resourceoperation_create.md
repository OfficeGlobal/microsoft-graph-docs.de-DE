# <a name="create-resourceoperation"></a><span data-ttu-id="ab196-101">resourceOperation erstellen</span><span class="sxs-lookup"><span data-stu-id="ab196-101">Create resourceOperation</span></span>

> <span data-ttu-id="ab196-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ab196-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ab196-103">Erstellt neue Objekte des Typs [resourceOperation](../resources/intune_rbac_resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="ab196-103">Create a new [plannerBucket](../resources/intune_rbac_resourceoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ab196-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ab196-104">Prerequisites</span></span>
<span data-ttu-id="ab196-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ab196-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ab196-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ab196-107">Permission type</span></span>|<span data-ttu-id="ab196-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ab196-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab196-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ab196-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ab196-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab196-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="ab196-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ab196-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab196-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ab196-112">Not supported.</span></span>|
|<span data-ttu-id="ab196-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ab196-113">Application</span></span>|<span data-ttu-id="ab196-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ab196-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab196-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ab196-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="ab196-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ab196-116">Request headers</span></span>
|<span data-ttu-id="ab196-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ab196-117">Header</span></span>|<span data-ttu-id="ab196-118">Wert</span><span class="sxs-lookup"><span data-stu-id="ab196-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab196-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab196-119">Authorization</span></span>|<span data-ttu-id="ab196-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ab196-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ab196-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ab196-121">Accept</span></span>|<span data-ttu-id="ab196-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ab196-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab196-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ab196-123">Request body</span></span>
<span data-ttu-id="ab196-124">Geben Sie im Anforderungstext eine JSON-Darstellung des resourceOperation-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="ab196-124">In the request body, supply a JSON representation of TableRow object.</span></span>

<span data-ttu-id="ab196-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der resourceOperation erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="ab196-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="ab196-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ab196-126">Property</span></span>|<span data-ttu-id="ab196-127">Typ</span><span class="sxs-lookup"><span data-stu-id="ab196-127">Type</span></span>|<span data-ttu-id="ab196-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ab196-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab196-129">id</span><span class="sxs-lookup"><span data-stu-id="ab196-129">id</span></span>|<span data-ttu-id="ab196-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab196-130">String</span></span>|<span data-ttu-id="ab196-131">Schlüssel der Ressourcenoperation.</span><span class="sxs-lookup"><span data-stu-id="ab196-131">Key of the Resource Operation.</span></span> <span data-ttu-id="ab196-132">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="ab196-132">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="ab196-133">resourceName</span><span class="sxs-lookup"><span data-stu-id="ab196-133">resourceName</span></span>|<span data-ttu-id="ab196-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab196-134">String</span></span>|<span data-ttu-id="ab196-135">Name der Ressource, auf die die Operation angewendet wird</span><span class="sxs-lookup"><span data-stu-id="ab196-135">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="ab196-136">actionName</span><span class="sxs-lookup"><span data-stu-id="ab196-136">ActionName</span></span>|<span data-ttu-id="ab196-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab196-137">String</span></span>|<span data-ttu-id="ab196-138">Typ von Aktion, den die Operation ausführen wird.</span><span class="sxs-lookup"><span data-stu-id="ab196-138">Type of action this operation is going to perform.</span></span> <span data-ttu-id="ab196-139">Der Wert für „actionName“ sollte prägnant sein und aus möglichst wenigen Wörtern bestehen.</span><span class="sxs-lookup"><span data-stu-id="ab196-139">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="ab196-140">description</span><span class="sxs-lookup"><span data-stu-id="ab196-140">description</span></span>|<span data-ttu-id="ab196-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab196-141">String</span></span>|<span data-ttu-id="ab196-142">Beschreibung der Ressourcenoperation.</span><span class="sxs-lookup"><span data-stu-id="ab196-142">Description of the resource operation.</span></span> <span data-ttu-id="ab196-143">Diese Beschreibung wird angezeigt, wenn der Benutzer im Azure-Portal den Mauszeiger auf der Operation platziert.</span><span class="sxs-lookup"><span data-stu-id="ab196-143">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="ab196-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="ab196-144">Response</span></span>
<span data-ttu-id="ab196-145">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [resourceOperation](../resources/intune_rbac_resourceoperation.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ab196-145">If successful, this method returns a `201 Created` response code and [plannerBucketTaskBoardTaskFormat](../resources/intune_rbac_resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab196-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ab196-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="ab196-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ab196-147">Request</span></span>
<span data-ttu-id="ab196-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ab196-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/resourceOperations
Content-type: application/json
Content-length: 178

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="ab196-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="ab196-149">Response</span></span>
<span data-ttu-id="ab196-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ab196-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 227

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value"
}
```



