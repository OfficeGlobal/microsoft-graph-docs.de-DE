---
title: Liste networkIPv6ConfigurationManagementConditions
description: Listeneigenschaften und Beziehungen der networkIPv6ConfigurationManagementCondition-Objekte.
ms.openlocfilehash: eb71bd64369a0cf02fff8e0390ba779a106d9684
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060459"
---
# <a name="list-networkipv6configurationmanagementconditions"></a><span data-ttu-id="4e4cb-103">Liste networkIPv6ConfigurationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="4e4cb-103">List networkIPv6ConfigurationManagementConditions</span></span>

> <span data-ttu-id="4e4cb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4e4cb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e4cb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4e4cb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4e4cb-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4e4cb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4e4cb-107">Listeneigenschaften und Beziehungen der [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="4e4cb-107">List properties and relationships of the [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4e4cb-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4e4cb-108">Prerequisites</span></span>
<span data-ttu-id="4e4cb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e4cb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e4cb-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4e4cb-111">Permission type</span></span>|<span data-ttu-id="4e4cb-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4e4cb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e4cb-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4e4cb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4e4cb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e4cb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4e4cb-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4e4cb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e4cb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4e4cb-116">Not supported.</span></span>|
|<span data-ttu-id="4e4cb-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4e4cb-117">Application</span></span>|<span data-ttu-id="4e4cb-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4e4cb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e4cb-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4e4cb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="4e4cb-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4e4cb-120">Request headers</span></span>
|<span data-ttu-id="4e4cb-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4e4cb-121">Header</span></span>|<span data-ttu-id="4e4cb-122">Wert</span><span class="sxs-lookup"><span data-stu-id="4e4cb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e4cb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e4cb-123">Authorization</span></span>|<span data-ttu-id="4e4cb-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4e4cb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e4cb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4e4cb-125">Accept</span></span>|<span data-ttu-id="4e4cb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4e4cb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e4cb-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4e4cb-127">Request body</span></span>
<span data-ttu-id="4e4cb-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4e4cb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e4cb-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="4e4cb-129">Response</span></span>
<span data-ttu-id="4e4cb-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="4e4cb-130">If successful, this method returns a `200 OK` response code and a collection of [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e4cb-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4e4cb-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="4e4cb-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4e4cb-132">Request</span></span>
<span data-ttu-id="4e4cb-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4e4cb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions
```

### <a name="response"></a><span data-ttu-id="4e4cb-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="4e4cb-134">Response</span></span>
<span data-ttu-id="4e4cb-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4e4cb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 760

{
  "value": [
    {
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
  ]
}
```





