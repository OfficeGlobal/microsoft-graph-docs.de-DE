---
title: Aktion „assign“
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b5d30818be0733d7b571f0c2e32fb01af5570d65
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400333"
---
# <a name="assign-action"></a><span data-ttu-id="9b6a0-103">Aktion „assign“</span><span class="sxs-lookup"><span data-stu-id="9b6a0-103">assign action</span></span>

> <span data-ttu-id="9b6a0-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="9b6a0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9b6a0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9b6a0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9b6a0-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9b6a0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b6a0-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="9b6a0-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b6a0-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9b6a0-108">Prerequisites</span></span>
<span data-ttu-id="9b6a0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9b6a0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9b6a0-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9b6a0-111">Permission type</span></span>|<span data-ttu-id="9b6a0-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9b6a0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b6a0-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9b6a0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9b6a0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b6a0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9b6a0-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9b6a0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b6a0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9b6a0-116">Not supported.</span></span>|
|<span data-ttu-id="9b6a0-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9b6a0-117">Application</span></span>|<span data-ttu-id="9b6a0-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9b6a0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b6a0-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9b6a0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="9b6a0-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9b6a0-120">Request headers</span></span>
|<span data-ttu-id="9b6a0-121">Header</span><span class="sxs-lookup"><span data-stu-id="9b6a0-121">Header</span></span>|<span data-ttu-id="9b6a0-122">Wert</span><span class="sxs-lookup"><span data-stu-id="9b6a0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b6a0-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="9b6a0-123">Authorization</span></span>|<span data-ttu-id="9b6a0-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9b6a0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b6a0-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9b6a0-125">Accept</span></span>|<span data-ttu-id="9b6a0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9b6a0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b6a0-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9b6a0-127">Request body</span></span>
<span data-ttu-id="9b6a0-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="9b6a0-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9b6a0-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="9b6a0-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9b6a0-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9b6a0-130">Property</span></span>|<span data-ttu-id="9b6a0-131">Typ</span><span class="sxs-lookup"><span data-stu-id="9b6a0-131">Type</span></span>|<span data-ttu-id="9b6a0-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9b6a0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b6a0-133">deviceConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="9b6a0-133">deviceConfigurationGroupAssignments</span></span>|<span data-ttu-id="9b6a0-134">[DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="9b6a0-134">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="9b6a0-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="9b6a0-135">Not yet documented</span></span>|
|<span data-ttu-id="9b6a0-136">assignments</span><span class="sxs-lookup"><span data-stu-id="9b6a0-136">assignments</span></span>|<span data-ttu-id="9b6a0-137">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="9b6a0-137">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="9b6a0-138">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="9b6a0-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9b6a0-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="9b6a0-139">Response</span></span>
<span data-ttu-id="9b6a0-140">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9b6a0-140">If successful, this action returns a `200 OK` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b6a0-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9b6a0-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b6a0-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9b6a0-142">Request</span></span>
<span data-ttu-id="9b6a0-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9b6a0-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9b6a0-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="9b6a0-144">Response</span></span>
<span data-ttu-id="9b6a0-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9b6a0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




