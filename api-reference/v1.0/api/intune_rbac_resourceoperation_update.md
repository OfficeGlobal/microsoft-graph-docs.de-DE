# <a name="update-resourceoperation"></a><span data-ttu-id="17ab8-101">resourceOperation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="17ab8-101">Update resourceOperation</span></span>

> <span data-ttu-id="17ab8-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="17ab8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="17ab8-103">Aktualisiert die Eigenschaften von Objekten des Typs [resourceOperation](../resources/intune_rbac_resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="17ab8-103">Update the properties of a [calendar](../resources/intune_rbac_resourceoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="17ab8-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="17ab8-104">Prerequisites</span></span>
<span data-ttu-id="17ab8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="17ab8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="17ab8-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="17ab8-107">Permission type</span></span>|<span data-ttu-id="17ab8-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="17ab8-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17ab8-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="17ab8-109">Delegated (work or school account)</span></span>|<span data-ttu-id="17ab8-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17ab8-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="17ab8-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="17ab8-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17ab8-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="17ab8-112">Not supported.</span></span>|
|<span data-ttu-id="17ab8-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="17ab8-113">Application</span></span>|<span data-ttu-id="17ab8-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="17ab8-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="17ab8-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="17ab8-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="17ab8-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="17ab8-116">Request headers</span></span>
|<span data-ttu-id="17ab8-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="17ab8-117">Header</span></span>|<span data-ttu-id="17ab8-118">Wert</span><span class="sxs-lookup"><span data-stu-id="17ab8-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17ab8-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="17ab8-119">Authorization</span></span>|<span data-ttu-id="17ab8-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="17ab8-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="17ab8-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="17ab8-121">Accept</span></span>|<span data-ttu-id="17ab8-122">application/json</span><span class="sxs-lookup"><span data-stu-id="17ab8-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17ab8-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="17ab8-123">Request body</span></span>
<span data-ttu-id="17ab8-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [resourceOperation](../resources/intune_rbac_resourceoperation.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="17ab8-124">In the request body, supply a JSON representation of [Attachment](../resources/intune_rbac_resourceoperation.md) object.</span></span>

<span data-ttu-id="17ab8-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [resourceOperation](../resources/intune_rbac_resourceoperation.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="17ab8-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="17ab8-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="17ab8-126">Property</span></span>|<span data-ttu-id="17ab8-127">Typ</span><span class="sxs-lookup"><span data-stu-id="17ab8-127">Type</span></span>|<span data-ttu-id="17ab8-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="17ab8-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17ab8-129">id</span><span class="sxs-lookup"><span data-stu-id="17ab8-129">id</span></span>|<span data-ttu-id="17ab8-130">String</span><span class="sxs-lookup"><span data-stu-id="17ab8-130">String</span></span>|<span data-ttu-id="17ab8-131">Schlüssel der Ressourcenoperation.</span><span class="sxs-lookup"><span data-stu-id="17ab8-131">Key of the Resource Operation.</span></span> <span data-ttu-id="17ab8-132">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="17ab8-132">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="17ab8-133">resourceName</span><span class="sxs-lookup"><span data-stu-id="17ab8-133">resourceName</span></span>|<span data-ttu-id="17ab8-134">String</span><span class="sxs-lookup"><span data-stu-id="17ab8-134">String</span></span>|<span data-ttu-id="17ab8-135">Name der Ressource, auf die die Operation angewendet wird</span><span class="sxs-lookup"><span data-stu-id="17ab8-135">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="17ab8-136">actionName</span><span class="sxs-lookup"><span data-stu-id="17ab8-136">ActionName</span></span>|<span data-ttu-id="17ab8-137">String</span><span class="sxs-lookup"><span data-stu-id="17ab8-137">String</span></span>|<span data-ttu-id="17ab8-138">Typ von Aktion, den die Operation ausführen wird.</span><span class="sxs-lookup"><span data-stu-id="17ab8-138">Type of action this operation is going to perform.</span></span> <span data-ttu-id="17ab8-139">Der Wert für „actionName“ sollte prägnant sein und aus möglichst wenigen Wörtern bestehen.</span><span class="sxs-lookup"><span data-stu-id="17ab8-139">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="17ab8-140">description</span><span class="sxs-lookup"><span data-stu-id="17ab8-140">description</span></span>|<span data-ttu-id="17ab8-141">String</span><span class="sxs-lookup"><span data-stu-id="17ab8-141">String</span></span>|<span data-ttu-id="17ab8-142">Beschreibung der Ressourcenoperation.</span><span class="sxs-lookup"><span data-stu-id="17ab8-142">Description of the resource operation.</span></span> <span data-ttu-id="17ab8-143">Diese Beschreibung wird angezeigt, wenn der Benutzer im Azure-Portal den Mauszeiger auf der Operation platziert.</span><span class="sxs-lookup"><span data-stu-id="17ab8-143">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="17ab8-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="17ab8-144">Response</span></span>
<span data-ttu-id="17ab8-145">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [resourceOperation](../resources/intune_rbac_resourceoperation.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="17ab8-145">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_rbac_resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17ab8-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="17ab8-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="17ab8-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="17ab8-147">Request</span></span>
<span data-ttu-id="17ab8-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="17ab8-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/resourceOperations/{resourceOperationId}
Content-type: application/json
Content-length: 122

{
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="17ab8-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="17ab8-149">Response</span></span>
<span data-ttu-id="17ab8-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="17ab8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



