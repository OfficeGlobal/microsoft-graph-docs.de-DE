---
title: Liste managementConditionStatements
description: Listeneigenschaften und Beziehungen der ManagementConditionStatement-Objekte.
ms.openlocfilehash: 7bc14cba615e6cbb4823f2b194f1756a7d728473
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064643"
---
# <a name="list-managementconditionstatements"></a><span data-ttu-id="ad0c8-103">Liste managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="ad0c8-103">List managementConditionStatements</span></span>

> <span data-ttu-id="ad0c8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ad0c8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad0c8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ad0c8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ad0c8-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ad0c8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ad0c8-107">Listeneigenschaften und Beziehungen der [ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="ad0c8-107">List properties and relationships of the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ad0c8-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ad0c8-108">Prerequisites</span></span>
<span data-ttu-id="ad0c8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad0c8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad0c8-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ad0c8-111">Permission type</span></span>|<span data-ttu-id="ad0c8-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ad0c8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad0c8-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ad0c8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ad0c8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad0c8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ad0c8-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ad0c8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad0c8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ad0c8-116">Not supported.</span></span>|
|<span data-ttu-id="ad0c8-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ad0c8-117">Application</span></span>|<span data-ttu-id="ad0c8-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ad0c8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad0c8-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ad0c8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditionStatements
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements
```

## <a name="request-headers"></a><span data-ttu-id="ad0c8-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ad0c8-120">Request headers</span></span>
|<span data-ttu-id="ad0c8-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ad0c8-121">Header</span></span>|<span data-ttu-id="ad0c8-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ad0c8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad0c8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad0c8-123">Authorization</span></span>|<span data-ttu-id="ad0c8-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ad0c8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad0c8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ad0c8-125">Accept</span></span>|<span data-ttu-id="ad0c8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ad0c8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad0c8-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ad0c8-127">Request body</span></span>
<span data-ttu-id="ad0c8-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ad0c8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad0c8-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="ad0c8-129">Response</span></span>
<span data-ttu-id="ad0c8-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="ad0c8-130">If successful, this method returns a `200 OK` response code and a collection of [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad0c8-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ad0c8-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ad0c8-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ad0c8-132">Request</span></span>
<span data-ttu-id="ad0c8-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ad0c8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements
```

### <a name="response"></a><span data-ttu-id="ad0c8-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="ad0c8-134">Response</span></span>
<span data-ttu-id="ad0c8-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ad0c8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 576

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managementConditionStatement",
      "id": "bedb0c00-0c00-bedb-000c-dbbe000cdbbe",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "expression": {
        "@odata.type": "microsoft.graph.managementConditionExpression"
      },
      "eTag": "ETag value",
      "applicablePlatforms": [
        "androidForWork"
      ]
    }
  ]
}
```





