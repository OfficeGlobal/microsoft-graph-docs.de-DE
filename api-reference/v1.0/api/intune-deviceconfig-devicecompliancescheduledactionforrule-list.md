---
title: Auflisten von „deviceComplianceScheduledActionForRule“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceComplianceScheduledActionForRule auf.
author: tfitzmac
ms.openlocfilehash: 551b1c336418c0abef8175b6f474904779eb4b2f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321539"
---
# <a name="list-devicecompliancescheduledactionforrules"></a><span data-ttu-id="f1e77-103">Auflisten von „deviceComplianceScheduledActionForRule“</span><span class="sxs-lookup"><span data-stu-id="f1e77-103">List deviceComplianceScheduledActionForRules</span></span>

> <span data-ttu-id="f1e77-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f1e77-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1e77-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) auf.</span><span class="sxs-lookup"><span data-stu-id="f1e77-105">List properties and relationships of the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f1e77-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f1e77-106">Prerequisites</span></span>
<span data-ttu-id="f1e77-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1e77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1e77-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f1e77-109">Permission type</span></span>|<span data-ttu-id="f1e77-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f1e77-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1e77-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f1e77-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f1e77-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1e77-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f1e77-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f1e77-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1e77-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f1e77-114">Not supported.</span></span>|
|<span data-ttu-id="f1e77-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f1e77-115">Application</span></span>|<span data-ttu-id="f1e77-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f1e77-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1e77-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f1e77-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="f1e77-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f1e77-118">Request headers</span></span>
|<span data-ttu-id="f1e77-119">Header</span><span class="sxs-lookup"><span data-stu-id="f1e77-119">Header</span></span>|<span data-ttu-id="f1e77-120">Wert</span><span class="sxs-lookup"><span data-stu-id="f1e77-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1e77-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f1e77-121">Authorization</span></span>|<span data-ttu-id="f1e77-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f1e77-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1e77-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f1e77-123">Accept</span></span>|<span data-ttu-id="f1e77-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f1e77-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1e77-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f1e77-125">Request body</span></span>
<span data-ttu-id="f1e77-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f1e77-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1e77-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="f1e77-127">Response</span></span>
<span data-ttu-id="f1e77-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f1e77-128">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1e77-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f1e77-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="f1e77-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f1e77-130">Request</span></span>
<span data-ttu-id="f1e77-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f1e77-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

### <a name="response"></a><span data-ttu-id="f1e77-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="f1e77-132">Response</span></span>
<span data-ttu-id="f1e77-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f1e77-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 208

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
      "id": "f0075d5e-5d5e-f007-5e5d-07f05e5d07f0",
      "ruleName": "Rule Name value"
    }
  ]
}
```



