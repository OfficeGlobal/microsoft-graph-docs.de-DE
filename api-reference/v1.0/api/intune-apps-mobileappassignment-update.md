---
title: Aktualisieren von „mobileAppAssignment“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs mobileAppAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2582bde394bb8b9e721e0205dc9c1f8ca96aa239
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256714"
---
# <a name="update-mobileappassignment"></a><span data-ttu-id="87b92-103">Aktualisieren von „mobileAppAssignment“</span><span class="sxs-lookup"><span data-stu-id="87b92-103">Update mobileAppAssignment</span></span>

> <span data-ttu-id="87b92-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="87b92-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87b92-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="87b92-105">Update the properties of a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87b92-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="87b92-106">Prerequisites</span></span>
<span data-ttu-id="87b92-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="87b92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="87b92-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="87b92-109">Permission type</span></span>|<span data-ttu-id="87b92-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="87b92-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87b92-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="87b92-111">Delegated (work or school account)</span></span>|<span data-ttu-id="87b92-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87b92-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="87b92-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="87b92-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87b92-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="87b92-114">Not supported.</span></span>|
|<span data-ttu-id="87b92-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="87b92-115">Application</span></span>|<span data-ttu-id="87b92-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="87b92-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87b92-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="87b92-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="87b92-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="87b92-118">Request headers</span></span>
|<span data-ttu-id="87b92-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="87b92-119">Header</span></span>|<span data-ttu-id="87b92-120">Wert</span><span class="sxs-lookup"><span data-stu-id="87b92-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87b92-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="87b92-121">Authorization</span></span>|<span data-ttu-id="87b92-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="87b92-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87b92-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="87b92-123">Accept</span></span>|<span data-ttu-id="87b92-124">application/json</span><span class="sxs-lookup"><span data-stu-id="87b92-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87b92-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="87b92-125">Request body</span></span>
<span data-ttu-id="87b92-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="87b92-126">In the request body, supply a JSON representation for the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

<span data-ttu-id="87b92-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="87b92-127">The following table shows the properties that are required when you create the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>

|<span data-ttu-id="87b92-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="87b92-128">Property</span></span>|<span data-ttu-id="87b92-129">Typ</span><span class="sxs-lookup"><span data-stu-id="87b92-129">Type</span></span>|<span data-ttu-id="87b92-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87b92-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87b92-131">id</span><span class="sxs-lookup"><span data-stu-id="87b92-131">id</span></span>|<span data-ttu-id="87b92-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="87b92-132">String</span></span>|<span data-ttu-id="87b92-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="87b92-133">Key of the entity.</span></span>|
|<span data-ttu-id="87b92-134">intent</span><span class="sxs-lookup"><span data-stu-id="87b92-134">intent</span></span>|[<span data-ttu-id="87b92-135">installIntent</span><span class="sxs-lookup"><span data-stu-id="87b92-135">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="87b92-136">Die vom Administrator definierte Installationspriorität. Mögliche Werte sind: `available`, `required`, `uninstall` und `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="87b92-136">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="87b92-137">target</span><span class="sxs-lookup"><span data-stu-id="87b92-137">target</span></span>|[<span data-ttu-id="87b92-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="87b92-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="87b92-139">Die vom Administrator definierte Zielgruppenzuordnung</span><span class="sxs-lookup"><span data-stu-id="87b92-139">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="87b92-140">settings</span><span class="sxs-lookup"><span data-stu-id="87b92-140">settings</span></span>|[<span data-ttu-id="87b92-141">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="87b92-141">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="87b92-142">Die vom Administrator definierten Einstellungen für die Zielgruppenzuordnung</span><span class="sxs-lookup"><span data-stu-id="87b92-142">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="87b92-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="87b92-143">Response</span></span>
<span data-ttu-id="87b92-144">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="87b92-144">If successful, this method returns a `200 OK` response code and an updated [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87b92-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="87b92-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="87b92-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="87b92-146">Request</span></span>
<span data-ttu-id="87b92-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="87b92-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
Content-type: application/json
Content-length: 273

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```

### <a name="response"></a><span data-ttu-id="87b92-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="87b92-148">Response</span></span>
<span data-ttu-id="87b92-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="87b92-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 322

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "591620b7-20b7-5916-b720-1659b7201659",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```



