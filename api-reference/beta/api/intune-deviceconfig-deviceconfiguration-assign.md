---
title: Aktion „assign“
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 455c51dee7f4e1a480fb28e965e0036f64149989
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938902"
---
# <a name="assign-action"></a><span data-ttu-id="06ff3-103">Aktion „assign“</span><span class="sxs-lookup"><span data-stu-id="06ff3-103">assign action</span></span>

> <span data-ttu-id="06ff3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="06ff3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06ff3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="06ff3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06ff3-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="06ff3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06ff3-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="06ff3-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="06ff3-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="06ff3-108">Prerequisites</span></span>
<span data-ttu-id="06ff3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06ff3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06ff3-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="06ff3-111">Permission type</span></span>|<span data-ttu-id="06ff3-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="06ff3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06ff3-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="06ff3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="06ff3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06ff3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="06ff3-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="06ff3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06ff3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="06ff3-116">Not supported.</span></span>|
|<span data-ttu-id="06ff3-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="06ff3-117">Application</span></span>|<span data-ttu-id="06ff3-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="06ff3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06ff3-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="06ff3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="06ff3-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="06ff3-120">Request headers</span></span>
|<span data-ttu-id="06ff3-121">Header</span><span class="sxs-lookup"><span data-stu-id="06ff3-121">Header</span></span>|<span data-ttu-id="06ff3-122">Wert</span><span class="sxs-lookup"><span data-stu-id="06ff3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06ff3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="06ff3-123">Authorization</span></span>|<span data-ttu-id="06ff3-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="06ff3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06ff3-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="06ff3-125">Accept</span></span>|<span data-ttu-id="06ff3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="06ff3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06ff3-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="06ff3-127">Request body</span></span>
<span data-ttu-id="06ff3-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="06ff3-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="06ff3-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="06ff3-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="06ff3-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="06ff3-130">Property</span></span>|<span data-ttu-id="06ff3-131">Typ</span><span class="sxs-lookup"><span data-stu-id="06ff3-131">Type</span></span>|<span data-ttu-id="06ff3-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="06ff3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06ff3-133">deviceConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="06ff3-133">deviceConfigurationGroupAssignments</span></span>|<span data-ttu-id="06ff3-134">[DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="06ff3-134">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="06ff3-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="06ff3-135">Not yet documented</span></span>|
|<span data-ttu-id="06ff3-136">assignments</span><span class="sxs-lookup"><span data-stu-id="06ff3-136">assignments</span></span>|<span data-ttu-id="06ff3-137">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="06ff3-137">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="06ff3-138">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="06ff3-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="06ff3-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="06ff3-139">Response</span></span>
<span data-ttu-id="06ff3-140">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="06ff3-140">If successful, this action returns a `200 OK` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06ff3-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="06ff3-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="06ff3-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="06ff3-142">Request</span></span>
<span data-ttu-id="06ff3-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="06ff3-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="06ff3-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="06ff3-144">Response</span></span>
<span data-ttu-id="06ff3-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="06ff3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





