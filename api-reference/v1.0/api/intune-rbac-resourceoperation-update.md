---
title: resourceOperation aktualisieren
description: Aktualisiert die Eigenschaften von Objekten des Typs resourceOperation.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 571a39b343930a7ade182c764229541f00d0b1eb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921157"
---
# <a name="update-resourceoperation"></a><span data-ttu-id="305fa-103">resourceOperation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="305fa-103">Update resourceOperation</span></span>

> <span data-ttu-id="305fa-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="305fa-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="305fa-105">Aktualisiert die Eigenschaften von Objekten des Typs [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="305fa-105">Update the properties of a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="305fa-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="305fa-106">Prerequisites</span></span>
<span data-ttu-id="305fa-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="305fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="305fa-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="305fa-109">Permission type</span></span>|<span data-ttu-id="305fa-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="305fa-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="305fa-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="305fa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="305fa-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="305fa-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="305fa-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="305fa-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="305fa-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="305fa-114">Not supported.</span></span>|
|<span data-ttu-id="305fa-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="305fa-115">Application</span></span>|<span data-ttu-id="305fa-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="305fa-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="305fa-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="305fa-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="305fa-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="305fa-118">Request headers</span></span>
|<span data-ttu-id="305fa-119">Header</span><span class="sxs-lookup"><span data-stu-id="305fa-119">Header</span></span>|<span data-ttu-id="305fa-120">Wert</span><span class="sxs-lookup"><span data-stu-id="305fa-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="305fa-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="305fa-121">Authorization</span></span>|<span data-ttu-id="305fa-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="305fa-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="305fa-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="305fa-123">Accept</span></span>|<span data-ttu-id="305fa-124">application/json</span><span class="sxs-lookup"><span data-stu-id="305fa-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="305fa-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="305fa-125">Request body</span></span>
<span data-ttu-id="305fa-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [resourceOperation](../resources/intune-rbac-resourceoperation.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="305fa-126">In the request body, supply a JSON representation for the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

<span data-ttu-id="305fa-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [resourceOperation](../resources/intune-rbac-resourceoperation.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="305fa-127">The following table shows the properties that are required when you create the [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>

|<span data-ttu-id="305fa-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="305fa-128">Property</span></span>|<span data-ttu-id="305fa-129">Typ</span><span class="sxs-lookup"><span data-stu-id="305fa-129">Type</span></span>|<span data-ttu-id="305fa-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="305fa-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="305fa-131">id</span><span class="sxs-lookup"><span data-stu-id="305fa-131">id</span></span>|<span data-ttu-id="305fa-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="305fa-132">String</span></span>|<span data-ttu-id="305fa-133">Schlüssel der Ressourcenoperation.</span><span class="sxs-lookup"><span data-stu-id="305fa-133">Key of the Resource Operation.</span></span> <span data-ttu-id="305fa-134">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="305fa-134">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="305fa-135">resourceName</span><span class="sxs-lookup"><span data-stu-id="305fa-135">resourceName</span></span>|<span data-ttu-id="305fa-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="305fa-136">String</span></span>|<span data-ttu-id="305fa-137">Name der Ressource, auf die die Operation angewendet wird</span><span class="sxs-lookup"><span data-stu-id="305fa-137">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="305fa-138">actionName</span><span class="sxs-lookup"><span data-stu-id="305fa-138">actionName</span></span>|<span data-ttu-id="305fa-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="305fa-139">String</span></span>|<span data-ttu-id="305fa-140">Typ von Aktion, den die Operation ausführen wird.</span><span class="sxs-lookup"><span data-stu-id="305fa-140">Type of action this operation is going to perform.</span></span> <span data-ttu-id="305fa-141">Der Wert für „actionName“ sollte prägnant sein und aus möglichst wenigen Wörtern bestehen.</span><span class="sxs-lookup"><span data-stu-id="305fa-141">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="305fa-142">description</span><span class="sxs-lookup"><span data-stu-id="305fa-142">description</span></span>|<span data-ttu-id="305fa-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="305fa-143">String</span></span>|<span data-ttu-id="305fa-144">Beschreibung der Ressourcenoperation.</span><span class="sxs-lookup"><span data-stu-id="305fa-144">Description of the resource operation.</span></span> <span data-ttu-id="305fa-145">Diese Beschreibung wird angezeigt, wenn der Benutzer im Azure-Portal den Mauszeiger auf der Operation platziert.</span><span class="sxs-lookup"><span data-stu-id="305fa-145">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="305fa-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="305fa-146">Response</span></span>
<span data-ttu-id="305fa-147">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [resourceOperation](../resources/intune-rbac-resourceoperation.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="305fa-147">If successful, this method returns a `200 OK` response code and an updated [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="305fa-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="305fa-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="305fa-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="305fa-149">Request</span></span>
<span data-ttu-id="305fa-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="305fa-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="305fa-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="305fa-151">Response</span></span>
<span data-ttu-id="305fa-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="305fa-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



