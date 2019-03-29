---
title: resourceOperation erstellen
description: Erstellt neue Objekte des Typs resourceOperation.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fde65e56ec2f9c622140819e68064ed02138e90f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30960370"
---
# <a name="create-resourceoperation"></a><span data-ttu-id="c61b3-103">resourceOperation erstellen</span><span class="sxs-lookup"><span data-stu-id="c61b3-103">Create resourceOperation</span></span>

> <span data-ttu-id="c61b3-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c61b3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c61b3-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c61b3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c61b3-106">Erstellt neue Objekte des Typs [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="c61b3-106">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c61b3-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c61b3-107">Prerequisites</span></span>
<span data-ttu-id="c61b3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c61b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c61b3-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c61b3-110">Permission type</span></span>|<span data-ttu-id="c61b3-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c61b3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c61b3-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c61b3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c61b3-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c61b3-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="c61b3-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c61b3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c61b3-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c61b3-115">Not supported.</span></span>|
|<span data-ttu-id="c61b3-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c61b3-116">Application</span></span>|<span data-ttu-id="c61b3-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c61b3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c61b3-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c61b3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="c61b3-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c61b3-119">Request headers</span></span>
|<span data-ttu-id="c61b3-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c61b3-120">Header</span></span>|<span data-ttu-id="c61b3-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c61b3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c61b3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c61b3-122">Authorization</span></span>|<span data-ttu-id="c61b3-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c61b3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c61b3-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c61b3-124">Accept</span></span>|<span data-ttu-id="c61b3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c61b3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c61b3-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c61b3-126">Request body</span></span>
<span data-ttu-id="c61b3-127">Geben Sie im Anforderungstext eine JSON-Darstellung des resourceOperation-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="c61b3-127">In the request body, supply a JSON representation for the resourceOperation object.</span></span>

<span data-ttu-id="c61b3-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der resourceOperation erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c61b3-128">The following table shows the properties that are required when you create the resourceOperation.</span></span>

|<span data-ttu-id="c61b3-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c61b3-129">Property</span></span>|<span data-ttu-id="c61b3-130">Typ</span><span class="sxs-lookup"><span data-stu-id="c61b3-130">Type</span></span>|<span data-ttu-id="c61b3-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c61b3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c61b3-132">id</span><span class="sxs-lookup"><span data-stu-id="c61b3-132">id</span></span>|<span data-ttu-id="c61b3-133">String</span><span class="sxs-lookup"><span data-stu-id="c61b3-133">String</span></span>|<span data-ttu-id="c61b3-134">Schlüssel der Ressourcenoperation.</span><span class="sxs-lookup"><span data-stu-id="c61b3-134">Key of the Resource Operation.</span></span> <span data-ttu-id="c61b3-135">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="c61b3-135">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="c61b3-136">resource</span><span class="sxs-lookup"><span data-stu-id="c61b3-136">resource</span></span>|<span data-ttu-id="c61b3-137">String</span><span class="sxs-lookup"><span data-stu-id="c61b3-137">String</span></span>|<span data-ttu-id="c61b3-138">Ressourcenkategorie, zu der dieser Vorgang gehört.</span><span class="sxs-lookup"><span data-stu-id="c61b3-138">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="c61b3-139">resourceName</span><span class="sxs-lookup"><span data-stu-id="c61b3-139">resourceName</span></span>|<span data-ttu-id="c61b3-140">String</span><span class="sxs-lookup"><span data-stu-id="c61b3-140">String</span></span>|<span data-ttu-id="c61b3-141">Name der Ressource, auf die die Operation angewendet wird</span><span class="sxs-lookup"><span data-stu-id="c61b3-141">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="c61b3-142">actionName</span><span class="sxs-lookup"><span data-stu-id="c61b3-142">actionName</span></span>|<span data-ttu-id="c61b3-143">String</span><span class="sxs-lookup"><span data-stu-id="c61b3-143">String</span></span>|<span data-ttu-id="c61b3-144">Typ von Aktion, den die Operation ausführen wird.</span><span class="sxs-lookup"><span data-stu-id="c61b3-144">Type of action this operation is going to perform.</span></span> <span data-ttu-id="c61b3-145">Der Wert für „actionName“ sollte prägnant sein und aus möglichst wenigen Wörtern bestehen.</span><span class="sxs-lookup"><span data-stu-id="c61b3-145">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="c61b3-146">description</span><span class="sxs-lookup"><span data-stu-id="c61b3-146">description</span></span>|<span data-ttu-id="c61b3-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c61b3-147">String</span></span>|<span data-ttu-id="c61b3-148">Beschreibung der Ressourcenoperation.</span><span class="sxs-lookup"><span data-stu-id="c61b3-148">Description of the resource operation.</span></span> <span data-ttu-id="c61b3-149">Diese Beschreibung wird angezeigt, wenn der Benutzer im Azure-Portal den Mauszeiger auf der Operation platziert.</span><span class="sxs-lookup"><span data-stu-id="c61b3-149">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="c61b3-150">enabledForScopeValidation</span><span class="sxs-lookup"><span data-stu-id="c61b3-150">enabledForScopeValidation</span></span>|<span data-ttu-id="c61b3-151">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c61b3-151">Boolean</span></span>|<span data-ttu-id="c61b3-152">Bestimmt, ob die Berechtigung für Bereiche validiert wird, die pro Rollenzuweisung definiert sind.</span><span class="sxs-lookup"><span data-stu-id="c61b3-152">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="c61b3-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="c61b3-153">Response</span></span>
<span data-ttu-id="c61b3-154">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [resourceOperation](../resources/intune-rbac-resourceoperation.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c61b3-154">If successful, this method returns a `201 Created` response code and a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c61b3-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c61b3-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="c61b3-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c61b3-156">Request</span></span>
<span data-ttu-id="c61b3-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c61b3-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c61b3-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="c61b3-158">Response</span></span>
<span data-ttu-id="c61b3-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c61b3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




