---
title: GetManagementConditionStatementExpressionString-Funktion
description: Noch nicht dokumentiert
author: tfitzmac
ms.openlocfilehash: cde3e5b3c4867d2b3b0156fce550896b0748c8e1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354547"
---
# <a name="getmanagementconditionstatementexpressionstring-function"></a><span data-ttu-id="c254a-103">GetManagementConditionStatementExpressionString-Funktion</span><span class="sxs-lookup"><span data-stu-id="c254a-103">getManagementConditionStatementExpressionString function</span></span>

> <span data-ttu-id="c254a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c254a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c254a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c254a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c254a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c254a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c254a-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="c254a-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c254a-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c254a-108">Prerequisites</span></span>
<span data-ttu-id="c254a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c254a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c254a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c254a-111">Permission type</span></span>|<span data-ttu-id="c254a-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c254a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c254a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c254a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c254a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c254a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c254a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c254a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c254a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c254a-116">Not supported.</span></span>|
|<span data-ttu-id="c254a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c254a-117">Application</span></span>|<span data-ttu-id="c254a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c254a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c254a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c254a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditionStatements/{managementConditionStatementId}/getManagementConditionStatementExpressionString
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/getManagementConditionStatementExpressionString
```

## <a name="request-headers"></a><span data-ttu-id="c254a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c254a-120">Request headers</span></span>
|<span data-ttu-id="c254a-121">Header</span><span class="sxs-lookup"><span data-stu-id="c254a-121">Header</span></span>|<span data-ttu-id="c254a-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c254a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c254a-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c254a-123">Authorization</span></span>|<span data-ttu-id="c254a-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c254a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c254a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c254a-125">Accept</span></span>|<span data-ttu-id="c254a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c254a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c254a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c254a-127">Request body</span></span>
<span data-ttu-id="c254a-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c254a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c254a-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="c254a-129">Response</span></span>
<span data-ttu-id="c254a-130">Wenn erfolgreich, diese Funktion gibt eine `200 OK` Antwortcode und eine [ManagementConditionExpressionString](../resources/intune-fencing-managementconditionexpressionstring.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="c254a-130">If successful, this function returns a `200 OK` response code and a [managementConditionExpressionString](../resources/intune-fencing-managementconditionexpressionstring.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c254a-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c254a-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="c254a-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c254a-132">Request</span></span>
<span data-ttu-id="c254a-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c254a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/{managementConditionStatementId}/getManagementConditionStatementExpressionString
```

### <a name="response"></a><span data-ttu-id="c254a-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="c254a-134">Response</span></span>
<span data-ttu-id="c254a-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c254a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 126

{
  "value": {
    "@odata.type": "microsoft.graph.managementConditionExpressionString",
    "value": "Value value"
  }
}
```





