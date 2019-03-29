---
title: Erstellen von „managedEBookAssignment“
description: Erstellen eines neuen managedEBookAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f62d14f924474103c288ab92920839cadc9c97d2
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30968252"
---
# <a name="create-managedebookassignment"></a><span data-ttu-id="32ecd-103">Erstellen von „managedEBookAssignment“</span><span class="sxs-lookup"><span data-stu-id="32ecd-103">Create managedEBookAssignment</span></span>

> <span data-ttu-id="32ecd-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="32ecd-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32ecd-105">Diese Methode erstellt ein neues Objekt des Typs [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="32ecd-105">Create a new [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32ecd-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="32ecd-106">Prerequisites</span></span>
<span data-ttu-id="32ecd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32ecd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32ecd-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="32ecd-109">Permission type</span></span>|<span data-ttu-id="32ecd-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="32ecd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32ecd-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="32ecd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="32ecd-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32ecd-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="32ecd-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="32ecd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32ecd-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="32ecd-114">Not supported.</span></span>|
|<span data-ttu-id="32ecd-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="32ecd-115">Application</span></span>|<span data-ttu-id="32ecd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="32ecd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32ecd-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="32ecd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="32ecd-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="32ecd-118">Request headers</span></span>
|<span data-ttu-id="32ecd-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="32ecd-119">Header</span></span>|<span data-ttu-id="32ecd-120">Wert</span><span class="sxs-lookup"><span data-stu-id="32ecd-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32ecd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="32ecd-121">Authorization</span></span>|<span data-ttu-id="32ecd-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="32ecd-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32ecd-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="32ecd-123">Accept</span></span>|<span data-ttu-id="32ecd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="32ecd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32ecd-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="32ecd-125">Request body</span></span>
<span data-ttu-id="32ecd-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „managedEBookAssignment“ an.</span><span class="sxs-lookup"><span data-stu-id="32ecd-126">In the request body, supply a JSON representation for the managedEBookAssignment object.</span></span>

<span data-ttu-id="32ecd-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „managedEBookAssignment“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="32ecd-127">The following table shows the properties that are required when you create the managedEBookAssignment.</span></span>

|<span data-ttu-id="32ecd-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="32ecd-128">Property</span></span>|<span data-ttu-id="32ecd-129">Typ</span><span class="sxs-lookup"><span data-stu-id="32ecd-129">Type</span></span>|<span data-ttu-id="32ecd-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="32ecd-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32ecd-131">id</span><span class="sxs-lookup"><span data-stu-id="32ecd-131">id</span></span>|<span data-ttu-id="32ecd-132">String</span><span class="sxs-lookup"><span data-stu-id="32ecd-132">String</span></span>|<span data-ttu-id="32ecd-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="32ecd-133">Key of the entity.</span></span>|
|<span data-ttu-id="32ecd-134">target</span><span class="sxs-lookup"><span data-stu-id="32ecd-134">target</span></span>|[<span data-ttu-id="32ecd-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="32ecd-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="32ecd-136">Das Zuweisungsziel für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="32ecd-136">The assignment target for eBook.</span></span>|
|<span data-ttu-id="32ecd-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="32ecd-137">installIntent</span></span>|[<span data-ttu-id="32ecd-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="32ecd-138">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="32ecd-139">Die Installationspriorität für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="32ecd-139">The install intent for eBook.</span></span> <span data-ttu-id="32ecd-140">Mögliche Werte sind: `available`, `required`, `uninstall` und `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="32ecd-140">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="32ecd-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="32ecd-141">Response</span></span>
<span data-ttu-id="32ecd-142">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="32ecd-142">If successful, this method returns a `201 Created` response code and a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32ecd-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="32ecd-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="32ecd-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="32ecd-144">Request</span></span>
<span data-ttu-id="32ecd-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="32ecd-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
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

### <a name="response"></a><span data-ttu-id="32ecd-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="32ecd-146">Response</span></span>
<span data-ttu-id="32ecd-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="32ecd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



