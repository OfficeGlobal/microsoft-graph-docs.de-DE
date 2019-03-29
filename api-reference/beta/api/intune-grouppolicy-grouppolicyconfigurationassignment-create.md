---
title: GroupPolicyConfigurationAssignment erstellen
description: Erstellen eines neuen groupPolicyConfigurationAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 44ce089e1a0f5e6b7bee4c2c19a85b5aca1e3bdc
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30959208"
---
# <a name="create-grouppolicyconfigurationassignment"></a><span data-ttu-id="fbc88-103">GroupPolicyConfigurationAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="fbc88-103">Create groupPolicyConfigurationAssignment</span></span>

> <span data-ttu-id="fbc88-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fbc88-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fbc88-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="fbc88-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbc88-106">Erstellen eines neuen [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="fbc88-106">Create a new [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fbc88-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fbc88-107">Prerequisites</span></span>
<span data-ttu-id="fbc88-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbc88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbc88-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fbc88-110">Permission type</span></span>|<span data-ttu-id="fbc88-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fbc88-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbc88-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fbc88-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fbc88-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbc88-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fbc88-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fbc88-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbc88-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fbc88-115">Not supported.</span></span>|
|<span data-ttu-id="fbc88-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fbc88-116">Application</span></span>|<span data-ttu-id="fbc88-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fbc88-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbc88-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fbc88-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="fbc88-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fbc88-119">Request headers</span></span>
|<span data-ttu-id="fbc88-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="fbc88-120">Header</span></span>|<span data-ttu-id="fbc88-121">Wert</span><span class="sxs-lookup"><span data-stu-id="fbc88-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbc88-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fbc88-122">Authorization</span></span>|<span data-ttu-id="fbc88-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fbc88-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbc88-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fbc88-124">Accept</span></span>|<span data-ttu-id="fbc88-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fbc88-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbc88-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fbc88-126">Request body</span></span>
<span data-ttu-id="fbc88-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das groupPolicyConfigurationAssignment-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="fbc88-127">In the request body, supply a JSON representation for the groupPolicyConfigurationAssignment object.</span></span>

<span data-ttu-id="fbc88-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der groupPolicyConfigurationAssignment erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="fbc88-128">The following table shows the properties that are required when you create the groupPolicyConfigurationAssignment.</span></span>

|<span data-ttu-id="fbc88-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fbc88-129">Property</span></span>|<span data-ttu-id="fbc88-130">Typ</span><span class="sxs-lookup"><span data-stu-id="fbc88-130">Type</span></span>|<span data-ttu-id="fbc88-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fbc88-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbc88-132">id</span><span class="sxs-lookup"><span data-stu-id="fbc88-132">id</span></span>|<span data-ttu-id="fbc88-133">String</span><span class="sxs-lookup"><span data-stu-id="fbc88-133">String</span></span>|<span data-ttu-id="fbc88-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="fbc88-134">Key of the entity.</span></span>|
|<span data-ttu-id="fbc88-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fbc88-135">lastModifiedDateTime</span></span>|<span data-ttu-id="fbc88-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbc88-136">DateTimeOffset</span></span>|<span data-ttu-id="fbc88-137">Datum und Uhrzeit der letzten Änderung der Entität.</span><span class="sxs-lookup"><span data-stu-id="fbc88-137">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="fbc88-138">target</span><span class="sxs-lookup"><span data-stu-id="fbc88-138">target</span></span>|[<span data-ttu-id="fbc88-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="fbc88-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="fbc88-140">Der Typ der Gruppen, die für die Gruppenrichtlinienkonfiguration vorgesehen sind.</span><span class="sxs-lookup"><span data-stu-id="fbc88-140">The type of groups targeted the group policy configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="fbc88-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="fbc88-141">Response</span></span>
<span data-ttu-id="fbc88-142">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="fbc88-142">If successful, this method returns a `201 Created` response code and a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbc88-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fbc88-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="fbc88-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fbc88-144">Request</span></span>
<span data-ttu-id="fbc88-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fbc88-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fbc88-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="fbc88-146">Response</span></span>
<span data-ttu-id="fbc88-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fbc88-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




