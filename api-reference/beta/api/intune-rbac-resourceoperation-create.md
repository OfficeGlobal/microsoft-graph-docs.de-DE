---
title: resourceOperation erstellen
description: Erstellt neue Objekte des Typs resourceOperation.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5ecbe52ac2c988967a121904e63d1bd6e00929a5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154152"
---
# <a name="create-resourceoperation"></a><span data-ttu-id="fa691-103">resourceOperation erstellen</span><span class="sxs-lookup"><span data-stu-id="fa691-103">Create resourceOperation</span></span>

> <span data-ttu-id="fa691-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fa691-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa691-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="fa691-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa691-106">Erstellt neue Objekte des Typs [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="fa691-106">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa691-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fa691-107">Prerequisites</span></span>
<span data-ttu-id="fa691-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fa691-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fa691-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fa691-110">Permission type</span></span>|<span data-ttu-id="fa691-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fa691-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa691-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fa691-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fa691-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa691-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="fa691-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fa691-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa691-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fa691-115">Not supported.</span></span>|
|<span data-ttu-id="fa691-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fa691-116">Application</span></span>|<span data-ttu-id="fa691-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fa691-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa691-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa691-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="fa691-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fa691-119">Request headers</span></span>
|<span data-ttu-id="fa691-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="fa691-120">Header</span></span>|<span data-ttu-id="fa691-121">Wert</span><span class="sxs-lookup"><span data-stu-id="fa691-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa691-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa691-122">Authorization</span></span>|<span data-ttu-id="fa691-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fa691-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa691-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fa691-124">Accept</span></span>|<span data-ttu-id="fa691-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fa691-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa691-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fa691-126">Request body</span></span>
<span data-ttu-id="fa691-127">Geben Sie im Anforderungstext eine JSON-Darstellung des resourceOperation-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="fa691-127">In the request body, supply a JSON representation for the resourceOperation object.</span></span>

<span data-ttu-id="fa691-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der resourceOperation erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="fa691-128">The following table shows the properties that are required when you create the resourceOperation.</span></span>

|<span data-ttu-id="fa691-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fa691-129">Property</span></span>|<span data-ttu-id="fa691-130">Typ</span><span class="sxs-lookup"><span data-stu-id="fa691-130">Type</span></span>|<span data-ttu-id="fa691-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fa691-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa691-132">id</span><span class="sxs-lookup"><span data-stu-id="fa691-132">id</span></span>|<span data-ttu-id="fa691-133">string</span><span class="sxs-lookup"><span data-stu-id="fa691-133">String</span></span>|<span data-ttu-id="fa691-134">Schlüssel der Ressourcenoperation.</span><span class="sxs-lookup"><span data-stu-id="fa691-134">Key of the Resource Operation.</span></span> <span data-ttu-id="fa691-135">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="fa691-135">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="fa691-136">resource</span><span class="sxs-lookup"><span data-stu-id="fa691-136">resource</span></span>|<span data-ttu-id="fa691-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa691-137">String</span></span>|<span data-ttu-id="fa691-138">Ressourcenkategorie, zu der dieser Vorgang gehört.</span><span class="sxs-lookup"><span data-stu-id="fa691-138">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="fa691-139">resourceName</span><span class="sxs-lookup"><span data-stu-id="fa691-139">resourceName</span></span>|<span data-ttu-id="fa691-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa691-140">String</span></span>|<span data-ttu-id="fa691-141">Name der Ressource, auf die die Operation angewendet wird</span><span class="sxs-lookup"><span data-stu-id="fa691-141">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="fa691-142">actionName</span><span class="sxs-lookup"><span data-stu-id="fa691-142">actionName</span></span>|<span data-ttu-id="fa691-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa691-143">String</span></span>|<span data-ttu-id="fa691-144">Typ von Aktion, den die Operation ausführen wird.</span><span class="sxs-lookup"><span data-stu-id="fa691-144">Type of action this operation is going to perform.</span></span> <span data-ttu-id="fa691-145">Der Wert für „actionName“ sollte prägnant sein und aus möglichst wenigen Wörtern bestehen.</span><span class="sxs-lookup"><span data-stu-id="fa691-145">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="fa691-146">description</span><span class="sxs-lookup"><span data-stu-id="fa691-146">description</span></span>|<span data-ttu-id="fa691-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa691-147">String</span></span>|<span data-ttu-id="fa691-148">Beschreibung der Ressourcenoperation.</span><span class="sxs-lookup"><span data-stu-id="fa691-148">Description of the resource operation.</span></span> <span data-ttu-id="fa691-149">Diese Beschreibung wird angezeigt, wenn der Benutzer im Azure-Portal den Mauszeiger auf der Operation platziert.</span><span class="sxs-lookup"><span data-stu-id="fa691-149">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="fa691-150">enabledForScopeValidation</span><span class="sxs-lookup"><span data-stu-id="fa691-150">enabledForScopeValidation</span></span>|<span data-ttu-id="fa691-151">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="fa691-151">Boolean</span></span>|<span data-ttu-id="fa691-152">Bestimmt, ob die Berechtigung für Bereiche validiert wird, die pro Rollenzuweisung definiert sind.</span><span class="sxs-lookup"><span data-stu-id="fa691-152">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="fa691-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa691-153">Response</span></span>
<span data-ttu-id="fa691-154">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [resourceOperation](../resources/intune-rbac-resourceoperation.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fa691-154">If successful, this method returns a `201 Created` response code and a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa691-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fa691-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa691-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa691-156">Request</span></span>
<span data-ttu-id="fa691-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fa691-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fa691-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa691-158">Response</span></span>
<span data-ttu-id="fa691-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fa691-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




