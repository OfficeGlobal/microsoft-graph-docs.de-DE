---
title: Aktualisieren von „iosVppEBookAssignment“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs iosVppEBookAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0ad070245ee687d08e4b636d7ef6301c42f1a586
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405814"
---
# <a name="update-iosvppebookassignment"></a><span data-ttu-id="8274b-103">Aktualisieren von „iosVppEBookAssignment“</span><span class="sxs-lookup"><span data-stu-id="8274b-103">Update iosVppEBookAssignment</span></span>

> <span data-ttu-id="8274b-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="8274b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8274b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8274b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8274b-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8274b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8274b-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8274b-107">Update the properties of a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8274b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8274b-108">Prerequisites</span></span>
<span data-ttu-id="8274b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8274b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8274b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8274b-111">Permission type</span></span>|<span data-ttu-id="8274b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8274b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8274b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8274b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8274b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8274b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8274b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8274b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8274b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8274b-116">Not supported.</span></span>|
|<span data-ttu-id="8274b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8274b-117">Application</span></span>|<span data-ttu-id="8274b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8274b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8274b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8274b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="8274b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8274b-120">Request headers</span></span>
|<span data-ttu-id="8274b-121">Header</span><span class="sxs-lookup"><span data-stu-id="8274b-121">Header</span></span>|<span data-ttu-id="8274b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="8274b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8274b-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="8274b-123">Authorization</span></span>|<span data-ttu-id="8274b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8274b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8274b-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8274b-125">Accept</span></span>|<span data-ttu-id="8274b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8274b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8274b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8274b-127">Request body</span></span>
<span data-ttu-id="8274b-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="8274b-128">In the request body, supply a JSON representation for the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

<span data-ttu-id="8274b-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="8274b-129">The following table shows the properties that are required when you create the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span></span>

|<span data-ttu-id="8274b-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8274b-130">Property</span></span>|<span data-ttu-id="8274b-131">Typ</span><span class="sxs-lookup"><span data-stu-id="8274b-131">Type</span></span>|<span data-ttu-id="8274b-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8274b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8274b-133">id</span><span class="sxs-lookup"><span data-stu-id="8274b-133">id</span></span>|<span data-ttu-id="8274b-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8274b-134">String</span></span>|<span data-ttu-id="8274b-135">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="8274b-135">Key of the entity.</span></span> <span data-ttu-id="8274b-136">Geerbt von [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8274b-136">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="8274b-137">target</span><span class="sxs-lookup"><span data-stu-id="8274b-137">target</span></span>|[<span data-ttu-id="8274b-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8274b-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8274b-139">Zuweisungsziel für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="8274b-139">The assignment target for eBook.</span></span> <span data-ttu-id="8274b-140">Geerbt von [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8274b-140">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="8274b-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="8274b-141">installIntent</span></span>|[<span data-ttu-id="8274b-142">installIntent</span><span class="sxs-lookup"><span data-stu-id="8274b-142">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="8274b-143">Installationspriorität für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="8274b-143">The install intent for eBook.</span></span> <span data-ttu-id="8274b-144">Geerbt von [ManagedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8274b-144">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="8274b-145">Mögliche Werte sind: `available`, `required`, `uninstall` und `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="8274b-145">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="8274b-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="8274b-146">Response</span></span>
<span data-ttu-id="8274b-147">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8274b-147">If successful, this method returns a `200 OK` response code and an updated [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8274b-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8274b-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="8274b-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8274b-149">Request</span></span>
<span data-ttu-id="8274b-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8274b-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8274b-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="8274b-151">Response</span></span>
<span data-ttu-id="8274b-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8274b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




