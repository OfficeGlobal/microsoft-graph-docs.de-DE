---
title: resourceOperation aktualisieren
description: Aktualisiert die Eigenschaften von Objekten des Typs resourceOperation.
ms.openlocfilehash: 0044d35577e42f8cd97bc80017ab89690fac110d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018159"
---
# <a name="update-resourceoperation"></a><span data-ttu-id="a8a2e-103">resourceOperation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a8a2e-103">Update resourceOperation</span></span>

> <span data-ttu-id="a8a2e-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a8a2e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8a2e-105">Aktualisiert die Eigenschaften von Objekten des Typs [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="a8a2e-105">Update the properties of a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a8a2e-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a8a2e-106">Prerequisites</span></span>
<span data-ttu-id="a8a2e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8a2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8a2e-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a8a2e-109">Permission type</span></span>|<span data-ttu-id="a8a2e-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a8a2e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8a2e-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a8a2e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a8a2e-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8a2e-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="a8a2e-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a8a2e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8a2e-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a8a2e-114">Not supported.</span></span>|
|<span data-ttu-id="a8a2e-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a8a2e-115">Application</span></span>|<span data-ttu-id="a8a2e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a8a2e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8a2e-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a8a2e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="a8a2e-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a8a2e-118">Request headers</span></span>
|<span data-ttu-id="a8a2e-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a8a2e-119">Header</span></span>|<span data-ttu-id="a8a2e-120">Wert</span><span class="sxs-lookup"><span data-stu-id="a8a2e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8a2e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8a2e-121">Authorization</span></span>|<span data-ttu-id="a8a2e-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a8a2e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8a2e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a8a2e-123">Accept</span></span>|<span data-ttu-id="a8a2e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a8a2e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8a2e-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a8a2e-125">Request body</span></span>
<span data-ttu-id="a8a2e-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [resourceOperation](../resources/intune-rbac-resourceoperation.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="a8a2e-126">In the request body, supply a JSON representation for the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

<span data-ttu-id="a8a2e-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [resourceOperation](../resources/intune-rbac-resourceoperation.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="a8a2e-127">The following table shows the properties that are required when you create the [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>

|<span data-ttu-id="a8a2e-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a8a2e-128">Property</span></span>|<span data-ttu-id="a8a2e-129">Typ</span><span class="sxs-lookup"><span data-stu-id="a8a2e-129">Type</span></span>|<span data-ttu-id="a8a2e-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a8a2e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8a2e-131">id</span><span class="sxs-lookup"><span data-stu-id="a8a2e-131">id</span></span>|<span data-ttu-id="a8a2e-132">String</span><span class="sxs-lookup"><span data-stu-id="a8a2e-132">String</span></span>|<span data-ttu-id="a8a2e-133">Schlüssel der Ressourcenoperation.</span><span class="sxs-lookup"><span data-stu-id="a8a2e-133">Key of the Resource Operation.</span></span> <span data-ttu-id="a8a2e-134">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="a8a2e-134">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="a8a2e-135">resourceName</span><span class="sxs-lookup"><span data-stu-id="a8a2e-135">resourceName</span></span>|<span data-ttu-id="a8a2e-136">String</span><span class="sxs-lookup"><span data-stu-id="a8a2e-136">String</span></span>|<span data-ttu-id="a8a2e-137">Name der Ressource, auf die die Operation angewendet wird</span><span class="sxs-lookup"><span data-stu-id="a8a2e-137">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="a8a2e-138">actionName</span><span class="sxs-lookup"><span data-stu-id="a8a2e-138">actionName</span></span>|<span data-ttu-id="a8a2e-139">String</span><span class="sxs-lookup"><span data-stu-id="a8a2e-139">String</span></span>|<span data-ttu-id="a8a2e-140">Typ von Aktion, den die Operation ausführen wird.</span><span class="sxs-lookup"><span data-stu-id="a8a2e-140">Type of action this operation is going to perform.</span></span> <span data-ttu-id="a8a2e-141">Der Wert für „actionName“ sollte prägnant sein und aus möglichst wenigen Wörtern bestehen.</span><span class="sxs-lookup"><span data-stu-id="a8a2e-141">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="a8a2e-142">description</span><span class="sxs-lookup"><span data-stu-id="a8a2e-142">description</span></span>|<span data-ttu-id="a8a2e-143">String</span><span class="sxs-lookup"><span data-stu-id="a8a2e-143">String</span></span>|<span data-ttu-id="a8a2e-144">Beschreibung der Ressourcenoperation.</span><span class="sxs-lookup"><span data-stu-id="a8a2e-144">Description of the resource operation.</span></span> <span data-ttu-id="a8a2e-145">Diese Beschreibung wird angezeigt, wenn der Benutzer im Azure-Portal den Mauszeiger auf der Operation platziert.</span><span class="sxs-lookup"><span data-stu-id="a8a2e-145">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="a8a2e-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="a8a2e-146">Response</span></span>
<span data-ttu-id="a8a2e-147">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [resourceOperation](../resources/intune-rbac-resourceoperation.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a8a2e-147">If successful, this method returns a `200 OK` response code and an updated [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8a2e-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a8a2e-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="a8a2e-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a8a2e-149">Request</span></span>
<span data-ttu-id="a8a2e-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a8a2e-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/resourceOperations/{resourceOperationId}
Content-type: application/json
Content-length: 178

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="a8a2e-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="a8a2e-151">Response</span></span>
<span data-ttu-id="a8a2e-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a8a2e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



