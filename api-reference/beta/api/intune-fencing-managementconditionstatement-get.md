---
title: Abrufen von managementConditionStatement
description: Lesen Sie Eigenschaften und Beziehungen des ManagementConditionStatement-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2f8791cd65f2344350168f6192bdaad6230349b2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817003"
---
# <a name="get-managementconditionstatement"></a><span data-ttu-id="b5a00-103">Abrufen von managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="b5a00-103">Get managementConditionStatement</span></span>

> <span data-ttu-id="b5a00-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b5a00-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b5a00-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b5a00-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b5a00-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b5a00-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b5a00-107">Lesen Sie Eigenschaften und Beziehungen des [ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b5a00-107">Read properties and relationships of the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b5a00-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b5a00-108">Prerequisites</span></span>
<span data-ttu-id="b5a00-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5a00-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5a00-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b5a00-111">Permission type</span></span>|<span data-ttu-id="b5a00-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b5a00-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5a00-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b5a00-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b5a00-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5a00-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b5a00-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b5a00-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5a00-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b5a00-116">Not supported.</span></span>|
|<span data-ttu-id="b5a00-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b5a00-117">Application</span></span>|<span data-ttu-id="b5a00-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b5a00-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5a00-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b5a00-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditionStatements/{managementConditionStatementId}
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b5a00-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b5a00-120">Optional query parameters</span></span>
<span data-ttu-id="b5a00-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b5a00-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b5a00-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b5a00-122">Request headers</span></span>
|<span data-ttu-id="b5a00-123">Header</span><span class="sxs-lookup"><span data-stu-id="b5a00-123">Header</span></span>|<span data-ttu-id="b5a00-124">Wert</span><span class="sxs-lookup"><span data-stu-id="b5a00-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5a00-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5a00-125">Authorization</span></span>|<span data-ttu-id="b5a00-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5a00-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5a00-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b5a00-127">Accept</span></span>|<span data-ttu-id="b5a00-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b5a00-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5a00-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b5a00-129">Request body</span></span>
<span data-ttu-id="b5a00-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b5a00-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5a00-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="b5a00-131">Response</span></span>
<span data-ttu-id="b5a00-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b5a00-132">If successful, this method returns a `200 OK` response code and [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5a00-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b5a00-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="b5a00-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b5a00-134">Request</span></span>
<span data-ttu-id="b5a00-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b5a00-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/{managementConditionStatementId}
```

### <a name="response"></a><span data-ttu-id="b5a00-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="b5a00-136">Response</span></span>
<span data-ttu-id="b5a00-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b5a00-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 536

{
  "value": {
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
}
```





