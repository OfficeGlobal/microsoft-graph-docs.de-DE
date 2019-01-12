---
title: Abrufen von networkIPv6ConfigurationManagementCondition
description: Lesen Sie Eigenschaften und Beziehungen des networkIPv6ConfigurationManagementCondition-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4ecd060949796180a7050164417d35fad99dc2a7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953350"
---
# <a name="get-networkipv6configurationmanagementcondition"></a><span data-ttu-id="ae75d-103">Abrufen von networkIPv6ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="ae75d-103">Get networkIPv6ConfigurationManagementCondition</span></span>

> <span data-ttu-id="ae75d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ae75d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ae75d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ae75d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ae75d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ae75d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ae75d-107">Lesen Sie Eigenschaften und Beziehungen des [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ae75d-107">Read properties and relationships of the [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ae75d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ae75d-108">Prerequisites</span></span>
<span data-ttu-id="ae75d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae75d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae75d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ae75d-111">Permission type</span></span>|<span data-ttu-id="ae75d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ae75d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae75d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ae75d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ae75d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae75d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ae75d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ae75d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae75d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae75d-116">Not supported.</span></span>|
|<span data-ttu-id="ae75d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ae75d-117">Application</span></span>|<span data-ttu-id="ae75d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae75d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae75d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae75d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/{managementConditionId}
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ae75d-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ae75d-120">Optional query parameters</span></span>
<span data-ttu-id="ae75d-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ae75d-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ae75d-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ae75d-122">Request headers</span></span>
|<span data-ttu-id="ae75d-123">Header</span><span class="sxs-lookup"><span data-stu-id="ae75d-123">Header</span></span>|<span data-ttu-id="ae75d-124">Wert</span><span class="sxs-lookup"><span data-stu-id="ae75d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae75d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae75d-125">Authorization</span></span>|<span data-ttu-id="ae75d-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ae75d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae75d-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ae75d-127">Accept</span></span>|<span data-ttu-id="ae75d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ae75d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae75d-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ae75d-129">Request body</span></span>
<span data-ttu-id="ae75d-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ae75d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae75d-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae75d-131">Response</span></span>
<span data-ttu-id="ae75d-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ae75d-132">If successful, this method returns a `200 OK` response code and [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae75d-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ae75d-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="ae75d-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae75d-134">Request</span></span>
<span data-ttu-id="ae75d-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ae75d-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
```

### <a name="response"></a><span data-ttu-id="ae75d-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae75d-136">Response</span></span>
<span data-ttu-id="ae75d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ae75d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 708

{
  "value": {
    "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
    "id": "25811206-1206-2581-0612-812506128125",
    "uniqueName": "Unique Name value",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
    "eTag": "ETag value",
    "applicablePlatforms": [
      "androidForWork"
    ],
    "ipV6Prefix": "Ip V6Prefix value",
    "ipV6Gateway": "Ip V6Gateway value",
    "ipV6DNSServerList": [
      "Ip V6DNSServer List value"
    ],
    "dnsSuffixList": [
      "Dns Suffix List value"
    ]
  }
}
```





