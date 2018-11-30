---
title: Aktion „assign“
description: Noch nicht dokumentiert
ms.openlocfilehash: dd26c61f298071a98ad0734aa1ac5023581d5a9e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065776"
---
# <a name="assign-action"></a><span data-ttu-id="37354-103">Aktion „assign“</span><span class="sxs-lookup"><span data-stu-id="37354-103">assign action</span></span>

> <span data-ttu-id="37354-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="37354-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="37354-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="37354-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="37354-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="37354-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="37354-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="37354-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="37354-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="37354-108">Prerequisites</span></span>
<span data-ttu-id="37354-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37354-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37354-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="37354-111">Permission type</span></span>|<span data-ttu-id="37354-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="37354-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37354-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="37354-113">Delegated (work or school account)</span></span>|<span data-ttu-id="37354-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37354-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="37354-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="37354-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37354-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="37354-116">Not supported.</span></span>|
|<span data-ttu-id="37354-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="37354-117">Application</span></span>|<span data-ttu-id="37354-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="37354-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37354-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="37354-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="37354-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="37354-120">Request headers</span></span>
|<span data-ttu-id="37354-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="37354-121">Header</span></span>|<span data-ttu-id="37354-122">Wert</span><span class="sxs-lookup"><span data-stu-id="37354-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37354-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="37354-123">Authorization</span></span>|<span data-ttu-id="37354-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="37354-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37354-125">Accept</span><span class="sxs-lookup"><span data-stu-id="37354-125">Accept</span></span>|<span data-ttu-id="37354-126">application/json</span><span class="sxs-lookup"><span data-stu-id="37354-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37354-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="37354-127">Request body</span></span>
<span data-ttu-id="37354-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="37354-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="37354-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="37354-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="37354-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="37354-130">Property</span></span>|<span data-ttu-id="37354-131">Typ</span><span class="sxs-lookup"><span data-stu-id="37354-131">Type</span></span>|<span data-ttu-id="37354-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="37354-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37354-133">deviceConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="37354-133">deviceConfigurationGroupAssignments</span></span>|<span data-ttu-id="37354-134">[DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="37354-134">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="37354-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="37354-135">Not yet documented</span></span>|
|<span data-ttu-id="37354-136">assignments</span><span class="sxs-lookup"><span data-stu-id="37354-136">assignments</span></span>|<span data-ttu-id="37354-137">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="37354-137">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="37354-138">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="37354-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="37354-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="37354-139">Response</span></span>
<span data-ttu-id="37354-140">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="37354-140">If successful, this action returns a `200 OK` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37354-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="37354-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="37354-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="37354-142">Request</span></span>
<span data-ttu-id="37354-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="37354-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="37354-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="37354-144">Response</span></span>
<span data-ttu-id="37354-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="37354-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





