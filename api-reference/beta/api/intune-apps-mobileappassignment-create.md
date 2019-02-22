---
title: Erstellen von „mobileAppAssignment“
description: Diese Methode erstellt ein neues Objekt des Typs mobileAppAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7abf1163d5d323bf460b0a8dab3b54eb7ef8a2f8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156700"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="95f9a-103">Erstellen von „mobileAppAssignment“</span><span class="sxs-lookup"><span data-stu-id="95f9a-103">Create mobileAppAssignment</span></span>

> <span data-ttu-id="95f9a-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="95f9a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95f9a-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="95f9a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95f9a-106">Diese Methode erstellt ein neues Objekt des Typs [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="95f9a-106">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95f9a-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="95f9a-107">Prerequisites</span></span>
<span data-ttu-id="95f9a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="95f9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="95f9a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="95f9a-110">Permission type</span></span>|<span data-ttu-id="95f9a-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="95f9a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95f9a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="95f9a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="95f9a-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95f9a-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="95f9a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="95f9a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95f9a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="95f9a-115">Not supported.</span></span>|
|<span data-ttu-id="95f9a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="95f9a-116">Application</span></span>|<span data-ttu-id="95f9a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="95f9a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95f9a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="95f9a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="95f9a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="95f9a-119">Request headers</span></span>
|<span data-ttu-id="95f9a-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="95f9a-120">Header</span></span>|<span data-ttu-id="95f9a-121">Wert</span><span class="sxs-lookup"><span data-stu-id="95f9a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95f9a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="95f9a-122">Authorization</span></span>|<span data-ttu-id="95f9a-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="95f9a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95f9a-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="95f9a-124">Accept</span></span>|<span data-ttu-id="95f9a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="95f9a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95f9a-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="95f9a-126">Request body</span></span>
<span data-ttu-id="95f9a-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „mobileAppAssignment“ an.</span><span class="sxs-lookup"><span data-stu-id="95f9a-127">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="95f9a-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „mobileAppAssignment“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="95f9a-128">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="95f9a-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="95f9a-129">Property</span></span>|<span data-ttu-id="95f9a-130">Typ</span><span class="sxs-lookup"><span data-stu-id="95f9a-130">Type</span></span>|<span data-ttu-id="95f9a-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="95f9a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95f9a-132">id</span><span class="sxs-lookup"><span data-stu-id="95f9a-132">id</span></span>|<span data-ttu-id="95f9a-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="95f9a-133">String</span></span>|<span data-ttu-id="95f9a-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="95f9a-134">Key of the entity.</span></span>|
|<span data-ttu-id="95f9a-135">intent</span><span class="sxs-lookup"><span data-stu-id="95f9a-135">intent</span></span>|[<span data-ttu-id="95f9a-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="95f9a-136">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="95f9a-137">Die vom Administrator definierte Installationspriorität. Mögliche Werte sind: `available`, `required`, `uninstall` und `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="95f9a-137">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="95f9a-138">target</span><span class="sxs-lookup"><span data-stu-id="95f9a-138">target</span></span>|[<span data-ttu-id="95f9a-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="95f9a-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="95f9a-140">Die vom Administrator definierte Zielgruppenzuordnung</span><span class="sxs-lookup"><span data-stu-id="95f9a-140">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="95f9a-141">settings</span><span class="sxs-lookup"><span data-stu-id="95f9a-141">settings</span></span>|[<span data-ttu-id="95f9a-142">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="95f9a-142">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="95f9a-143">Die vom Administrator definierten Einstellungen für die Zielgruppenzuordnung</span><span class="sxs-lookup"><span data-stu-id="95f9a-143">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="95f9a-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="95f9a-144">Response</span></span>
<span data-ttu-id="95f9a-145">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="95f9a-145">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95f9a-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="95f9a-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="95f9a-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="95f9a-147">Request</span></span>
<span data-ttu-id="95f9a-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="95f9a-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments
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

### <a name="response"></a><span data-ttu-id="95f9a-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="95f9a-149">Response</span></span>
<span data-ttu-id="95f9a-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="95f9a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




