---
title: Abrufen von locationManagementCondition
description: Lesen Sie Eigenschaften und Beziehungen des LocationManagementCondition-Objekts.
ms.openlocfilehash: df713d68b45c0ad62bce5ade42a53bdc5d69bd83
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061762"
---
# <a name="get-locationmanagementcondition"></a><span data-ttu-id="d7fd5-103">Abrufen von locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="d7fd5-103">Get locationManagementCondition</span></span>

> <span data-ttu-id="d7fd5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d7fd5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d7fd5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d7fd5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d7fd5-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d7fd5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d7fd5-107">Lesen Sie Eigenschaften und Beziehungen des [LocationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d7fd5-107">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d7fd5-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d7fd5-108">Prerequisites</span></span>
<span data-ttu-id="d7fd5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7fd5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7fd5-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d7fd5-111">Permission type</span></span>|<span data-ttu-id="d7fd5-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d7fd5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7fd5-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d7fd5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d7fd5-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7fd5-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d7fd5-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d7fd5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7fd5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d7fd5-116">Not supported.</span></span>|
|<span data-ttu-id="d7fd5-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d7fd5-117">Application</span></span>|<span data-ttu-id="d7fd5-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d7fd5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7fd5-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d7fd5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/{managementConditionId}
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d7fd5-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d7fd5-120">Optional query parameters</span></span>
<span data-ttu-id="d7fd5-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d7fd5-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d7fd5-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d7fd5-122">Request headers</span></span>
|<span data-ttu-id="d7fd5-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d7fd5-123">Header</span></span>|<span data-ttu-id="d7fd5-124">Wert</span><span class="sxs-lookup"><span data-stu-id="d7fd5-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7fd5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7fd5-125">Authorization</span></span>|<span data-ttu-id="d7fd5-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d7fd5-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7fd5-127">Accept</span><span class="sxs-lookup"><span data-stu-id="d7fd5-127">Accept</span></span>|<span data-ttu-id="d7fd5-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d7fd5-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7fd5-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d7fd5-129">Request body</span></span>
<span data-ttu-id="d7fd5-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d7fd5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7fd5-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="d7fd5-131">Response</span></span>
<span data-ttu-id="d7fd5-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [LocationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d7fd5-132">If successful, this method returns a `200 OK` response code and [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7fd5-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d7fd5-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="d7fd5-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d7fd5-134">Request</span></span>
<span data-ttu-id="d7fd5-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d7fd5-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
```

### <a name="response"></a><span data-ttu-id="d7fd5-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="d7fd5-136">Response</span></span>
<span data-ttu-id="d7fd5-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d7fd5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 476

{
  "value": {
    "@odata.type": "#microsoft.graph.locationManagementCondition",
    "id": "23b1ca32-ca32-23b1-32ca-b12332cab123",
    "uniqueName": "Unique Name value",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
    "eTag": "ETag value",
    "applicablePlatforms": [
      "androidForWork"
    ]
  }
}
```





