---
title: Aktualisieren von „managedEBookAssignment“
description: Aktualisieren der Eigenschaften eines managedEBookAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f85fe3da8970c671520c7086390108af9f3a0a97
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30959231"
---
# <a name="update-managedebookassignment"></a><span data-ttu-id="4840d-103">Aktualisieren von „managedEBookAssignment“</span><span class="sxs-lookup"><span data-stu-id="4840d-103">Update managedEBookAssignment</span></span>

> <span data-ttu-id="4840d-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4840d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4840d-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4840d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4840d-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4840d-106">Update the properties of a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4840d-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4840d-107">Prerequisites</span></span>
<span data-ttu-id="4840d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4840d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4840d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4840d-110">Permission type</span></span>|<span data-ttu-id="4840d-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4840d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4840d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4840d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4840d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4840d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4840d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4840d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4840d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4840d-115">Not supported.</span></span>|
|<span data-ttu-id="4840d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4840d-116">Application</span></span>|<span data-ttu-id="4840d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4840d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4840d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4840d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="4840d-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4840d-119">Request headers</span></span>
|<span data-ttu-id="4840d-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4840d-120">Header</span></span>|<span data-ttu-id="4840d-121">Wert</span><span class="sxs-lookup"><span data-stu-id="4840d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4840d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4840d-122">Authorization</span></span>|<span data-ttu-id="4840d-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4840d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4840d-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4840d-124">Accept</span></span>|<span data-ttu-id="4840d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4840d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4840d-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4840d-126">Request body</span></span>
<span data-ttu-id="4840d-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="4840d-127">In the request body, supply a JSON representation for the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

<span data-ttu-id="4840d-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="4840d-128">The following table shows the properties that are required when you create the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>

|<span data-ttu-id="4840d-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4840d-129">Property</span></span>|<span data-ttu-id="4840d-130">Typ</span><span class="sxs-lookup"><span data-stu-id="4840d-130">Type</span></span>|<span data-ttu-id="4840d-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4840d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4840d-132">id</span><span class="sxs-lookup"><span data-stu-id="4840d-132">id</span></span>|<span data-ttu-id="4840d-133">String</span><span class="sxs-lookup"><span data-stu-id="4840d-133">String</span></span>|<span data-ttu-id="4840d-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="4840d-134">Key of the entity.</span></span>|
|<span data-ttu-id="4840d-135">target</span><span class="sxs-lookup"><span data-stu-id="4840d-135">target</span></span>|[<span data-ttu-id="4840d-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4840d-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="4840d-137">Das Zuweisungsziel für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="4840d-137">The assignment target for eBook.</span></span>|
|<span data-ttu-id="4840d-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="4840d-138">installIntent</span></span>|[<span data-ttu-id="4840d-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="4840d-139">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="4840d-140">Die Installationspriorität für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="4840d-140">The install intent for eBook.</span></span> <span data-ttu-id="4840d-141">Mögliche Werte sind: `available`, `required`, `uninstall` und `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="4840d-141">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="4840d-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="4840d-142">Response</span></span>
<span data-ttu-id="4840d-143">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4840d-143">If successful, this method returns a `200 OK` response code and an updated [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4840d-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4840d-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="4840d-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4840d-145">Request</span></span>
<span data-ttu-id="4840d-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4840d-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
Content-type: application/json
Content-length: 194

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="4840d-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="4840d-147">Response</span></span>
<span data-ttu-id="4840d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4840d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 243

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```




