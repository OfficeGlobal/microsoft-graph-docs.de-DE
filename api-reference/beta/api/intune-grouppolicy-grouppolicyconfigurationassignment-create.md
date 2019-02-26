---
title: GroupPolicyConfigurationAssignment erstellen
description: Erstellen eines neuen groupPolicyConfigurationAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 783a84466ecdee5cb4e5250338426b19d9c4f005
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146550"
---
# <a name="create-grouppolicyconfigurationassignment"></a><span data-ttu-id="b908f-103">GroupPolicyConfigurationAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="b908f-103">Create groupPolicyConfigurationAssignment</span></span>

> <span data-ttu-id="b908f-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b908f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b908f-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b908f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b908f-106">Erstellen eines neuen [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b908f-106">Create a new [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b908f-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b908f-107">Prerequisites</span></span>
<span data-ttu-id="b908f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b908f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b908f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b908f-110">Permission type</span></span>|<span data-ttu-id="b908f-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b908f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b908f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b908f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b908f-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b908f-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b908f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b908f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b908f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b908f-115">Not supported.</span></span>|
|<span data-ttu-id="b908f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b908f-116">Application</span></span>|<span data-ttu-id="b908f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b908f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b908f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b908f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="b908f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b908f-119">Request headers</span></span>
|<span data-ttu-id="b908f-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b908f-120">Header</span></span>|<span data-ttu-id="b908f-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b908f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b908f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b908f-122">Authorization</span></span>|<span data-ttu-id="b908f-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b908f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b908f-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b908f-124">Accept</span></span>|<span data-ttu-id="b908f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b908f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b908f-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b908f-126">Request body</span></span>
<span data-ttu-id="b908f-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das groupPolicyConfigurationAssignment-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="b908f-127">In the request body, supply a JSON representation for the groupPolicyConfigurationAssignment object.</span></span>

<span data-ttu-id="b908f-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der groupPolicyConfigurationAssignment erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b908f-128">The following table shows the properties that are required when you create the groupPolicyConfigurationAssignment.</span></span>

|<span data-ttu-id="b908f-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b908f-129">Property</span></span>|<span data-ttu-id="b908f-130">Typ</span><span class="sxs-lookup"><span data-stu-id="b908f-130">Type</span></span>|<span data-ttu-id="b908f-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b908f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b908f-132">id</span><span class="sxs-lookup"><span data-stu-id="b908f-132">id</span></span>|<span data-ttu-id="b908f-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b908f-133">String</span></span>|<span data-ttu-id="b908f-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b908f-134">Key of the entity.</span></span>|
|<span data-ttu-id="b908f-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b908f-135">lastModifiedDateTime</span></span>|<span data-ttu-id="b908f-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b908f-136">DateTimeOffset</span></span>|<span data-ttu-id="b908f-137">Datum und Uhrzeit der letzten Änderung der Entität.</span><span class="sxs-lookup"><span data-stu-id="b908f-137">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="b908f-138">target</span><span class="sxs-lookup"><span data-stu-id="b908f-138">target</span></span>|[<span data-ttu-id="b908f-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b908f-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b908f-140">Der Typ der Gruppen, die für die Gruppenrichtlinienkonfiguration vorgesehen sind.</span><span class="sxs-lookup"><span data-stu-id="b908f-140">The type of groups targeted the group policy configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="b908f-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="b908f-141">Response</span></span>
<span data-ttu-id="b908f-142">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b908f-142">If successful, this method returns a `201 Created` response code and a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b908f-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b908f-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="b908f-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b908f-144">Request</span></span>
<span data-ttu-id="b908f-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b908f-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments
Content-type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="b908f-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="b908f-146">Response</span></span>
<span data-ttu-id="b908f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b908f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




