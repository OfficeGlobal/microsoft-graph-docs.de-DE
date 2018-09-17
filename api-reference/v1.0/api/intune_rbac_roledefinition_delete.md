# <a name="delete-roledefinition"></a><span data-ttu-id="1c495-101">roleDefinition löschen</span><span class="sxs-lookup"><span data-stu-id="1c495-101">Delete roleDefinition</span></span>

> <span data-ttu-id="1c495-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1c495-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1c495-103">Löscht Objekte des Typs [roleDefinition](../resources/intune_rbac_roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="1c495-103">Deletes a [roleDefinition](../resources/intune_rbac_roledefinition.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1c495-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1c495-104">Prerequisites</span></span>
<span data-ttu-id="1c495-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1c495-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1c495-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1c495-107">Permission type</span></span>|<span data-ttu-id="1c495-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1c495-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c495-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1c495-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1c495-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c495-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="1c495-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1c495-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c495-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1c495-112">Not supported.</span></span>|
|<span data-ttu-id="1c495-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1c495-113">Application</span></span>|<span data-ttu-id="1c495-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1c495-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c495-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1c495-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/roleDefinitions/{roleDefinitionId}
DELETE /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="1c495-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1c495-116">Request headers</span></span>
|<span data-ttu-id="1c495-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1c495-117">Header</span></span>|<span data-ttu-id="1c495-118">Wert</span><span class="sxs-lookup"><span data-stu-id="1c495-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c495-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1c495-119">Authorization</span></span>|<span data-ttu-id="1c495-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1c495-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c495-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="1c495-121">Accept</span></span>|<span data-ttu-id="1c495-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="1c495-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c495-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1c495-123">Request body</span></span>
<span data-ttu-id="1c495-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1c495-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c495-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="1c495-125">Response</span></span>
<span data-ttu-id="1c495-126">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1c495-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1c495-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1c495-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="1c495-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1c495-128">Request</span></span>
<span data-ttu-id="1c495-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1c495-129">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}
```

### <a name="response"></a><span data-ttu-id="1c495-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="1c495-130">Response</span></span>
<span data-ttu-id="1c495-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1c495-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








