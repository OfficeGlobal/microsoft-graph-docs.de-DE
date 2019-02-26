---
title: Erstellen von „mobileAppAssignment“
description: Diese Methode erstellt ein neues Objekt des Typs mobileAppAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ee72f668dacebe8c5567b57453fe5ef70b8f6540
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261138"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="b27df-103">Erstellen von „mobileAppAssignment“</span><span class="sxs-lookup"><span data-stu-id="b27df-103">Create mobileAppAssignment</span></span>

> <span data-ttu-id="b27df-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b27df-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b27df-105">Diese Methode erstellt ein neues Objekt des Typs [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b27df-105">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b27df-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b27df-106">Prerequisites</span></span>
<span data-ttu-id="b27df-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b27df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b27df-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b27df-109">Permission type</span></span>|<span data-ttu-id="b27df-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b27df-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b27df-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b27df-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b27df-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b27df-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b27df-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b27df-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b27df-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b27df-114">Not supported.</span></span>|
|<span data-ttu-id="b27df-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b27df-115">Application</span></span>|<span data-ttu-id="b27df-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b27df-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b27df-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b27df-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="b27df-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b27df-118">Request headers</span></span>
|<span data-ttu-id="b27df-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b27df-119">Header</span></span>|<span data-ttu-id="b27df-120">Wert</span><span class="sxs-lookup"><span data-stu-id="b27df-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b27df-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b27df-121">Authorization</span></span>|<span data-ttu-id="b27df-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b27df-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b27df-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b27df-123">Accept</span></span>|<span data-ttu-id="b27df-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b27df-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b27df-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b27df-125">Request body</span></span>
<span data-ttu-id="b27df-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „mobileAppAssignment“ an.</span><span class="sxs-lookup"><span data-stu-id="b27df-126">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="b27df-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „mobileAppAssignment“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="b27df-127">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="b27df-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b27df-128">Property</span></span>|<span data-ttu-id="b27df-129">Typ</span><span class="sxs-lookup"><span data-stu-id="b27df-129">Type</span></span>|<span data-ttu-id="b27df-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b27df-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b27df-131">id</span><span class="sxs-lookup"><span data-stu-id="b27df-131">id</span></span>|<span data-ttu-id="b27df-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b27df-132">String</span></span>|<span data-ttu-id="b27df-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b27df-133">Key of the entity.</span></span>|
|<span data-ttu-id="b27df-134">intent</span><span class="sxs-lookup"><span data-stu-id="b27df-134">intent</span></span>|[<span data-ttu-id="b27df-135">installIntent</span><span class="sxs-lookup"><span data-stu-id="b27df-135">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="b27df-136">Die vom Administrator definierte Installationspriorität. Mögliche Werte sind: `available`, `required`, `uninstall` und `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="b27df-136">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="b27df-137">target</span><span class="sxs-lookup"><span data-stu-id="b27df-137">target</span></span>|[<span data-ttu-id="b27df-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b27df-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b27df-139">Die vom Administrator definierte Zielgruppenzuordnung</span><span class="sxs-lookup"><span data-stu-id="b27df-139">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="b27df-140">settings</span><span class="sxs-lookup"><span data-stu-id="b27df-140">settings</span></span>|[<span data-ttu-id="b27df-141">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="b27df-141">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="b27df-142">Die vom Administrator definierten Einstellungen für die Zielgruppenzuordnung</span><span class="sxs-lookup"><span data-stu-id="b27df-142">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="b27df-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="b27df-143">Response</span></span>
<span data-ttu-id="b27df-144">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b27df-144">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b27df-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b27df-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="b27df-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b27df-146">Request</span></span>
<span data-ttu-id="b27df-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b27df-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments
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

### <a name="response"></a><span data-ttu-id="b27df-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="b27df-148">Response</span></span>
<span data-ttu-id="b27df-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b27df-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



