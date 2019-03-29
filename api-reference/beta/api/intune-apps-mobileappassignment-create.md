---
title: Erstellen von „mobileAppAssignment“
description: Diese Methode erstellt ein neues Objekt des Typs mobileAppAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d42e1dde94037e932757f0d0c6202bcb10e3f540
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30985046"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="99bce-103">Erstellen von „mobileAppAssignment“</span><span class="sxs-lookup"><span data-stu-id="99bce-103">Create mobileAppAssignment</span></span>

> <span data-ttu-id="99bce-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="99bce-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99bce-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="99bce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99bce-106">Diese Methode erstellt ein neues Objekt des Typs [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="99bce-106">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99bce-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="99bce-107">Prerequisites</span></span>
<span data-ttu-id="99bce-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99bce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99bce-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="99bce-110">Permission type</span></span>|<span data-ttu-id="99bce-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="99bce-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99bce-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="99bce-112">Delegated (work or school account)</span></span>|<span data-ttu-id="99bce-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99bce-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="99bce-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="99bce-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99bce-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="99bce-115">Not supported.</span></span>|
|<span data-ttu-id="99bce-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="99bce-116">Application</span></span>|<span data-ttu-id="99bce-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="99bce-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="99bce-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="99bce-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="99bce-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="99bce-119">Request headers</span></span>
|<span data-ttu-id="99bce-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="99bce-120">Header</span></span>|<span data-ttu-id="99bce-121">Wert</span><span class="sxs-lookup"><span data-stu-id="99bce-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99bce-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="99bce-122">Authorization</span></span>|<span data-ttu-id="99bce-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="99bce-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99bce-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="99bce-124">Accept</span></span>|<span data-ttu-id="99bce-125">application/json</span><span class="sxs-lookup"><span data-stu-id="99bce-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99bce-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="99bce-126">Request body</span></span>
<span data-ttu-id="99bce-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „mobileAppAssignment“ an.</span><span class="sxs-lookup"><span data-stu-id="99bce-127">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="99bce-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „mobileAppAssignment“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="99bce-128">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="99bce-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="99bce-129">Property</span></span>|<span data-ttu-id="99bce-130">Typ</span><span class="sxs-lookup"><span data-stu-id="99bce-130">Type</span></span>|<span data-ttu-id="99bce-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="99bce-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99bce-132">id</span><span class="sxs-lookup"><span data-stu-id="99bce-132">id</span></span>|<span data-ttu-id="99bce-133">String</span><span class="sxs-lookup"><span data-stu-id="99bce-133">String</span></span>|<span data-ttu-id="99bce-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="99bce-134">Key of the entity.</span></span>|
|<span data-ttu-id="99bce-135">intent</span><span class="sxs-lookup"><span data-stu-id="99bce-135">intent</span></span>|[<span data-ttu-id="99bce-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="99bce-136">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="99bce-137">Die vom Administrator definierte Installationspriorität. Mögliche Werte sind: `available`, `required`, `uninstall` und `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="99bce-137">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="99bce-138">target</span><span class="sxs-lookup"><span data-stu-id="99bce-138">target</span></span>|[<span data-ttu-id="99bce-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="99bce-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="99bce-140">Die vom Administrator definierte Zielgruppenzuordnung</span><span class="sxs-lookup"><span data-stu-id="99bce-140">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="99bce-141">settings</span><span class="sxs-lookup"><span data-stu-id="99bce-141">settings</span></span>|[<span data-ttu-id="99bce-142">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="99bce-142">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="99bce-143">Die vom Administrator definierten Einstellungen für die Zielgruppenzuordnung</span><span class="sxs-lookup"><span data-stu-id="99bce-143">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="99bce-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="99bce-144">Response</span></span>
<span data-ttu-id="99bce-145">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="99bce-145">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99bce-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="99bce-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="99bce-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="99bce-147">Request</span></span>
<span data-ttu-id="99bce-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="99bce-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="99bce-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="99bce-149">Response</span></span>
<span data-ttu-id="99bce-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="99bce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




