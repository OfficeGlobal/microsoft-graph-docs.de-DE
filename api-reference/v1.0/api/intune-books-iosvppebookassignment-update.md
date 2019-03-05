---
title: Aktualisieren von „iosVppEBookAssignment“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs iosVppEBookAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0505c55b9513eeb21ac0a120974f945a402d7764
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256735"
---
# <a name="update-iosvppebookassignment"></a><span data-ttu-id="67073-103">Aktualisieren von „iosVppEBookAssignment“</span><span class="sxs-lookup"><span data-stu-id="67073-103">Update iosVppEBookAssignment</span></span>

> <span data-ttu-id="67073-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="67073-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67073-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="67073-105">Update the properties of a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67073-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="67073-106">Prerequisites</span></span>
<span data-ttu-id="67073-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="67073-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="67073-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="67073-109">Permission type</span></span>|<span data-ttu-id="67073-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="67073-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67073-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="67073-111">Delegated (work or school account)</span></span>|<span data-ttu-id="67073-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67073-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="67073-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="67073-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67073-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="67073-114">Not supported.</span></span>|
|<span data-ttu-id="67073-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="67073-115">Application</span></span>|<span data-ttu-id="67073-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="67073-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67073-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="67073-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="67073-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="67073-118">Request headers</span></span>
|<span data-ttu-id="67073-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="67073-119">Header</span></span>|<span data-ttu-id="67073-120">Wert</span><span class="sxs-lookup"><span data-stu-id="67073-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67073-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="67073-121">Authorization</span></span>|<span data-ttu-id="67073-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="67073-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67073-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="67073-123">Accept</span></span>|<span data-ttu-id="67073-124">application/json</span><span class="sxs-lookup"><span data-stu-id="67073-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67073-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="67073-125">Request body</span></span>
<span data-ttu-id="67073-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="67073-126">In the request body, supply a JSON representation for the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

<span data-ttu-id="67073-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="67073-127">The following table shows the properties that are required when you create the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span></span>

|<span data-ttu-id="67073-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="67073-128">Property</span></span>|<span data-ttu-id="67073-129">Typ</span><span class="sxs-lookup"><span data-stu-id="67073-129">Type</span></span>|<span data-ttu-id="67073-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="67073-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67073-131">id</span><span class="sxs-lookup"><span data-stu-id="67073-131">id</span></span>|<span data-ttu-id="67073-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="67073-132">String</span></span>|<span data-ttu-id="67073-133">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="67073-133">Key of the entity.</span></span> <span data-ttu-id="67073-134">Geerbt von [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="67073-134">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="67073-135">target</span><span class="sxs-lookup"><span data-stu-id="67073-135">target</span></span>|[<span data-ttu-id="67073-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="67073-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="67073-137">Zuweisungsziel für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="67073-137">The assignment target for eBook.</span></span> <span data-ttu-id="67073-138">Geerbt von [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="67073-138">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="67073-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="67073-139">installIntent</span></span>|[<span data-ttu-id="67073-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="67073-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="67073-141">Installationspriorität für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="67073-141">The install intent for eBook.</span></span> <span data-ttu-id="67073-142">Von [ManagedEBookAssignment](../resources/intune-books-managedebookassignment.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="67073-142">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="67073-143">Mögliche Werte sind: `available`, `required`, `uninstall` und `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="67073-143">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="67073-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="67073-144">Response</span></span>
<span data-ttu-id="67073-145">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="67073-145">If successful, this method returns a `200 OK` response code and an updated [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67073-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="67073-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="67073-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="67073-147">Request</span></span>
<span data-ttu-id="67073-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="67073-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
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

### <a name="response"></a><span data-ttu-id="67073-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="67073-149">Response</span></span>
<span data-ttu-id="67073-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="67073-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



