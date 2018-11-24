# <a name="create-resourceoperation"></a><span data-ttu-id="e955e-101">resourceOperation erstellen</span><span class="sxs-lookup"><span data-stu-id="e955e-101">Create resourceOperation</span></span>

> <span data-ttu-id="e955e-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e955e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e955e-103">Erstellt neue Objekte des Typs [resourceOperation](../resources/intune_rbac_resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="e955e-103">Create a new [resourceOperation](../resources/intune_rbac_resourceoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e955e-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e955e-104">Prerequisites</span></span>
<span data-ttu-id="e955e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e955e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e955e-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e955e-107">Permission type</span></span>|<span data-ttu-id="e955e-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e955e-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e955e-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e955e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e955e-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e955e-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="e955e-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e955e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e955e-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e955e-112">Not supported.</span></span>|
|<span data-ttu-id="e955e-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e955e-113">Application</span></span>|<span data-ttu-id="e955e-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e955e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e955e-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e955e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="e955e-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e955e-116">Request headers</span></span>
|<span data-ttu-id="e955e-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e955e-117">Header</span></span>|<span data-ttu-id="e955e-118">Wert</span><span class="sxs-lookup"><span data-stu-id="e955e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e955e-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="e955e-119">Authorization</span></span>|<span data-ttu-id="e955e-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e955e-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e955e-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e955e-121">Accept</span></span>|<span data-ttu-id="e955e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e955e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e955e-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e955e-123">Request body</span></span>
<span data-ttu-id="e955e-124">Geben Sie im Anforderungstext eine JSON-Darstellung des resourceOperation-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="e955e-124">In the request body, supply a JSON representation for the resourceOperation object.</span></span>

<span data-ttu-id="e955e-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der resourceOperation erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="e955e-125">The following table shows the properties that are required when you create the resourceOperation.</span></span>

|<span data-ttu-id="e955e-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e955e-126">Property</span></span>|<span data-ttu-id="e955e-127">Typ</span><span class="sxs-lookup"><span data-stu-id="e955e-127">Type</span></span>|<span data-ttu-id="e955e-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e955e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e955e-129">id</span><span class="sxs-lookup"><span data-stu-id="e955e-129">id</span></span>|<span data-ttu-id="e955e-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e955e-130">String</span></span>|<span data-ttu-id="e955e-131">Schlüssel der Ressourcenoperation.</span><span class="sxs-lookup"><span data-stu-id="e955e-131">Key of the Resource Operation.</span></span> <span data-ttu-id="e955e-132">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="e955e-132">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="e955e-133">resourceName</span><span class="sxs-lookup"><span data-stu-id="e955e-133">resourceName</span></span>|<span data-ttu-id="e955e-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e955e-134">String</span></span>|<span data-ttu-id="e955e-135">Name der Ressource, auf die die Operation angewendet wird</span><span class="sxs-lookup"><span data-stu-id="e955e-135">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="e955e-136">actionName</span><span class="sxs-lookup"><span data-stu-id="e955e-136">actionName</span></span>|<span data-ttu-id="e955e-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e955e-137">String</span></span>|<span data-ttu-id="e955e-138">Typ von Aktion, den die Operation ausführen wird.</span><span class="sxs-lookup"><span data-stu-id="e955e-138">Type of action this operation is going to perform.</span></span> <span data-ttu-id="e955e-139">Der Wert für „actionName“ sollte prägnant sein und aus möglichst wenigen Wörtern bestehen.</span><span class="sxs-lookup"><span data-stu-id="e955e-139">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="e955e-140">description</span><span class="sxs-lookup"><span data-stu-id="e955e-140">description</span></span>|<span data-ttu-id="e955e-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e955e-141">String</span></span>|<span data-ttu-id="e955e-142">Beschreibung der Ressourcenoperation.</span><span class="sxs-lookup"><span data-stu-id="e955e-142">Description of the resource operation.</span></span> <span data-ttu-id="e955e-143">Diese Beschreibung wird angezeigt, wenn der Benutzer im Azure-Portal den Mauszeiger auf der Operation platziert.</span><span class="sxs-lookup"><span data-stu-id="e955e-143">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="e955e-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="e955e-144">Response</span></span>
<span data-ttu-id="e955e-145">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [resourceOperation](../resources/intune_rbac_resourceoperation.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e955e-145">If successful, this method returns a `201 Created` response code and a [resourceOperation](../resources/intune_rbac_resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e955e-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e955e-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="e955e-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e955e-147">Request</span></span>
<span data-ttu-id="e955e-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e955e-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e955e-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="e955e-149">Response</span></span>
<span data-ttu-id="e955e-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e955e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



