---
title: resourceOperation aktualisieren
description: Aktualisiert die Eigenschaften von Objekten des Typs resourceOperation.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 266d45150c5633a66c5996b5cb9285f97ecaf6bb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411141"
---
# <a name="update-resourceoperation"></a><span data-ttu-id="f5381-103">resourceOperation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f5381-103">Update resourceOperation</span></span>

> <span data-ttu-id="f5381-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="f5381-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f5381-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f5381-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f5381-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f5381-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5381-107">Aktualisiert die Eigenschaften von Objekten des Typs [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="f5381-107">Update the properties of a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f5381-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f5381-108">Prerequisites</span></span>
<span data-ttu-id="f5381-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f5381-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f5381-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f5381-111">Permission type</span></span>|<span data-ttu-id="f5381-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f5381-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5381-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f5381-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f5381-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5381-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="f5381-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f5381-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5381-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f5381-116">Not supported.</span></span>|
|<span data-ttu-id="f5381-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f5381-117">Application</span></span>|<span data-ttu-id="f5381-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f5381-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5381-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f5381-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="f5381-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f5381-120">Request headers</span></span>
|<span data-ttu-id="f5381-121">Header</span><span class="sxs-lookup"><span data-stu-id="f5381-121">Header</span></span>|<span data-ttu-id="f5381-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f5381-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5381-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f5381-123">Authorization</span></span>|<span data-ttu-id="f5381-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f5381-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5381-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f5381-125">Accept</span></span>|<span data-ttu-id="f5381-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f5381-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5381-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f5381-127">Request body</span></span>
<span data-ttu-id="f5381-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [resourceOperation](../resources/intune-rbac-resourceoperation.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="f5381-128">In the request body, supply a JSON representation for the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

<span data-ttu-id="f5381-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [resourceOperation](../resources/intune-rbac-resourceoperation.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="f5381-129">The following table shows the properties that are required when you create the [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>

|<span data-ttu-id="f5381-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f5381-130">Property</span></span>|<span data-ttu-id="f5381-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f5381-131">Type</span></span>|<span data-ttu-id="f5381-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f5381-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5381-133">id</span><span class="sxs-lookup"><span data-stu-id="f5381-133">id</span></span>|<span data-ttu-id="f5381-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f5381-134">String</span></span>|<span data-ttu-id="f5381-135">Schlüssel der Ressourcenoperation.</span><span class="sxs-lookup"><span data-stu-id="f5381-135">Key of the Resource Operation.</span></span> <span data-ttu-id="f5381-136">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="f5381-136">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="f5381-137">resource</span><span class="sxs-lookup"><span data-stu-id="f5381-137">resource</span></span>|<span data-ttu-id="f5381-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f5381-138">String</span></span>|<span data-ttu-id="f5381-139">Resource-Kategorie, zu dem dieser Vorgang gehört.</span><span class="sxs-lookup"><span data-stu-id="f5381-139">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="f5381-140">resourceName</span><span class="sxs-lookup"><span data-stu-id="f5381-140">resourceName</span></span>|<span data-ttu-id="f5381-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f5381-141">String</span></span>|<span data-ttu-id="f5381-142">Name der Ressource, auf die die Operation angewendet wird</span><span class="sxs-lookup"><span data-stu-id="f5381-142">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="f5381-143">actionName</span><span class="sxs-lookup"><span data-stu-id="f5381-143">actionName</span></span>|<span data-ttu-id="f5381-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f5381-144">String</span></span>|<span data-ttu-id="f5381-145">Typ von Aktion, den die Operation ausführen wird.</span><span class="sxs-lookup"><span data-stu-id="f5381-145">Type of action this operation is going to perform.</span></span> <span data-ttu-id="f5381-146">Der Wert für „actionName“ sollte prägnant sein und aus möglichst wenigen Wörtern bestehen.</span><span class="sxs-lookup"><span data-stu-id="f5381-146">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="f5381-147">description</span><span class="sxs-lookup"><span data-stu-id="f5381-147">description</span></span>|<span data-ttu-id="f5381-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f5381-148">String</span></span>|<span data-ttu-id="f5381-149">Beschreibung der Ressourcenoperation.</span><span class="sxs-lookup"><span data-stu-id="f5381-149">Description of the resource operation.</span></span> <span data-ttu-id="f5381-150">Diese Beschreibung wird angezeigt, wenn der Benutzer im Azure-Portal den Mauszeiger auf der Operation platziert.</span><span class="sxs-lookup"><span data-stu-id="f5381-150">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="f5381-151">enabledForScopeValidation</span><span class="sxs-lookup"><span data-stu-id="f5381-151">enabledForScopeValidation</span></span>|<span data-ttu-id="f5381-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5381-152">Boolean</span></span>|<span data-ttu-id="f5381-153">Bestimmt, ob die Berechtigung für pro Rollenzuweisung definierten Bereiche nicht überprüft wird.</span><span class="sxs-lookup"><span data-stu-id="f5381-153">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="f5381-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="f5381-154">Response</span></span>
<span data-ttu-id="f5381-155">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [resourceOperation](../resources/intune-rbac-resourceoperation.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f5381-155">If successful, this method returns a `200 OK` response code and an updated [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5381-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f5381-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="f5381-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f5381-157">Request</span></span>
<span data-ttu-id="f5381-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f5381-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/resourceOperations/{resourceOperationId}
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

### <a name="response"></a><span data-ttu-id="f5381-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="f5381-159">Response</span></span>
<span data-ttu-id="f5381-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f5381-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




