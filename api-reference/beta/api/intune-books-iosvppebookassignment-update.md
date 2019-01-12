---
title: Aktualisieren von „iosVppEBookAssignment“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs iosVppEBookAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 272de2b88b930b8f55849e6a791dce6c77d1595c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27958376"
---
# <a name="update-iosvppebookassignment"></a><span data-ttu-id="96f21-103">Aktualisieren von „iosVppEBookAssignment“</span><span class="sxs-lookup"><span data-stu-id="96f21-103">Update iosVppEBookAssignment</span></span>

> <span data-ttu-id="96f21-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="96f21-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96f21-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="96f21-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="96f21-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="96f21-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="96f21-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="96f21-107">Update the properties of a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="96f21-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="96f21-108">Prerequisites</span></span>
<span data-ttu-id="96f21-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96f21-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96f21-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="96f21-111">Permission type</span></span>|<span data-ttu-id="96f21-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="96f21-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96f21-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="96f21-113">Delegated (work or school account)</span></span>|<span data-ttu-id="96f21-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96f21-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="96f21-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="96f21-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96f21-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="96f21-116">Not supported.</span></span>|
|<span data-ttu-id="96f21-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="96f21-117">Application</span></span>|<span data-ttu-id="96f21-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="96f21-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="96f21-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="96f21-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="96f21-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="96f21-120">Request headers</span></span>
|<span data-ttu-id="96f21-121">Header</span><span class="sxs-lookup"><span data-stu-id="96f21-121">Header</span></span>|<span data-ttu-id="96f21-122">Wert</span><span class="sxs-lookup"><span data-stu-id="96f21-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96f21-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="96f21-123">Authorization</span></span>|<span data-ttu-id="96f21-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="96f21-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96f21-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="96f21-125">Accept</span></span>|<span data-ttu-id="96f21-126">application/json</span><span class="sxs-lookup"><span data-stu-id="96f21-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96f21-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="96f21-127">Request body</span></span>
<span data-ttu-id="96f21-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="96f21-128">In the request body, supply a JSON representation for the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

<span data-ttu-id="96f21-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="96f21-129">The following table shows the properties that are required when you create the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span></span>

|<span data-ttu-id="96f21-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="96f21-130">Property</span></span>|<span data-ttu-id="96f21-131">Typ</span><span class="sxs-lookup"><span data-stu-id="96f21-131">Type</span></span>|<span data-ttu-id="96f21-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="96f21-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96f21-133">id</span><span class="sxs-lookup"><span data-stu-id="96f21-133">id</span></span>|<span data-ttu-id="96f21-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="96f21-134">String</span></span>|<span data-ttu-id="96f21-135">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="96f21-135">Key of the entity.</span></span> <span data-ttu-id="96f21-136">Geerbt von [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="96f21-136">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="96f21-137">target</span><span class="sxs-lookup"><span data-stu-id="96f21-137">target</span></span>|[<span data-ttu-id="96f21-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="96f21-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="96f21-139">Zuweisungsziel für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="96f21-139">The assignment target for eBook.</span></span> <span data-ttu-id="96f21-140">Geerbt von [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="96f21-140">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="96f21-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="96f21-141">installIntent</span></span>|[<span data-ttu-id="96f21-142">installIntent</span><span class="sxs-lookup"><span data-stu-id="96f21-142">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="96f21-143">Installationspriorität für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="96f21-143">The install intent for eBook.</span></span> <span data-ttu-id="96f21-144">Geerbt von [ManagedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="96f21-144">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="96f21-145">Mögliche Werte sind: `available`, `required`, `uninstall` und `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="96f21-145">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="96f21-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="96f21-146">Response</span></span>
<span data-ttu-id="96f21-147">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="96f21-147">If successful, this method returns a `200 OK` response code and an updated [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96f21-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="96f21-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="96f21-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="96f21-149">Request</span></span>
<span data-ttu-id="96f21-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="96f21-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="96f21-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="96f21-151">Response</span></span>
<span data-ttu-id="96f21-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="96f21-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





