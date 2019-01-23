---
title: Aktualisieren von „mobileAppAssignment“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs mobileAppAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bbedecc237e56022351fef82853fc3c2cb14bb91
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424322"
---
# <a name="update-mobileappassignment"></a><span data-ttu-id="13af1-103">Aktualisieren von „mobileAppAssignment“</span><span class="sxs-lookup"><span data-stu-id="13af1-103">Update mobileAppAssignment</span></span>

> <span data-ttu-id="13af1-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="13af1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="13af1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="13af1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="13af1-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="13af1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13af1-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="13af1-107">Update the properties of a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13af1-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="13af1-108">Prerequisites</span></span>
<span data-ttu-id="13af1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="13af1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="13af1-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="13af1-111">Permission type</span></span>|<span data-ttu-id="13af1-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="13af1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13af1-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="13af1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="13af1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13af1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="13af1-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="13af1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13af1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="13af1-116">Not supported.</span></span>|
|<span data-ttu-id="13af1-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="13af1-117">Application</span></span>|<span data-ttu-id="13af1-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="13af1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13af1-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="13af1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="13af1-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="13af1-120">Request headers</span></span>
|<span data-ttu-id="13af1-121">Header</span><span class="sxs-lookup"><span data-stu-id="13af1-121">Header</span></span>|<span data-ttu-id="13af1-122">Wert</span><span class="sxs-lookup"><span data-stu-id="13af1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13af1-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="13af1-123">Authorization</span></span>|<span data-ttu-id="13af1-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="13af1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13af1-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="13af1-125">Accept</span></span>|<span data-ttu-id="13af1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="13af1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13af1-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="13af1-127">Request body</span></span>
<span data-ttu-id="13af1-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="13af1-128">In the request body, supply a JSON representation for the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

<span data-ttu-id="13af1-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="13af1-129">The following table shows the properties that are required when you create the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>

|<span data-ttu-id="13af1-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="13af1-130">Property</span></span>|<span data-ttu-id="13af1-131">Typ</span><span class="sxs-lookup"><span data-stu-id="13af1-131">Type</span></span>|<span data-ttu-id="13af1-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="13af1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13af1-133">id</span><span class="sxs-lookup"><span data-stu-id="13af1-133">id</span></span>|<span data-ttu-id="13af1-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13af1-134">String</span></span>|<span data-ttu-id="13af1-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="13af1-135">Key of the entity.</span></span>|
|<span data-ttu-id="13af1-136">intent</span><span class="sxs-lookup"><span data-stu-id="13af1-136">intent</span></span>|[<span data-ttu-id="13af1-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="13af1-137">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="13af1-138">Die vom Administrator definierte Installationspriorität. Mögliche Werte sind: `available`, `required`, `uninstall` und `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="13af1-138">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="13af1-139">target</span><span class="sxs-lookup"><span data-stu-id="13af1-139">target</span></span>|[<span data-ttu-id="13af1-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="13af1-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="13af1-141">Die vom Administrator definierte Zielgruppenzuordnung</span><span class="sxs-lookup"><span data-stu-id="13af1-141">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="13af1-142">settings</span><span class="sxs-lookup"><span data-stu-id="13af1-142">settings</span></span>|[<span data-ttu-id="13af1-143">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="13af1-143">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="13af1-144">Die vom Administrator definierten Einstellungen für die Zielgruppenzuordnung</span><span class="sxs-lookup"><span data-stu-id="13af1-144">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="13af1-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="13af1-145">Response</span></span>
<span data-ttu-id="13af1-146">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="13af1-146">If successful, this method returns a `200 OK` response code and an updated [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13af1-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="13af1-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="13af1-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="13af1-148">Request</span></span>
<span data-ttu-id="13af1-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="13af1-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
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

### <a name="response"></a><span data-ttu-id="13af1-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="13af1-150">Response</span></span>
<span data-ttu-id="13af1-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="13af1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




