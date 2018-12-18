---
title: Aktualisieren von „managedEBookAssignment“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs managedEBookAssignment.
author: tfitzmac
ms.openlocfilehash: 9ac5d51413a9539667a11ee15e5789d359c94d9b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315764"
---
# <a name="update-managedebookassignment"></a><span data-ttu-id="f9b13-103">Aktualisieren von „managedEBookAssignment“</span><span class="sxs-lookup"><span data-stu-id="f9b13-103">Update managedEBookAssignment</span></span>

> <span data-ttu-id="f9b13-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f9b13-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9b13-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f9b13-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f9b13-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f9b13-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f9b13-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f9b13-107">Update the properties of a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f9b13-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f9b13-108">Prerequisites</span></span>
<span data-ttu-id="f9b13-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9b13-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9b13-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f9b13-111">Permission type</span></span>|<span data-ttu-id="f9b13-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f9b13-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9b13-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f9b13-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f9b13-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9b13-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f9b13-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f9b13-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9b13-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f9b13-116">Not supported.</span></span>|
|<span data-ttu-id="f9b13-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f9b13-117">Application</span></span>|<span data-ttu-id="f9b13-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f9b13-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9b13-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f9b13-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="f9b13-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f9b13-120">Request headers</span></span>
|<span data-ttu-id="f9b13-121">Header</span><span class="sxs-lookup"><span data-stu-id="f9b13-121">Header</span></span>|<span data-ttu-id="f9b13-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f9b13-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9b13-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f9b13-123">Authorization</span></span>|<span data-ttu-id="f9b13-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f9b13-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9b13-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f9b13-125">Accept</span></span>|<span data-ttu-id="f9b13-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f9b13-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9b13-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f9b13-127">Request body</span></span>
<span data-ttu-id="f9b13-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="f9b13-128">In the request body, supply a JSON representation for the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

<span data-ttu-id="f9b13-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="f9b13-129">The following table shows the properties that are required when you create the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>

|<span data-ttu-id="f9b13-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f9b13-130">Property</span></span>|<span data-ttu-id="f9b13-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f9b13-131">Type</span></span>|<span data-ttu-id="f9b13-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f9b13-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9b13-133">id</span><span class="sxs-lookup"><span data-stu-id="f9b13-133">id</span></span>|<span data-ttu-id="f9b13-134">String</span><span class="sxs-lookup"><span data-stu-id="f9b13-134">String</span></span>|<span data-ttu-id="f9b13-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f9b13-135">Key of the entity.</span></span>|
|<span data-ttu-id="f9b13-136">target</span><span class="sxs-lookup"><span data-stu-id="f9b13-136">target</span></span>|[<span data-ttu-id="f9b13-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f9b13-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="f9b13-138">Zuweisungsziel für das E-Book</span><span class="sxs-lookup"><span data-stu-id="f9b13-138">The assignment target for eBook.</span></span>|
|<span data-ttu-id="f9b13-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="f9b13-139">installIntent</span></span>|[<span data-ttu-id="f9b13-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="f9b13-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="f9b13-141">Installationspriorität für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="f9b13-141">The install intent for eBook.</span></span> <span data-ttu-id="f9b13-142">Mögliche Werte sind: `available`, `required`, `uninstall` und `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="f9b13-142">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="f9b13-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="f9b13-143">Response</span></span>
<span data-ttu-id="f9b13-144">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f9b13-144">If successful, this method returns a `200 OK` response code and an updated [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9b13-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f9b13-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="f9b13-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f9b13-146">Request</span></span>
<span data-ttu-id="f9b13-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f9b13-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f9b13-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="f9b13-148">Response</span></span>
<span data-ttu-id="f9b13-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f9b13-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





