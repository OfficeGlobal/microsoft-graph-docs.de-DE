---
title: Aktualisieren von „mobileAppAssignment“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs mobileAppAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e46df43d27e35d4d9c88a6520761d737b8bf720c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887269"
---
# <a name="update-mobileappassignment"></a><span data-ttu-id="ef162-103">Aktualisieren von „mobileAppAssignment“</span><span class="sxs-lookup"><span data-stu-id="ef162-103">Update mobileAppAssignment</span></span>

> <span data-ttu-id="ef162-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ef162-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ef162-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ef162-105">Update the properties of a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ef162-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ef162-106">Prerequisites</span></span>
<span data-ttu-id="ef162-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef162-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef162-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ef162-109">Permission type</span></span>|<span data-ttu-id="ef162-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ef162-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef162-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ef162-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ef162-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef162-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ef162-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ef162-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef162-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ef162-114">Not supported.</span></span>|
|<span data-ttu-id="ef162-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ef162-115">Application</span></span>|<span data-ttu-id="ef162-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ef162-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef162-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ef162-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="ef162-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ef162-118">Request headers</span></span>
|<span data-ttu-id="ef162-119">Header</span><span class="sxs-lookup"><span data-stu-id="ef162-119">Header</span></span>|<span data-ttu-id="ef162-120">Wert</span><span class="sxs-lookup"><span data-stu-id="ef162-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef162-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef162-121">Authorization</span></span>|<span data-ttu-id="ef162-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ef162-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef162-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ef162-123">Accept</span></span>|<span data-ttu-id="ef162-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ef162-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef162-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ef162-125">Request body</span></span>
<span data-ttu-id="ef162-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="ef162-126">In the request body, supply a JSON representation for the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

<span data-ttu-id="ef162-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="ef162-127">The following table shows the properties that are required when you create the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>

|<span data-ttu-id="ef162-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ef162-128">Property</span></span>|<span data-ttu-id="ef162-129">Typ</span><span class="sxs-lookup"><span data-stu-id="ef162-129">Type</span></span>|<span data-ttu-id="ef162-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ef162-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef162-131">id</span><span class="sxs-lookup"><span data-stu-id="ef162-131">id</span></span>|<span data-ttu-id="ef162-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ef162-132">String</span></span>|<span data-ttu-id="ef162-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ef162-133">Key of the entity.</span></span>|
|<span data-ttu-id="ef162-134">intent</span><span class="sxs-lookup"><span data-stu-id="ef162-134">intent</span></span>|[<span data-ttu-id="ef162-135">installIntent</span><span class="sxs-lookup"><span data-stu-id="ef162-135">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="ef162-136">Die vom Administrator definierte Installationspriorität. Mögliche Werte sind: `available`, `required`, `uninstall` und `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="ef162-136">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="ef162-137">target</span><span class="sxs-lookup"><span data-stu-id="ef162-137">target</span></span>|[<span data-ttu-id="ef162-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ef162-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ef162-139">Die vom Administrator definierte Zielgruppenzuordnung</span><span class="sxs-lookup"><span data-stu-id="ef162-139">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="ef162-140">settings</span><span class="sxs-lookup"><span data-stu-id="ef162-140">settings</span></span>|[<span data-ttu-id="ef162-141">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="ef162-141">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="ef162-142">Die vom Administrator definierten Einstellungen für die Zielgruppenzuordnung</span><span class="sxs-lookup"><span data-stu-id="ef162-142">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="ef162-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="ef162-143">Response</span></span>
<span data-ttu-id="ef162-144">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ef162-144">If successful, this method returns a `200 OK` response code and an updated [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef162-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ef162-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="ef162-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ef162-146">Request</span></span>
<span data-ttu-id="ef162-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ef162-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ef162-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="ef162-148">Response</span></span>
<span data-ttu-id="ef162-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ef162-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



