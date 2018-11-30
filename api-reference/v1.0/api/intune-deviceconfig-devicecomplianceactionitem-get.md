---
title: deviceComplianceActionItem abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceComplianceActionItem-Objekts.
ms.openlocfilehash: 1697c7316495751a6bea18028f6e3df6ddaa469e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017570"
---
# <a name="get-devicecomplianceactionitem"></a><span data-ttu-id="01c42-103">deviceComplianceActionItem abrufen</span><span class="sxs-lookup"><span data-stu-id="01c42-103">Get deviceComplianceActionItem</span></span>

> <span data-ttu-id="01c42-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="01c42-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="01c42-105">Lesen von Eigenschaften und Beziehungen des [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="01c42-105">Read properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="01c42-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="01c42-106">Prerequisites</span></span>
<span data-ttu-id="01c42-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01c42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01c42-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="01c42-109">Permission type</span></span>|<span data-ttu-id="01c42-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="01c42-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01c42-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="01c42-111">Delegated (work or school account)</span></span>|<span data-ttu-id="01c42-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="01c42-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="01c42-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="01c42-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01c42-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="01c42-114">Not supported.</span></span>|
|<span data-ttu-id="01c42-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="01c42-115">Application</span></span>|<span data-ttu-id="01c42-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="01c42-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="01c42-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="01c42-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="01c42-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="01c42-118">Optional query parameters</span></span>
<span data-ttu-id="01c42-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="01c42-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="01c42-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="01c42-120">Request headers</span></span>
|<span data-ttu-id="01c42-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="01c42-121">Header</span></span>|<span data-ttu-id="01c42-122">Wert</span><span class="sxs-lookup"><span data-stu-id="01c42-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01c42-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="01c42-123">Authorization</span></span>|<span data-ttu-id="01c42-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="01c42-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01c42-125">Accept</span><span class="sxs-lookup"><span data-stu-id="01c42-125">Accept</span></span>|<span data-ttu-id="01c42-126">application/json</span><span class="sxs-lookup"><span data-stu-id="01c42-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01c42-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="01c42-127">Request body</span></span>
<span data-ttu-id="01c42-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="01c42-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01c42-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="01c42-129">Response</span></span>
<span data-ttu-id="01c42-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="01c42-130">If successful, this method returns a `200 OK` response code and [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01c42-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="01c42-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="01c42-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="01c42-132">Request</span></span>
<span data-ttu-id="01c42-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="01c42-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

### <a name="response"></a><span data-ttu-id="01c42-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="01c42-134">Response</span></span>
<span data-ttu-id="01c42-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="01c42-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 355

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
    "id": "e01a1893-1893-e01a-9318-1ae093181ae0",
    "gracePeriodHours": 0,
    "actionType": "notification",
    "notificationTemplateId": "Notification Template Id value",
    "notificationMessageCCList": [
      "Notification Message CCList value"
    ]
  }
}
```



