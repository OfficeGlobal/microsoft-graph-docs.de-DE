---
title: Auflisten von „deviceComplianceActionItem“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceComplianceActionItem auf.
ms.openlocfilehash: 11e87ce644043d4f990c805bc65c7ea833f345b2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018341"
---
# <a name="list-devicecomplianceactionitems"></a><span data-ttu-id="18554-103">Auflisten von „deviceComplianceActionItem“</span><span class="sxs-lookup"><span data-stu-id="18554-103">List deviceComplianceActionItems</span></span>

> <span data-ttu-id="18554-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="18554-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="18554-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) auf.</span><span class="sxs-lookup"><span data-stu-id="18554-105">List properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="18554-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="18554-106">Prerequisites</span></span>
<span data-ttu-id="18554-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18554-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18554-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="18554-109">Permission type</span></span>|<span data-ttu-id="18554-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="18554-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18554-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="18554-111">Delegated (work or school account)</span></span>|<span data-ttu-id="18554-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="18554-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="18554-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="18554-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18554-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="18554-114">Not supported.</span></span>|
|<span data-ttu-id="18554-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="18554-115">Application</span></span>|<span data-ttu-id="18554-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="18554-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18554-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="18554-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="18554-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="18554-118">Request headers</span></span>
|<span data-ttu-id="18554-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="18554-119">Header</span></span>|<span data-ttu-id="18554-120">Wert</span><span class="sxs-lookup"><span data-stu-id="18554-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18554-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="18554-121">Authorization</span></span>|<span data-ttu-id="18554-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="18554-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18554-123">Accept</span><span class="sxs-lookup"><span data-stu-id="18554-123">Accept</span></span>|<span data-ttu-id="18554-124">application/json</span><span class="sxs-lookup"><span data-stu-id="18554-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18554-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="18554-125">Request body</span></span>
<span data-ttu-id="18554-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="18554-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18554-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="18554-127">Response</span></span>
<span data-ttu-id="18554-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="18554-128">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18554-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="18554-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="18554-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="18554-130">Request</span></span>
<span data-ttu-id="18554-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="18554-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

### <a name="response"></a><span data-ttu-id="18554-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="18554-132">Response</span></span>
<span data-ttu-id="18554-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="18554-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 385

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
      "id": "e01a1893-1893-e01a-9318-1ae093181ae0",
      "gracePeriodHours": 0,
      "actionType": "notification",
      "notificationTemplateId": "Notification Template Id value",
      "notificationMessageCCList": [
        "Notification Message CCList value"
      ]
    }
  ]
}
```



