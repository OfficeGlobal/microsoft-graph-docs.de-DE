---
title: Auflisten von „deviceComplianceActionItem“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceComplianceActionItem auf.
author: tfitzmac
ms.openlocfilehash: 78aedc180f793938db86c7faa3595052371233a1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342315"
---
# <a name="list-devicecomplianceactionitems"></a><span data-ttu-id="b3256-103">Auflisten von „deviceComplianceActionItem“</span><span class="sxs-lookup"><span data-stu-id="b3256-103">List deviceComplianceActionItems</span></span>

> <span data-ttu-id="b3256-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b3256-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b3256-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b3256-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b3256-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b3256-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3256-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) auf.</span><span class="sxs-lookup"><span data-stu-id="b3256-107">List properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b3256-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b3256-108">Prerequisites</span></span>
<span data-ttu-id="b3256-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3256-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3256-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b3256-111">Permission type</span></span>|<span data-ttu-id="b3256-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b3256-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3256-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b3256-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b3256-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3256-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b3256-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b3256-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3256-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b3256-116">Not supported.</span></span>|
|<span data-ttu-id="b3256-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b3256-117">Application</span></span>|<span data-ttu-id="b3256-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b3256-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3256-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b3256-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b3256-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b3256-120">Request headers</span></span>
|<span data-ttu-id="b3256-121">Header</span><span class="sxs-lookup"><span data-stu-id="b3256-121">Header</span></span>|<span data-ttu-id="b3256-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b3256-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3256-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b3256-123">Authorization</span></span>|<span data-ttu-id="b3256-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b3256-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3256-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b3256-125">Accept</span></span>|<span data-ttu-id="b3256-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b3256-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3256-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b3256-127">Request body</span></span>
<span data-ttu-id="b3256-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b3256-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3256-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="b3256-129">Response</span></span>
<span data-ttu-id="b3256-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b3256-130">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3256-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b3256-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b3256-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b3256-132">Request</span></span>
<span data-ttu-id="b3256-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b3256-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

### <a name="response"></a><span data-ttu-id="b3256-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="b3256-134">Response</span></span>
<span data-ttu-id="b3256-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b3256-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





