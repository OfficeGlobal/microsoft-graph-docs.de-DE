---
title: deviceComplianceActionItem abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceComplianceActionItem-Objekts.
author: tfitzmac
ms.openlocfilehash: 2fd6762ca3f0d7128721eb240d7d00bcf1291da4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307952"
---
# <a name="get-devicecomplianceactionitem"></a><span data-ttu-id="eecfa-103">deviceComplianceActionItem abrufen</span><span class="sxs-lookup"><span data-stu-id="eecfa-103">Get deviceComplianceActionItem</span></span>

> <span data-ttu-id="eecfa-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="eecfa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eecfa-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="eecfa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eecfa-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="eecfa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eecfa-107">Lesen von Eigenschaften und Beziehungen des [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="eecfa-107">Read properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eecfa-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="eecfa-108">Prerequisites</span></span>
<span data-ttu-id="eecfa-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eecfa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eecfa-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eecfa-111">Permission type</span></span>|<span data-ttu-id="eecfa-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="eecfa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eecfa-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eecfa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eecfa-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="eecfa-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="eecfa-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eecfa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eecfa-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eecfa-116">Not supported.</span></span>|
|<span data-ttu-id="eecfa-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eecfa-117">Application</span></span>|<span data-ttu-id="eecfa-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eecfa-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eecfa-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eecfa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eecfa-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="eecfa-120">Optional query parameters</span></span>
<span data-ttu-id="eecfa-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="eecfa-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="eecfa-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eecfa-122">Request headers</span></span>
|<span data-ttu-id="eecfa-123">Header</span><span class="sxs-lookup"><span data-stu-id="eecfa-123">Header</span></span>|<span data-ttu-id="eecfa-124">Wert</span><span class="sxs-lookup"><span data-stu-id="eecfa-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eecfa-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="eecfa-125">Authorization</span></span>|<span data-ttu-id="eecfa-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="eecfa-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eecfa-127">Accept</span><span class="sxs-lookup"><span data-stu-id="eecfa-127">Accept</span></span>|<span data-ttu-id="eecfa-128">application/json</span><span class="sxs-lookup"><span data-stu-id="eecfa-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eecfa-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="eecfa-129">Request body</span></span>
<span data-ttu-id="eecfa-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="eecfa-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eecfa-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="eecfa-131">Response</span></span>
<span data-ttu-id="eecfa-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eecfa-132">If successful, this method returns a `200 OK` response code and [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eecfa-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eecfa-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="eecfa-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eecfa-134">Request</span></span>
<span data-ttu-id="eecfa-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="eecfa-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

### <a name="response"></a><span data-ttu-id="eecfa-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="eecfa-136">Response</span></span>
<span data-ttu-id="eecfa-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eecfa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





