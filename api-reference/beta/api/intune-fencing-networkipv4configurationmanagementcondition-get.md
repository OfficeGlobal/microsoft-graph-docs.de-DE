---
title: Abrufen von networkIPv4ConfigurationManagementCondition
description: Lesen Sie Eigenschaften und Beziehungen des networkIPv4ConfigurationManagementCondition-Objekts.
author: tfitzmac
ms.openlocfilehash: a13e202d1347705edd4d26e01a65668dba971f73
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319495"
---
# <a name="get-networkipv4configurationmanagementcondition"></a><span data-ttu-id="a613a-103">Abrufen von networkIPv4ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="a613a-103">Get networkIPv4ConfigurationManagementCondition</span></span>

> <span data-ttu-id="a613a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a613a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a613a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a613a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a613a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a613a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a613a-107">Lesen Sie Eigenschaften und Beziehungen des [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="a613a-107">Read properties and relationships of the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a613a-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a613a-108">Prerequisites</span></span>
<span data-ttu-id="a613a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a613a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a613a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a613a-111">Permission type</span></span>|<span data-ttu-id="a613a-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a613a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a613a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a613a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a613a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a613a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a613a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a613a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a613a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a613a-116">Not supported.</span></span>|
|<span data-ttu-id="a613a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a613a-117">Application</span></span>|<span data-ttu-id="a613a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a613a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a613a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a613a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/{managementConditionId}
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a613a-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a613a-120">Optional query parameters</span></span>
<span data-ttu-id="a613a-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a613a-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a613a-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a613a-122">Request headers</span></span>
|<span data-ttu-id="a613a-123">Header</span><span class="sxs-lookup"><span data-stu-id="a613a-123">Header</span></span>|<span data-ttu-id="a613a-124">Wert</span><span class="sxs-lookup"><span data-stu-id="a613a-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a613a-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="a613a-125">Authorization</span></span>|<span data-ttu-id="a613a-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a613a-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a613a-127">Accept</span><span class="sxs-lookup"><span data-stu-id="a613a-127">Accept</span></span>|<span data-ttu-id="a613a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a613a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a613a-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a613a-129">Request body</span></span>
<span data-ttu-id="a613a-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a613a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a613a-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="a613a-131">Response</span></span>
<span data-ttu-id="a613a-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="a613a-132">If successful, this method returns a `200 OK` response code and [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a613a-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a613a-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="a613a-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a613a-134">Request</span></span>
<span data-ttu-id="a613a-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a613a-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
```

### <a name="response"></a><span data-ttu-id="a613a-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="a613a-136">Response</span></span>
<span data-ttu-id="a613a-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a613a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 756

{
  "value": {
    "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
    "id": "5e4a8284-8284-5e4a-8482-4a5e84824a5e",
    "uniqueName": "Unique Name value",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
    "eTag": "ETag value",
    "applicablePlatforms": [
      "androidForWork"
    ],
    "ipV4Prefix": "Ip V4Prefix value",
    "ipV4Gateway": "Ip V4Gateway value",
    "ipV4DHCPServer": "Ip V4DHCPServer value",
    "ipV4DNSServerList": [
      "Ip V4DNSServer List value"
    ],
    "dnsSuffixList": [
      "Dns Suffix List value"
    ]
  }
}
```





