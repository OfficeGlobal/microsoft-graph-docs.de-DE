---
title: resourceOperation erstellen
description: Erstellt neue Objekte des Typs resourceOperation.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 86bcd9af52a25e47b3a1fb07ec86f4ff7da0f8ba
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884707"
---
# <a name="create-resourceoperation"></a><span data-ttu-id="d56ab-103">resourceOperation erstellen</span><span class="sxs-lookup"><span data-stu-id="d56ab-103">Create resourceOperation</span></span>

> <span data-ttu-id="d56ab-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d56ab-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d56ab-105">Erstellt neue Objekte des Typs [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="d56ab-105">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d56ab-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d56ab-106">Prerequisites</span></span>
<span data-ttu-id="d56ab-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d56ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d56ab-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d56ab-109">Permission type</span></span>|<span data-ttu-id="d56ab-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d56ab-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d56ab-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d56ab-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d56ab-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d56ab-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="d56ab-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d56ab-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d56ab-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d56ab-114">Not supported.</span></span>|
|<span data-ttu-id="d56ab-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d56ab-115">Application</span></span>|<span data-ttu-id="d56ab-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d56ab-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d56ab-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d56ab-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="d56ab-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d56ab-118">Request headers</span></span>
|<span data-ttu-id="d56ab-119">Header</span><span class="sxs-lookup"><span data-stu-id="d56ab-119">Header</span></span>|<span data-ttu-id="d56ab-120">Wert</span><span class="sxs-lookup"><span data-stu-id="d56ab-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d56ab-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d56ab-121">Authorization</span></span>|<span data-ttu-id="d56ab-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d56ab-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d56ab-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d56ab-123">Accept</span></span>|<span data-ttu-id="d56ab-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d56ab-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d56ab-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d56ab-125">Request body</span></span>
<span data-ttu-id="d56ab-126">Geben Sie im Anforderungstext eine JSON-Darstellung des resourceOperation-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="d56ab-126">In the request body, supply a JSON representation for the resourceOperation object.</span></span>

<span data-ttu-id="d56ab-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der resourceOperation erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="d56ab-127">The following table shows the properties that are required when you create the resourceOperation.</span></span>

|<span data-ttu-id="d56ab-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d56ab-128">Property</span></span>|<span data-ttu-id="d56ab-129">Typ</span><span class="sxs-lookup"><span data-stu-id="d56ab-129">Type</span></span>|<span data-ttu-id="d56ab-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d56ab-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d56ab-131">id</span><span class="sxs-lookup"><span data-stu-id="d56ab-131">id</span></span>|<span data-ttu-id="d56ab-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d56ab-132">String</span></span>|<span data-ttu-id="d56ab-133">Schlüssel der Ressourcenoperation.</span><span class="sxs-lookup"><span data-stu-id="d56ab-133">Key of the Resource Operation.</span></span> <span data-ttu-id="d56ab-134">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="d56ab-134">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="d56ab-135">resourceName</span><span class="sxs-lookup"><span data-stu-id="d56ab-135">resourceName</span></span>|<span data-ttu-id="d56ab-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d56ab-136">String</span></span>|<span data-ttu-id="d56ab-137">Name der Ressource, auf die die Operation angewendet wird</span><span class="sxs-lookup"><span data-stu-id="d56ab-137">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="d56ab-138">actionName</span><span class="sxs-lookup"><span data-stu-id="d56ab-138">actionName</span></span>|<span data-ttu-id="d56ab-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d56ab-139">String</span></span>|<span data-ttu-id="d56ab-140">Typ von Aktion, den die Operation ausführen wird.</span><span class="sxs-lookup"><span data-stu-id="d56ab-140">Type of action this operation is going to perform.</span></span> <span data-ttu-id="d56ab-141">Der Wert für „actionName“ sollte prägnant sein und aus möglichst wenigen Wörtern bestehen.</span><span class="sxs-lookup"><span data-stu-id="d56ab-141">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="d56ab-142">description</span><span class="sxs-lookup"><span data-stu-id="d56ab-142">description</span></span>|<span data-ttu-id="d56ab-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d56ab-143">String</span></span>|<span data-ttu-id="d56ab-144">Beschreibung der Ressourcenoperation.</span><span class="sxs-lookup"><span data-stu-id="d56ab-144">Description of the resource operation.</span></span> <span data-ttu-id="d56ab-145">Diese Beschreibung wird angezeigt, wenn der Benutzer im Azure-Portal den Mauszeiger auf der Operation platziert.</span><span class="sxs-lookup"><span data-stu-id="d56ab-145">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="d56ab-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="d56ab-146">Response</span></span>
<span data-ttu-id="d56ab-147">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [resourceOperation](../resources/intune-rbac-resourceoperation.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d56ab-147">If successful, this method returns a `201 Created` response code and a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d56ab-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d56ab-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="d56ab-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d56ab-149">Request</span></span>
<span data-ttu-id="d56ab-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d56ab-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d56ab-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="d56ab-151">Response</span></span>
<span data-ttu-id="d56ab-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d56ab-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



