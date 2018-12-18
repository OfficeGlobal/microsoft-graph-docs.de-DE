---
title: Liste networkIPv4ConfigurationManagementConditions
description: Listeneigenschaften und Beziehungen der networkIPv4ConfigurationManagementCondition-Objekte.
author: tfitzmac
ms.openlocfilehash: 6e1707fa85788fb5085f37654645b0863b5a8b46
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27363613"
---
# <a name="list-networkipv4configurationmanagementconditions"></a><span data-ttu-id="85f57-103">Liste networkIPv4ConfigurationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="85f57-103">List networkIPv4ConfigurationManagementConditions</span></span>

> <span data-ttu-id="85f57-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="85f57-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85f57-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="85f57-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="85f57-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="85f57-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="85f57-107">Listeneigenschaften und Beziehungen der [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="85f57-107">List properties and relationships of the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="85f57-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="85f57-108">Prerequisites</span></span>
<span data-ttu-id="85f57-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85f57-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85f57-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="85f57-111">Permission type</span></span>|<span data-ttu-id="85f57-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="85f57-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85f57-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="85f57-113">Delegated (work or school account)</span></span>|<span data-ttu-id="85f57-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="85f57-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="85f57-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="85f57-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85f57-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="85f57-116">Not supported.</span></span>|
|<span data-ttu-id="85f57-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="85f57-117">Application</span></span>|<span data-ttu-id="85f57-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="85f57-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85f57-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="85f57-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="85f57-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="85f57-120">Request headers</span></span>
|<span data-ttu-id="85f57-121">Header</span><span class="sxs-lookup"><span data-stu-id="85f57-121">Header</span></span>|<span data-ttu-id="85f57-122">Wert</span><span class="sxs-lookup"><span data-stu-id="85f57-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85f57-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="85f57-123">Authorization</span></span>|<span data-ttu-id="85f57-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="85f57-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85f57-125">Accept</span><span class="sxs-lookup"><span data-stu-id="85f57-125">Accept</span></span>|<span data-ttu-id="85f57-126">application/json</span><span class="sxs-lookup"><span data-stu-id="85f57-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85f57-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="85f57-127">Request body</span></span>
<span data-ttu-id="85f57-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="85f57-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85f57-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="85f57-129">Response</span></span>
<span data-ttu-id="85f57-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="85f57-130">If successful, this method returns a `200 OK` response code and a collection of [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85f57-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="85f57-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="85f57-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="85f57-132">Request</span></span>
<span data-ttu-id="85f57-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="85f57-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions
```

### <a name="response"></a><span data-ttu-id="85f57-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="85f57-134">Response</span></span>
<span data-ttu-id="85f57-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="85f57-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 810

{
  "value": [
    {
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
  ]
}
```





