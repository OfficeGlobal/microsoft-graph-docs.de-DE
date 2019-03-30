---
title: Erstellen von „managedEBookAssignment“
description: Erstellen eines neuen managedEBookAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 89e7f41962818f3d1ce535a792262f613f052929
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30981314"
---
# <a name="create-managedebookassignment"></a><span data-ttu-id="1ba63-103">Erstellen von „managedEBookAssignment“</span><span class="sxs-lookup"><span data-stu-id="1ba63-103">Create managedEBookAssignment</span></span>

> <span data-ttu-id="1ba63-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1ba63-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ba63-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1ba63-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ba63-106">Diese Methode erstellt ein neues Objekt des Typs [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1ba63-106">Create a new [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ba63-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1ba63-107">Prerequisites</span></span>
<span data-ttu-id="1ba63-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ba63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ba63-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1ba63-110">Permission type</span></span>|<span data-ttu-id="1ba63-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1ba63-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ba63-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1ba63-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1ba63-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ba63-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1ba63-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1ba63-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ba63-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1ba63-115">Not supported.</span></span>|
|<span data-ttu-id="1ba63-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1ba63-116">Application</span></span>|<span data-ttu-id="1ba63-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1ba63-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ba63-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1ba63-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="1ba63-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1ba63-119">Request headers</span></span>
|<span data-ttu-id="1ba63-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1ba63-120">Header</span></span>|<span data-ttu-id="1ba63-121">Wert</span><span class="sxs-lookup"><span data-stu-id="1ba63-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ba63-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ba63-122">Authorization</span></span>|<span data-ttu-id="1ba63-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1ba63-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ba63-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1ba63-124">Accept</span></span>|<span data-ttu-id="1ba63-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1ba63-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ba63-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1ba63-126">Request body</span></span>
<span data-ttu-id="1ba63-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „managedEBookAssignment“ an.</span><span class="sxs-lookup"><span data-stu-id="1ba63-127">In the request body, supply a JSON representation for the managedEBookAssignment object.</span></span>

<span data-ttu-id="1ba63-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „managedEBookAssignment“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="1ba63-128">The following table shows the properties that are required when you create the managedEBookAssignment.</span></span>

|<span data-ttu-id="1ba63-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1ba63-129">Property</span></span>|<span data-ttu-id="1ba63-130">Typ</span><span class="sxs-lookup"><span data-stu-id="1ba63-130">Type</span></span>|<span data-ttu-id="1ba63-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1ba63-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ba63-132">id</span><span class="sxs-lookup"><span data-stu-id="1ba63-132">id</span></span>|<span data-ttu-id="1ba63-133">String</span><span class="sxs-lookup"><span data-stu-id="1ba63-133">String</span></span>|<span data-ttu-id="1ba63-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="1ba63-134">Key of the entity.</span></span>|
|<span data-ttu-id="1ba63-135">target</span><span class="sxs-lookup"><span data-stu-id="1ba63-135">target</span></span>|[<span data-ttu-id="1ba63-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1ba63-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1ba63-137">Das Zuweisungsziel für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="1ba63-137">The assignment target for eBook.</span></span>|
|<span data-ttu-id="1ba63-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="1ba63-138">installIntent</span></span>|[<span data-ttu-id="1ba63-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="1ba63-139">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="1ba63-140">Die Installationspriorität für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="1ba63-140">The install intent for eBook.</span></span> <span data-ttu-id="1ba63-141">Mögliche Werte sind: `available`, `required`, `uninstall` und `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="1ba63-141">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="1ba63-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="1ba63-142">Response</span></span>
<span data-ttu-id="1ba63-143">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1ba63-143">If successful, this method returns a `201 Created` response code and a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ba63-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1ba63-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ba63-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1ba63-145">Request</span></span>
<span data-ttu-id="1ba63-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1ba63-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
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

### <a name="response"></a><span data-ttu-id="1ba63-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="1ba63-147">Response</span></span>
<span data-ttu-id="1ba63-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1ba63-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




