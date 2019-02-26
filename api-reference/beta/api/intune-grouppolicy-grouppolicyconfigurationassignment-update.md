---
title: GroupPolicyConfigurationAssignment aktualisieren
description: Aktualisieren der Eigenschaften eines groupPolicyConfigurationAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b42d594f45f7e88ae4d532397455954b9e9095c2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157540"
---
# <a name="update-grouppolicyconfigurationassignment"></a><span data-ttu-id="2a0c8-103">GroupPolicyConfigurationAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2a0c8-103">Update groupPolicyConfigurationAssignment</span></span>

> <span data-ttu-id="2a0c8-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2a0c8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a0c8-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2a0c8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a0c8-106">Aktualisieren der Eigenschaften eines [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="2a0c8-106">Update the properties of a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a0c8-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2a0c8-107">Prerequisites</span></span>
<span data-ttu-id="2a0c8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2a0c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2a0c8-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2a0c8-110">Permission type</span></span>|<span data-ttu-id="2a0c8-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2a0c8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a0c8-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2a0c8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2a0c8-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a0c8-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2a0c8-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2a0c8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a0c8-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2a0c8-115">Not supported.</span></span>|
|<span data-ttu-id="2a0c8-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2a0c8-116">Application</span></span>|<span data-ttu-id="2a0c8-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2a0c8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a0c8-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a0c8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments/{groupPolicyConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="2a0c8-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2a0c8-119">Request headers</span></span>
|<span data-ttu-id="2a0c8-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2a0c8-120">Header</span></span>|<span data-ttu-id="2a0c8-121">Wert</span><span class="sxs-lookup"><span data-stu-id="2a0c8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a0c8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a0c8-122">Authorization</span></span>|<span data-ttu-id="2a0c8-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2a0c8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a0c8-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2a0c8-124">Accept</span></span>|<span data-ttu-id="2a0c8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2a0c8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a0c8-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2a0c8-126">Request body</span></span>
<span data-ttu-id="2a0c8-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="2a0c8-127">In the request body, supply a JSON representation for the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

<span data-ttu-id="2a0c8-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="2a0c8-128">The following table shows the properties that are required when you create the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>

|<span data-ttu-id="2a0c8-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2a0c8-129">Property</span></span>|<span data-ttu-id="2a0c8-130">Typ</span><span class="sxs-lookup"><span data-stu-id="2a0c8-130">Type</span></span>|<span data-ttu-id="2a0c8-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2a0c8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a0c8-132">id</span><span class="sxs-lookup"><span data-stu-id="2a0c8-132">id</span></span>|<span data-ttu-id="2a0c8-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2a0c8-133">String</span></span>|<span data-ttu-id="2a0c8-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="2a0c8-134">Key of the entity.</span></span>|
|<span data-ttu-id="2a0c8-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2a0c8-135">lastModifiedDateTime</span></span>|<span data-ttu-id="2a0c8-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a0c8-136">DateTimeOffset</span></span>|<span data-ttu-id="2a0c8-137">Datum und Uhrzeit der letzten Änderung der Entität.</span><span class="sxs-lookup"><span data-stu-id="2a0c8-137">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="2a0c8-138">target</span><span class="sxs-lookup"><span data-stu-id="2a0c8-138">target</span></span>|[<span data-ttu-id="2a0c8-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2a0c8-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2a0c8-140">Der Typ der Gruppen, die für die Gruppenrichtlinienkonfiguration vorgesehen sind.</span><span class="sxs-lookup"><span data-stu-id="2a0c8-140">The type of groups targeted the group policy configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="2a0c8-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a0c8-141">Response</span></span>
<span data-ttu-id="2a0c8-142">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2a0c8-142">If successful, this method returns a `200 OK` response code and an updated [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a0c8-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2a0c8-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a0c8-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a0c8-144">Request</span></span>
<span data-ttu-id="2a0c8-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2a0c8-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments/{groupPolicyConfigurationAssignmentId}
Content-type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="2a0c8-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a0c8-146">Response</span></span>
<span data-ttu-id="2a0c8-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2a0c8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 287

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




