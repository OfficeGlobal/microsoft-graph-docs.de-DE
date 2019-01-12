---
title: resourceOperation aktualisieren
description: Aktualisiert die Eigenschaften von Objekten des Typs resourceOperation.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b5d65fb9394ba1bf33ce657941f2807d3dda44a4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919064"
---
# <a name="update-resourceoperation"></a><span data-ttu-id="7a80e-103">resourceOperation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="7a80e-103">Update resourceOperation</span></span>

> <span data-ttu-id="7a80e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7a80e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7a80e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7a80e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7a80e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7a80e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7a80e-107">Aktualisiert die Eigenschaften von Objekten des Typs [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="7a80e-107">Update the properties of a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7a80e-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7a80e-108">Prerequisites</span></span>
<span data-ttu-id="7a80e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a80e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a80e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7a80e-111">Permission type</span></span>|<span data-ttu-id="7a80e-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7a80e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a80e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7a80e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7a80e-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a80e-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="7a80e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7a80e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a80e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7a80e-116">Not supported.</span></span>|
|<span data-ttu-id="7a80e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7a80e-117">Application</span></span>|<span data-ttu-id="7a80e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7a80e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a80e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7a80e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="7a80e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7a80e-120">Request headers</span></span>
|<span data-ttu-id="7a80e-121">Header</span><span class="sxs-lookup"><span data-stu-id="7a80e-121">Header</span></span>|<span data-ttu-id="7a80e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="7a80e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a80e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a80e-123">Authorization</span></span>|<span data-ttu-id="7a80e-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7a80e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a80e-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7a80e-125">Accept</span></span>|<span data-ttu-id="7a80e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7a80e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a80e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7a80e-127">Request body</span></span>
<span data-ttu-id="7a80e-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [resourceOperation](../resources/intune-rbac-resourceoperation.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="7a80e-128">In the request body, supply a JSON representation for the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

<span data-ttu-id="7a80e-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [resourceOperation](../resources/intune-rbac-resourceoperation.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="7a80e-129">The following table shows the properties that are required when you create the [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>

|<span data-ttu-id="7a80e-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7a80e-130">Property</span></span>|<span data-ttu-id="7a80e-131">Typ</span><span class="sxs-lookup"><span data-stu-id="7a80e-131">Type</span></span>|<span data-ttu-id="7a80e-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7a80e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a80e-133">id</span><span class="sxs-lookup"><span data-stu-id="7a80e-133">id</span></span>|<span data-ttu-id="7a80e-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7a80e-134">String</span></span>|<span data-ttu-id="7a80e-135">Schlüssel der Ressourcenoperation.</span><span class="sxs-lookup"><span data-stu-id="7a80e-135">Key of the Resource Operation.</span></span> <span data-ttu-id="7a80e-136">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="7a80e-136">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="7a80e-137">resource</span><span class="sxs-lookup"><span data-stu-id="7a80e-137">resource</span></span>|<span data-ttu-id="7a80e-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7a80e-138">String</span></span>|<span data-ttu-id="7a80e-139">Resource-Kategorie, zu dem dieser Vorgang gehört.</span><span class="sxs-lookup"><span data-stu-id="7a80e-139">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="7a80e-140">resourceName</span><span class="sxs-lookup"><span data-stu-id="7a80e-140">resourceName</span></span>|<span data-ttu-id="7a80e-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7a80e-141">String</span></span>|<span data-ttu-id="7a80e-142">Name der Ressource, auf die die Operation angewendet wird</span><span class="sxs-lookup"><span data-stu-id="7a80e-142">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="7a80e-143">actionName</span><span class="sxs-lookup"><span data-stu-id="7a80e-143">actionName</span></span>|<span data-ttu-id="7a80e-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7a80e-144">String</span></span>|<span data-ttu-id="7a80e-145">Typ von Aktion, den die Operation ausführen wird.</span><span class="sxs-lookup"><span data-stu-id="7a80e-145">Type of action this operation is going to perform.</span></span> <span data-ttu-id="7a80e-146">Der Wert für „actionName“ sollte prägnant sein und aus möglichst wenigen Wörtern bestehen.</span><span class="sxs-lookup"><span data-stu-id="7a80e-146">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="7a80e-147">description</span><span class="sxs-lookup"><span data-stu-id="7a80e-147">description</span></span>|<span data-ttu-id="7a80e-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7a80e-148">String</span></span>|<span data-ttu-id="7a80e-149">Beschreibung der Ressourcenoperation.</span><span class="sxs-lookup"><span data-stu-id="7a80e-149">Description of the resource operation.</span></span> <span data-ttu-id="7a80e-150">Diese Beschreibung wird angezeigt, wenn der Benutzer im Azure-Portal den Mauszeiger auf der Operation platziert.</span><span class="sxs-lookup"><span data-stu-id="7a80e-150">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="7a80e-151">enabledForScopeValidation</span><span class="sxs-lookup"><span data-stu-id="7a80e-151">enabledForScopeValidation</span></span>|<span data-ttu-id="7a80e-152">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7a80e-152">Boolean</span></span>|<span data-ttu-id="7a80e-153">Bestimmt, ob die Berechtigung für pro Rollenzuweisung definierten Bereiche nicht überprüft wird.</span><span class="sxs-lookup"><span data-stu-id="7a80e-153">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="7a80e-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="7a80e-154">Response</span></span>
<span data-ttu-id="7a80e-155">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [resourceOperation](../resources/intune-rbac-resourceoperation.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7a80e-155">If successful, this method returns a `200 OK` response code and an updated [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a80e-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7a80e-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="7a80e-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7a80e-157">Request</span></span>
<span data-ttu-id="7a80e-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7a80e-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/resourceOperations/{resourceOperationId}
Content-type: application/json
Content-length: 193

{
  "resource": "Resource value",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value",
  "enabledForScopeValidation": true
}
```

### <a name="response"></a><span data-ttu-id="7a80e-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="7a80e-159">Response</span></span>
<span data-ttu-id="7a80e-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7a80e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 298

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
  "resource": "Resource value",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value",
  "enabledForScopeValidation": true
}
```





