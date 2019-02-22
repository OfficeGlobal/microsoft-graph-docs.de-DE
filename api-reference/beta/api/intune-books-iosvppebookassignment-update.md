---
title: Aktualisieren von „iosVppEBookAssignment“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs iosVppEBookAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0c04bd5a2a6e57d64a1baed1a80cb6e6c2761a00
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158478"
---
# <a name="update-iosvppebookassignment"></a><span data-ttu-id="fe3e3-103">Aktualisieren von „iosVppEBookAssignment“</span><span class="sxs-lookup"><span data-stu-id="fe3e3-103">Update iosVppEBookAssignment</span></span>

> <span data-ttu-id="fe3e3-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe3e3-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe3e3-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="fe3e3-106">Update the properties of a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe3e3-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fe3e3-107">Prerequisites</span></span>
<span data-ttu-id="fe3e3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fe3e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fe3e3-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fe3e3-110">Permission type</span></span>|<span data-ttu-id="fe3e3-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fe3e3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe3e3-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fe3e3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fe3e3-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe3e3-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fe3e3-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fe3e3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe3e3-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fe3e3-115">Not supported.</span></span>|
|<span data-ttu-id="fe3e3-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fe3e3-116">Application</span></span>|<span data-ttu-id="fe3e3-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fe3e3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe3e3-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fe3e3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="fe3e3-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fe3e3-119">Request headers</span></span>
|<span data-ttu-id="fe3e3-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="fe3e3-120">Header</span></span>|<span data-ttu-id="fe3e3-121">Wert</span><span class="sxs-lookup"><span data-stu-id="fe3e3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe3e3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe3e3-122">Authorization</span></span>|<span data-ttu-id="fe3e3-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fe3e3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe3e3-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fe3e3-124">Accept</span></span>|<span data-ttu-id="fe3e3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fe3e3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe3e3-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fe3e3-126">Request body</span></span>
<span data-ttu-id="fe3e3-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-127">In the request body, supply a JSON representation for the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

<span data-ttu-id="fe3e3-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-128">The following table shows the properties that are required when you create the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span></span>

|<span data-ttu-id="fe3e3-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fe3e3-129">Property</span></span>|<span data-ttu-id="fe3e3-130">Typ</span><span class="sxs-lookup"><span data-stu-id="fe3e3-130">Type</span></span>|<span data-ttu-id="fe3e3-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fe3e3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe3e3-132">id</span><span class="sxs-lookup"><span data-stu-id="fe3e3-132">id</span></span>|<span data-ttu-id="fe3e3-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fe3e3-133">String</span></span>|<span data-ttu-id="fe3e3-134">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-134">Key of the entity.</span></span> <span data-ttu-id="fe3e3-135">Geerbt von [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="fe3e3-135">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="fe3e3-136">target</span><span class="sxs-lookup"><span data-stu-id="fe3e3-136">target</span></span>|[<span data-ttu-id="fe3e3-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="fe3e3-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="fe3e3-138">Zuweisungsziel für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-138">The assignment target for eBook.</span></span> <span data-ttu-id="fe3e3-139">Geerbt von [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="fe3e3-139">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="fe3e3-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="fe3e3-140">installIntent</span></span>|[<span data-ttu-id="fe3e3-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="fe3e3-141">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="fe3e3-142">Installationspriorität für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-142">The install intent for eBook.</span></span> <span data-ttu-id="fe3e3-143">Von [ManagedEBookAssignment](../resources/intune-books-managedebookassignment.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-143">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="fe3e3-144">Mögliche Werte sind: `available`, `required`, `uninstall` und `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-144">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="fe3e3-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="fe3e3-145">Response</span></span>
<span data-ttu-id="fe3e3-146">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-146">If successful, this method returns a `200 OK` response code and an updated [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe3e3-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fe3e3-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe3e3-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fe3e3-148">Request</span></span>
<span data-ttu-id="fe3e3-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
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

### <a name="response"></a><span data-ttu-id="fe3e3-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="fe3e3-150">Response</span></span>
<span data-ttu-id="fe3e3-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




