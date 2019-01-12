---
title: Erstellen von „iosVppEBookAssignment“
description: Diese Methode erstellt ein neues Objekt des Typs iosVppEBookAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b5ff460b702c943268d9992bd17e99fd54369548
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963969"
---
# <a name="create-iosvppebookassignment"></a><span data-ttu-id="c3d28-103">Erstellen von „iosVppEBookAssignment“</span><span class="sxs-lookup"><span data-stu-id="c3d28-103">Create iosVppEBookAssignment</span></span>

> <span data-ttu-id="c3d28-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c3d28-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c3d28-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c3d28-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c3d28-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c3d28-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c3d28-107">Diese Methode erstellt ein neues Objekt des Typs [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c3d28-107">Create a new [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c3d28-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c3d28-108">Prerequisites</span></span>
<span data-ttu-id="c3d28-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3d28-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3d28-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c3d28-111">Permission type</span></span>|<span data-ttu-id="c3d28-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c3d28-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3d28-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c3d28-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c3d28-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3d28-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c3d28-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c3d28-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3d28-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c3d28-116">Not supported.</span></span>|
|<span data-ttu-id="c3d28-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c3d28-117">Application</span></span>|<span data-ttu-id="c3d28-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c3d28-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3d28-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c3d28-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="c3d28-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c3d28-120">Request headers</span></span>
|<span data-ttu-id="c3d28-121">Header</span><span class="sxs-lookup"><span data-stu-id="c3d28-121">Header</span></span>|<span data-ttu-id="c3d28-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c3d28-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3d28-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3d28-123">Authorization</span></span>|<span data-ttu-id="c3d28-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c3d28-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3d28-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c3d28-125">Accept</span></span>|<span data-ttu-id="c3d28-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c3d28-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3d28-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c3d28-127">Request body</span></span>
<span data-ttu-id="c3d28-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „iosVppEBookAssignment“ an.</span><span class="sxs-lookup"><span data-stu-id="c3d28-128">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="c3d28-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „iosVppEBookAssignment“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="c3d28-129">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="c3d28-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c3d28-130">Property</span></span>|<span data-ttu-id="c3d28-131">Typ</span><span class="sxs-lookup"><span data-stu-id="c3d28-131">Type</span></span>|<span data-ttu-id="c3d28-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c3d28-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3d28-133">id</span><span class="sxs-lookup"><span data-stu-id="c3d28-133">id</span></span>|<span data-ttu-id="c3d28-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c3d28-134">String</span></span>|<span data-ttu-id="c3d28-135">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="c3d28-135">Key of the entity.</span></span> <span data-ttu-id="c3d28-136">Geerbt von [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c3d28-136">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="c3d28-137">target</span><span class="sxs-lookup"><span data-stu-id="c3d28-137">target</span></span>|[<span data-ttu-id="c3d28-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c3d28-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c3d28-139">Zuweisungsziel für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="c3d28-139">The assignment target for eBook.</span></span> <span data-ttu-id="c3d28-140">Geerbt von [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c3d28-140">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="c3d28-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="c3d28-141">installIntent</span></span>|[<span data-ttu-id="c3d28-142">installIntent</span><span class="sxs-lookup"><span data-stu-id="c3d28-142">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="c3d28-143">Installationspriorität für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="c3d28-143">The install intent for eBook.</span></span> <span data-ttu-id="c3d28-144">Geerbt von [ManagedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c3d28-144">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="c3d28-145">Mögliche Werte sind: `available`, `required`, `uninstall` und `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="c3d28-145">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="c3d28-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="c3d28-146">Response</span></span>
<span data-ttu-id="c3d28-147">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c3d28-147">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3d28-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c3d28-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="c3d28-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c3d28-149">Request</span></span>
<span data-ttu-id="c3d28-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c3d28-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
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

### <a name="response"></a><span data-ttu-id="c3d28-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="c3d28-151">Response</span></span>
<span data-ttu-id="c3d28-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c3d28-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





