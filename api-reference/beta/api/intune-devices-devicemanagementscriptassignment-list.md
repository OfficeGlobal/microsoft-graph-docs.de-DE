---
title: Liste deviceManagementScriptAssignments
description: Listeneigenschaften und Beziehungen der DeviceManagementScriptAssignment-Objekte.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 47bf7ca7938fb8bab7ea41a925804f1e7b084ff5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873920"
---
# <a name="list-devicemanagementscriptassignments"></a><span data-ttu-id="08c91-103">Liste deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="08c91-103">List deviceManagementScriptAssignments</span></span>

> <span data-ttu-id="08c91-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="08c91-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="08c91-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="08c91-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="08c91-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="08c91-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="08c91-107">Listeneigenschaften und Beziehungen der [DeviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="08c91-107">List properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="08c91-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="08c91-108">Prerequisites</span></span>
<span data-ttu-id="08c91-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08c91-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08c91-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="08c91-111">Permission type</span></span>|<span data-ttu-id="08c91-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="08c91-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08c91-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="08c91-113">Delegated (work or school account)</span></span>|<span data-ttu-id="08c91-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="08c91-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="08c91-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="08c91-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08c91-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="08c91-116">Not supported.</span></span>|
|<span data-ttu-id="08c91-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="08c91-117">Application</span></span>|<span data-ttu-id="08c91-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="08c91-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="08c91-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="08c91-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="08c91-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="08c91-120">Request headers</span></span>
|<span data-ttu-id="08c91-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="08c91-121">Header</span></span>|<span data-ttu-id="08c91-122">Wert</span><span class="sxs-lookup"><span data-stu-id="08c91-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08c91-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="08c91-123">Authorization</span></span>|<span data-ttu-id="08c91-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="08c91-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08c91-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="08c91-125">Accept</span></span>|<span data-ttu-id="08c91-126">application/json</span><span class="sxs-lookup"><span data-stu-id="08c91-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08c91-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="08c91-127">Request body</span></span>
<span data-ttu-id="08c91-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="08c91-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08c91-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="08c91-129">Response</span></span>
<span data-ttu-id="08c91-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [DeviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="08c91-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08c91-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="08c91-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="08c91-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="08c91-132">Request</span></span>
<span data-ttu-id="08c91-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="08c91-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments
```

### <a name="response"></a><span data-ttu-id="08c91-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="08c91-134">Response</span></span>
<span data-ttu-id="08c91-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="08c91-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 274

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
      "id": "a87a601e-601e-a87a-1e60-7aa81e607aa8",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





