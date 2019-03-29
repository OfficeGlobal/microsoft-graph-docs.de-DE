---
title: IntuneBrandingProfileAssignment aktualisieren
description: Aktualisieren der Eigenschaften eines intuneBrandingProfileAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e951ba830d60d1114c24f604e75d6afc55c83b1e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964521"
---
# <a name="update-intunebrandingprofileassignment"></a><span data-ttu-id="1c564-103">IntuneBrandingProfileAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1c564-103">Update intuneBrandingProfileAssignment</span></span>

> <span data-ttu-id="1c564-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1c564-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c564-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1c564-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c564-106">Aktualisieren der Eigenschaften eines [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="1c564-106">Update the properties of a [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c564-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1c564-107">Prerequisites</span></span>
<span data-ttu-id="1c564-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c564-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c564-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1c564-110">Permission type</span></span>|<span data-ttu-id="1c564-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1c564-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c564-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1c564-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1c564-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c564-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1c564-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1c564-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c564-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1c564-115">Not supported.</span></span>|
|<span data-ttu-id="1c564-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1c564-116">Application</span></span>|<span data-ttu-id="1c564-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1c564-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c564-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1c564-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="1c564-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1c564-119">Request headers</span></span>
|<span data-ttu-id="1c564-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1c564-120">Header</span></span>|<span data-ttu-id="1c564-121">Wert</span><span class="sxs-lookup"><span data-stu-id="1c564-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c564-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c564-122">Authorization</span></span>|<span data-ttu-id="1c564-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1c564-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c564-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1c564-124">Accept</span></span>|<span data-ttu-id="1c564-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1c564-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c564-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1c564-126">Request body</span></span>
<span data-ttu-id="1c564-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="1c564-127">In the request body, supply a JSON representation for the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

<span data-ttu-id="1c564-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="1c564-128">The following table shows the properties that are required when you create the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md).</span></span>

|<span data-ttu-id="1c564-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1c564-129">Property</span></span>|<span data-ttu-id="1c564-130">Typ</span><span class="sxs-lookup"><span data-stu-id="1c564-130">Type</span></span>|<span data-ttu-id="1c564-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1c564-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c564-132">id</span><span class="sxs-lookup"><span data-stu-id="1c564-132">id</span></span>|<span data-ttu-id="1c564-133">String</span><span class="sxs-lookup"><span data-stu-id="1c564-133">String</span></span>|<span data-ttu-id="1c564-134">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="1c564-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="1c564-135">target</span><span class="sxs-lookup"><span data-stu-id="1c564-135">target</span></span>|[<span data-ttu-id="1c564-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1c564-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1c564-137">Zuordnungsziel, dem das Branding-Profil zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="1c564-137">Assignment target that the branding profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="1c564-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="1c564-138">Response</span></span>
<span data-ttu-id="1c564-139">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1c564-139">If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c564-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1c564-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c564-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1c564-141">Request</span></span>
<span data-ttu-id="1c564-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1c564-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
Content-type: application/json
Content-length: 171

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="1c564-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="1c564-143">Response</span></span>
<span data-ttu-id="1c564-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1c564-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 220

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "id": "ee38a117-a117-ee38-17a1-38ee17a138ee",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




