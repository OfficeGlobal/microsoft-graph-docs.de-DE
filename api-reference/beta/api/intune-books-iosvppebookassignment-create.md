---
title: Erstellen von „iosVppEBookAssignment“
description: Diese Methode erstellt ein neues Objekt des Typs iosVppEBookAssignment.
ms.openlocfilehash: 192f5e006fa89f3dbf25a320967af68fbd06f7ef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063409"
---
# <a name="create-iosvppebookassignment"></a><span data-ttu-id="079c8-103">Erstellen von „iosVppEBookAssignment“</span><span class="sxs-lookup"><span data-stu-id="079c8-103">Create iosVppEBookAssignment</span></span>

> <span data-ttu-id="079c8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="079c8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="079c8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="079c8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="079c8-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="079c8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="079c8-107">Diese Methode erstellt ein neues Objekt des Typs [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="079c8-107">Create a new [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="079c8-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="079c8-108">Prerequisites</span></span>
<span data-ttu-id="079c8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="079c8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="079c8-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="079c8-111">Permission type</span></span>|<span data-ttu-id="079c8-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="079c8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="079c8-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="079c8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="079c8-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="079c8-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="079c8-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="079c8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="079c8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="079c8-116">Not supported.</span></span>|
|<span data-ttu-id="079c8-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="079c8-117">Application</span></span>|<span data-ttu-id="079c8-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="079c8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="079c8-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="079c8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="079c8-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="079c8-120">Request headers</span></span>
|<span data-ttu-id="079c8-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="079c8-121">Header</span></span>|<span data-ttu-id="079c8-122">Wert</span><span class="sxs-lookup"><span data-stu-id="079c8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="079c8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="079c8-123">Authorization</span></span>|<span data-ttu-id="079c8-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="079c8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="079c8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="079c8-125">Accept</span></span>|<span data-ttu-id="079c8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="079c8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="079c8-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="079c8-127">Request body</span></span>
<span data-ttu-id="079c8-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „iosVppEBookAssignment“ an.</span><span class="sxs-lookup"><span data-stu-id="079c8-128">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="079c8-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „iosVppEBookAssignment“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="079c8-129">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="079c8-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="079c8-130">Property</span></span>|<span data-ttu-id="079c8-131">Typ</span><span class="sxs-lookup"><span data-stu-id="079c8-131">Type</span></span>|<span data-ttu-id="079c8-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="079c8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="079c8-133">id</span><span class="sxs-lookup"><span data-stu-id="079c8-133">id</span></span>|<span data-ttu-id="079c8-134">String</span><span class="sxs-lookup"><span data-stu-id="079c8-134">String</span></span>|<span data-ttu-id="079c8-135">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="079c8-135">Key of the entity.</span></span> <span data-ttu-id="079c8-136">Geerbt von [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="079c8-136">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="079c8-137">target</span><span class="sxs-lookup"><span data-stu-id="079c8-137">target</span></span>|[<span data-ttu-id="079c8-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="079c8-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="079c8-139">Zuweisungsziel für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="079c8-139">The assignment target for eBook.</span></span> <span data-ttu-id="079c8-140">Geerbt von [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="079c8-140">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="079c8-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="079c8-141">installIntent</span></span>|[<span data-ttu-id="079c8-142">installIntent</span><span class="sxs-lookup"><span data-stu-id="079c8-142">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="079c8-143">Installationspriorität für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="079c8-143">The install intent for eBook.</span></span> <span data-ttu-id="079c8-144">Geerbt von [ManagedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="079c8-144">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="079c8-145">Mögliche Werte sind: `available`, `required`, `uninstall` und `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="079c8-145">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="079c8-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="079c8-146">Response</span></span>
<span data-ttu-id="079c8-147">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="079c8-147">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="079c8-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="079c8-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="079c8-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="079c8-149">Request</span></span>
<span data-ttu-id="079c8-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="079c8-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="079c8-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="079c8-151">Response</span></span>
<span data-ttu-id="079c8-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="079c8-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





