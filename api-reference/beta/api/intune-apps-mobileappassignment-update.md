---
title: Aktualisieren von „mobileAppAssignment“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs mobileAppAssignment.
author: tfitzmac
ms.openlocfilehash: ee6a6de3d20257121721ccb94f316230db8112d2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361117"
---
# <a name="update-mobileappassignment"></a><span data-ttu-id="d48c4-103">Aktualisieren von „mobileAppAssignment“</span><span class="sxs-lookup"><span data-stu-id="d48c4-103">Update mobileAppAssignment</span></span>

> <span data-ttu-id="d48c4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d48c4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d48c4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d48c4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d48c4-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d48c4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d48c4-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d48c4-107">Update the properties of a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d48c4-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d48c4-108">Prerequisites</span></span>
<span data-ttu-id="d48c4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d48c4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d48c4-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d48c4-111">Permission type</span></span>|<span data-ttu-id="d48c4-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d48c4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d48c4-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d48c4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d48c4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d48c4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d48c4-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d48c4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d48c4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d48c4-116">Not supported.</span></span>|
|<span data-ttu-id="d48c4-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d48c4-117">Application</span></span>|<span data-ttu-id="d48c4-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d48c4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d48c4-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d48c4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="d48c4-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d48c4-120">Request headers</span></span>
|<span data-ttu-id="d48c4-121">Header</span><span class="sxs-lookup"><span data-stu-id="d48c4-121">Header</span></span>|<span data-ttu-id="d48c4-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d48c4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d48c4-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="d48c4-123">Authorization</span></span>|<span data-ttu-id="d48c4-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d48c4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d48c4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d48c4-125">Accept</span></span>|<span data-ttu-id="d48c4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d48c4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d48c4-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d48c4-127">Request body</span></span>
<span data-ttu-id="d48c4-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="d48c4-128">In the request body, supply a JSON representation for the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

<span data-ttu-id="d48c4-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="d48c4-129">The following table shows the properties that are required when you create the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>

|<span data-ttu-id="d48c4-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d48c4-130">Property</span></span>|<span data-ttu-id="d48c4-131">Typ</span><span class="sxs-lookup"><span data-stu-id="d48c4-131">Type</span></span>|<span data-ttu-id="d48c4-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d48c4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d48c4-133">id</span><span class="sxs-lookup"><span data-stu-id="d48c4-133">id</span></span>|<span data-ttu-id="d48c4-134">String</span><span class="sxs-lookup"><span data-stu-id="d48c4-134">String</span></span>|<span data-ttu-id="d48c4-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d48c4-135">Key of the entity.</span></span>|
|<span data-ttu-id="d48c4-136">intent</span><span class="sxs-lookup"><span data-stu-id="d48c4-136">intent</span></span>|[<span data-ttu-id="d48c4-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="d48c4-137">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="d48c4-138">Die vom Administrator definierte Installationspriorität. Mögliche Werte sind: `available`, `required`, `uninstall` und `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="d48c4-138">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="d48c4-139">target</span><span class="sxs-lookup"><span data-stu-id="d48c4-139">target</span></span>|[<span data-ttu-id="d48c4-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d48c4-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d48c4-141">Die vom Administrator definierte Zielgruppenzuordnung</span><span class="sxs-lookup"><span data-stu-id="d48c4-141">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="d48c4-142">settings</span><span class="sxs-lookup"><span data-stu-id="d48c4-142">settings</span></span>|[<span data-ttu-id="d48c4-143">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="d48c4-143">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="d48c4-144">Die vom Administrator definierten Einstellungen für die Zielgruppenzuordnung</span><span class="sxs-lookup"><span data-stu-id="d48c4-144">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="d48c4-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="d48c4-145">Response</span></span>
<span data-ttu-id="d48c4-146">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d48c4-146">If successful, this method returns a `200 OK` response code and an updated [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d48c4-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d48c4-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="d48c4-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d48c4-148">Request</span></span>
<span data-ttu-id="d48c4-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d48c4-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
Content-type: application/json
Content-length: 215

{
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```

### <a name="response"></a><span data-ttu-id="d48c4-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="d48c4-150">Response</span></span>
<span data-ttu-id="d48c4-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d48c4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





