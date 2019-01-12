---
title: Erstellen von „iosVppEBookAssignment“
description: Diese Methode erstellt ein neues Objekt des Typs iosVppEBookAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c2abbe332e59b642178ac87e682c7ef8fa3efe13
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961848"
---
# <a name="create-iosvppebookassignment"></a><span data-ttu-id="264a0-103">Erstellen von „iosVppEBookAssignment“</span><span class="sxs-lookup"><span data-stu-id="264a0-103">Create iosVppEBookAssignment</span></span>

> <span data-ttu-id="264a0-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="264a0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="264a0-105">Diese Methode erstellt ein neues Objekt des Typs [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="264a0-105">Create a new [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="264a0-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="264a0-106">Prerequisites</span></span>
<span data-ttu-id="264a0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="264a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="264a0-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="264a0-109">Permission type</span></span>|<span data-ttu-id="264a0-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="264a0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="264a0-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="264a0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="264a0-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="264a0-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="264a0-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="264a0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="264a0-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="264a0-114">Not supported.</span></span>|
|<span data-ttu-id="264a0-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="264a0-115">Application</span></span>|<span data-ttu-id="264a0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="264a0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="264a0-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="264a0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="264a0-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="264a0-118">Request headers</span></span>
|<span data-ttu-id="264a0-119">Header</span><span class="sxs-lookup"><span data-stu-id="264a0-119">Header</span></span>|<span data-ttu-id="264a0-120">Wert</span><span class="sxs-lookup"><span data-stu-id="264a0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="264a0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="264a0-121">Authorization</span></span>|<span data-ttu-id="264a0-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="264a0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="264a0-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="264a0-123">Accept</span></span>|<span data-ttu-id="264a0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="264a0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="264a0-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="264a0-125">Request body</span></span>
<span data-ttu-id="264a0-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „iosVppEBookAssignment“ an.</span><span class="sxs-lookup"><span data-stu-id="264a0-126">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="264a0-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „iosVppEBookAssignment“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="264a0-127">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="264a0-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="264a0-128">Property</span></span>|<span data-ttu-id="264a0-129">Typ</span><span class="sxs-lookup"><span data-stu-id="264a0-129">Type</span></span>|<span data-ttu-id="264a0-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="264a0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="264a0-131">id</span><span class="sxs-lookup"><span data-stu-id="264a0-131">id</span></span>|<span data-ttu-id="264a0-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="264a0-132">String</span></span>|<span data-ttu-id="264a0-133">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="264a0-133">Key of the entity.</span></span> <span data-ttu-id="264a0-134">Geerbt von [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="264a0-134">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="264a0-135">target</span><span class="sxs-lookup"><span data-stu-id="264a0-135">target</span></span>|[<span data-ttu-id="264a0-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="264a0-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="264a0-137">Zuweisungsziel für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="264a0-137">The assignment target for eBook.</span></span> <span data-ttu-id="264a0-138">Geerbt von [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="264a0-138">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="264a0-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="264a0-139">installIntent</span></span>|[<span data-ttu-id="264a0-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="264a0-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="264a0-141">Installationspriorität für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="264a0-141">The install intent for eBook.</span></span> <span data-ttu-id="264a0-142">Geerbt von [ManagedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="264a0-142">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="264a0-143">Mögliche Werte sind: `available`, `required`, `uninstall` und `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="264a0-143">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="264a0-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="264a0-144">Response</span></span>
<span data-ttu-id="264a0-145">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="264a0-145">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="264a0-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="264a0-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="264a0-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="264a0-147">Request</span></span>
<span data-ttu-id="264a0-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="264a0-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
Content-type: application/json
Content-length: 193

{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="264a0-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="264a0-149">Response</span></span>
<span data-ttu-id="264a0-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="264a0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 242

{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "id": "48f05789-5789-48f0-8957-f0488957f048",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```



