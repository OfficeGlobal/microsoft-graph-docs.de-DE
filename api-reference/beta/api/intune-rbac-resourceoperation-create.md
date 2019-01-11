---
title: resourceOperation erstellen
description: Erstellt neue Objekte des Typs resourceOperation.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ea0a77b56cbbfd68a7886e220b29222b794cf932
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862601"
---
# <a name="create-resourceoperation"></a><span data-ttu-id="31dc1-103">resourceOperation erstellen</span><span class="sxs-lookup"><span data-stu-id="31dc1-103">Create resourceOperation</span></span>

> <span data-ttu-id="31dc1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="31dc1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31dc1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="31dc1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="31dc1-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="31dc1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="31dc1-107">Erstellt neue Objekte des Typs [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="31dc1-107">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="31dc1-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="31dc1-108">Prerequisites</span></span>
<span data-ttu-id="31dc1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31dc1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31dc1-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="31dc1-111">Permission type</span></span>|<span data-ttu-id="31dc1-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="31dc1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31dc1-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="31dc1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="31dc1-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31dc1-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="31dc1-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="31dc1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31dc1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="31dc1-116">Not supported.</span></span>|
|<span data-ttu-id="31dc1-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="31dc1-117">Application</span></span>|<span data-ttu-id="31dc1-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="31dc1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="31dc1-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="31dc1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="31dc1-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="31dc1-120">Request headers</span></span>
|<span data-ttu-id="31dc1-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="31dc1-121">Header</span></span>|<span data-ttu-id="31dc1-122">Wert</span><span class="sxs-lookup"><span data-stu-id="31dc1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31dc1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="31dc1-123">Authorization</span></span>|<span data-ttu-id="31dc1-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="31dc1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31dc1-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="31dc1-125">Accept</span></span>|<span data-ttu-id="31dc1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="31dc1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31dc1-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="31dc1-127">Request body</span></span>
<span data-ttu-id="31dc1-128">Geben Sie im Anforderungstext eine JSON-Darstellung des resourceOperation-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="31dc1-128">In the request body, supply a JSON representation for the resourceOperation object.</span></span>

<span data-ttu-id="31dc1-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der resourceOperation erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="31dc1-129">The following table shows the properties that are required when you create the resourceOperation.</span></span>

|<span data-ttu-id="31dc1-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="31dc1-130">Property</span></span>|<span data-ttu-id="31dc1-131">Typ</span><span class="sxs-lookup"><span data-stu-id="31dc1-131">Type</span></span>|<span data-ttu-id="31dc1-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="31dc1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31dc1-133">id</span><span class="sxs-lookup"><span data-stu-id="31dc1-133">id</span></span>|<span data-ttu-id="31dc1-134">String</span><span class="sxs-lookup"><span data-stu-id="31dc1-134">String</span></span>|<span data-ttu-id="31dc1-135">Schlüssel der Ressourcenoperation.</span><span class="sxs-lookup"><span data-stu-id="31dc1-135">Key of the Resource Operation.</span></span> <span data-ttu-id="31dc1-136">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="31dc1-136">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="31dc1-137">resource</span><span class="sxs-lookup"><span data-stu-id="31dc1-137">resource</span></span>|<span data-ttu-id="31dc1-138">String</span><span class="sxs-lookup"><span data-stu-id="31dc1-138">String</span></span>|<span data-ttu-id="31dc1-139">Resource-Kategorie, zu dem dieser Vorgang gehört.</span><span class="sxs-lookup"><span data-stu-id="31dc1-139">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="31dc1-140">resourceName</span><span class="sxs-lookup"><span data-stu-id="31dc1-140">resourceName</span></span>|<span data-ttu-id="31dc1-141">String</span><span class="sxs-lookup"><span data-stu-id="31dc1-141">String</span></span>|<span data-ttu-id="31dc1-142">Name der Ressource, auf die die Operation angewendet wird</span><span class="sxs-lookup"><span data-stu-id="31dc1-142">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="31dc1-143">actionName</span><span class="sxs-lookup"><span data-stu-id="31dc1-143">actionName</span></span>|<span data-ttu-id="31dc1-144">String</span><span class="sxs-lookup"><span data-stu-id="31dc1-144">String</span></span>|<span data-ttu-id="31dc1-145">Typ von Aktion, den die Operation ausführen wird.</span><span class="sxs-lookup"><span data-stu-id="31dc1-145">Type of action this operation is going to perform.</span></span> <span data-ttu-id="31dc1-146">Der Wert für „actionName“ sollte prägnant sein und aus möglichst wenigen Wörtern bestehen.</span><span class="sxs-lookup"><span data-stu-id="31dc1-146">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="31dc1-147">description</span><span class="sxs-lookup"><span data-stu-id="31dc1-147">description</span></span>|<span data-ttu-id="31dc1-148">String</span><span class="sxs-lookup"><span data-stu-id="31dc1-148">String</span></span>|<span data-ttu-id="31dc1-149">Beschreibung der Ressourcenoperation.</span><span class="sxs-lookup"><span data-stu-id="31dc1-149">Description of the resource operation.</span></span> <span data-ttu-id="31dc1-150">Diese Beschreibung wird angezeigt, wenn der Benutzer im Azure-Portal den Mauszeiger auf der Operation platziert.</span><span class="sxs-lookup"><span data-stu-id="31dc1-150">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="31dc1-151">enabledForScopeValidation</span><span class="sxs-lookup"><span data-stu-id="31dc1-151">enabledForScopeValidation</span></span>|<span data-ttu-id="31dc1-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="31dc1-152">Boolean</span></span>|<span data-ttu-id="31dc1-153">Bestimmt, ob die Berechtigung für pro Rollenzuweisung definierten Bereiche nicht überprüft wird.</span><span class="sxs-lookup"><span data-stu-id="31dc1-153">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="31dc1-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="31dc1-154">Response</span></span>
<span data-ttu-id="31dc1-155">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [resourceOperation](../resources/intune-rbac-resourceoperation.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="31dc1-155">If successful, this method returns a `201 Created` response code and a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31dc1-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="31dc1-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="31dc1-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="31dc1-157">Request</span></span>
<span data-ttu-id="31dc1-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="31dc1-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/resourceOperations
Content-type: application/json
Content-length: 249

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "resource": "Resource value",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value",
  "enabledForScopeValidation": true
}
```

### <a name="response"></a><span data-ttu-id="31dc1-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="31dc1-159">Response</span></span>
<span data-ttu-id="31dc1-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="31dc1-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





