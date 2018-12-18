---
title: Aktualisieren von „iosVppEBookAssignment“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs iosVppEBookAssignment.
author: tfitzmac
ms.openlocfilehash: 537c2ef5838dc68881f3de693a6591570219ece4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338150"
---
# <a name="update-iosvppebookassignment"></a><span data-ttu-id="38131-103">Aktualisieren von „iosVppEBookAssignment“</span><span class="sxs-lookup"><span data-stu-id="38131-103">Update iosVppEBookAssignment</span></span>

> <span data-ttu-id="38131-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="38131-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="38131-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="38131-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="38131-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="38131-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="38131-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="38131-107">Update the properties of a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="38131-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="38131-108">Prerequisites</span></span>
<span data-ttu-id="38131-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38131-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38131-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="38131-111">Permission type</span></span>|<span data-ttu-id="38131-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="38131-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38131-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="38131-113">Delegated (work or school account)</span></span>|<span data-ttu-id="38131-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38131-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="38131-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="38131-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38131-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="38131-116">Not supported.</span></span>|
|<span data-ttu-id="38131-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="38131-117">Application</span></span>|<span data-ttu-id="38131-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="38131-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="38131-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="38131-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="38131-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="38131-120">Request headers</span></span>
|<span data-ttu-id="38131-121">Header</span><span class="sxs-lookup"><span data-stu-id="38131-121">Header</span></span>|<span data-ttu-id="38131-122">Wert</span><span class="sxs-lookup"><span data-stu-id="38131-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38131-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="38131-123">Authorization</span></span>|<span data-ttu-id="38131-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="38131-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38131-125">Accept</span><span class="sxs-lookup"><span data-stu-id="38131-125">Accept</span></span>|<span data-ttu-id="38131-126">application/json</span><span class="sxs-lookup"><span data-stu-id="38131-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38131-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="38131-127">Request body</span></span>
<span data-ttu-id="38131-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="38131-128">In the request body, supply a JSON representation for the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

<span data-ttu-id="38131-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="38131-129">The following table shows the properties that are required when you create the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span></span>

|<span data-ttu-id="38131-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="38131-130">Property</span></span>|<span data-ttu-id="38131-131">Typ</span><span class="sxs-lookup"><span data-stu-id="38131-131">Type</span></span>|<span data-ttu-id="38131-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="38131-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38131-133">id</span><span class="sxs-lookup"><span data-stu-id="38131-133">id</span></span>|<span data-ttu-id="38131-134">String</span><span class="sxs-lookup"><span data-stu-id="38131-134">String</span></span>|<span data-ttu-id="38131-135">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="38131-135">Key of the entity.</span></span> <span data-ttu-id="38131-136">Geerbt von [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="38131-136">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="38131-137">target</span><span class="sxs-lookup"><span data-stu-id="38131-137">target</span></span>|[<span data-ttu-id="38131-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="38131-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="38131-139">Zuweisungsziel für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="38131-139">The assignment target for eBook.</span></span> <span data-ttu-id="38131-140">Geerbt von [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="38131-140">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="38131-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="38131-141">installIntent</span></span>|[<span data-ttu-id="38131-142">installIntent</span><span class="sxs-lookup"><span data-stu-id="38131-142">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="38131-143">Installationspriorität für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="38131-143">The install intent for eBook.</span></span> <span data-ttu-id="38131-144">Geerbt von [ManagedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="38131-144">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="38131-145">Mögliche Werte sind: `available`, `required`, `uninstall` und `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="38131-145">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="38131-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="38131-146">Response</span></span>
<span data-ttu-id="38131-147">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="38131-147">If successful, this method returns a `200 OK` response code and an updated [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38131-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="38131-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="38131-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="38131-149">Request</span></span>
<span data-ttu-id="38131-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="38131-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
Content-type: application/json
Content-length: 133

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="38131-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="38131-151">Response</span></span>
<span data-ttu-id="38131-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="38131-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





