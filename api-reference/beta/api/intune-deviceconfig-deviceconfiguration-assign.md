---
title: Aktion zuweisen
description: Noch nicht dokumentiert.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 618176fd2aecfaa6feb058c22e9f2c9c335efe0b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30989302"
---
# <a name="assign-action"></a><span data-ttu-id="f441a-103">Aktion zuweisen</span><span class="sxs-lookup"><span data-stu-id="f441a-103">assign action</span></span>

> <span data-ttu-id="f441a-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f441a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f441a-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f441a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f441a-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="f441a-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f441a-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f441a-107">Prerequisites</span></span>
<span data-ttu-id="f441a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f441a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f441a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f441a-110">Permission type</span></span>|<span data-ttu-id="f441a-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f441a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f441a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f441a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f441a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f441a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f441a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f441a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f441a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f441a-115">Not supported.</span></span>|
|<span data-ttu-id="f441a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f441a-116">Application</span></span>|<span data-ttu-id="f441a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f441a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f441a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f441a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="f441a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f441a-119">Request headers</span></span>
|<span data-ttu-id="f441a-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f441a-120">Header</span></span>|<span data-ttu-id="f441a-121">Wert</span><span class="sxs-lookup"><span data-stu-id="f441a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f441a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f441a-122">Authorization</span></span>|<span data-ttu-id="f441a-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f441a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f441a-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f441a-124">Accept</span></span>|<span data-ttu-id="f441a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f441a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f441a-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f441a-126">Request body</span></span>
<span data-ttu-id="f441a-127">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="f441a-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f441a-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="f441a-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f441a-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f441a-129">Property</span></span>|<span data-ttu-id="f441a-130">Typ</span><span class="sxs-lookup"><span data-stu-id="f441a-130">Type</span></span>|<span data-ttu-id="f441a-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f441a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f441a-132">deviceConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="f441a-132">deviceConfigurationGroupAssignments</span></span>|<span data-ttu-id="f441a-133">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="f441a-133">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="f441a-134">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="f441a-134">Not yet documented</span></span>|
|<span data-ttu-id="f441a-135">assignments</span><span class="sxs-lookup"><span data-stu-id="f441a-135">assignments</span></span>|<span data-ttu-id="f441a-136">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="f441a-136">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="f441a-137">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="f441a-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f441a-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="f441a-138">Response</span></span>
<span data-ttu-id="f441a-139">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f441a-139">If successful, this action returns a `200 OK` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f441a-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f441a-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="f441a-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f441a-141">Request</span></span>
<span data-ttu-id="f441a-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f441a-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign

Content-type: application/json
Content-length: 548

{
  "deviceConfigurationGroupAssignments": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
      "id": "561d26c5-26c5-561d-c526-1d56c5261d56",
      "targetGroupId": "Target Group Id value",
      "excludeGroup": true
    }
  ],
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="f441a-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="f441a-143">Response</span></span>
<span data-ttu-id="f441a-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f441a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 271

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```




