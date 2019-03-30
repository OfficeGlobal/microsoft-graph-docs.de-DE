---
title: NetworkIPv4ConfigurationManagementCondition abrufen
description: Lesen von Eigenschaften und Beziehungen des networkIPv4ConfigurationManagementCondition-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 969b3a750f175077ab6ab82c6917039a798009a5
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30989113"
---
# <a name="get-networkipv4configurationmanagementcondition"></a><span data-ttu-id="24621-103">NetworkIPv4ConfigurationManagementCondition abrufen</span><span class="sxs-lookup"><span data-stu-id="24621-103">Get networkIPv4ConfigurationManagementCondition</span></span>

> <span data-ttu-id="24621-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="24621-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24621-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="24621-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24621-106">Lesen von Eigenschaften und Beziehungen des [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="24621-106">Read properties and relationships of the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24621-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="24621-107">Prerequisites</span></span>
<span data-ttu-id="24621-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24621-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24621-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="24621-110">Permission type</span></span>|<span data-ttu-id="24621-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="24621-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24621-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="24621-112">Delegated (work or school account)</span></span>|<span data-ttu-id="24621-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="24621-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="24621-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="24621-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24621-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="24621-115">Not supported.</span></span>|
|<span data-ttu-id="24621-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="24621-116">Application</span></span>|<span data-ttu-id="24621-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="24621-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24621-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="24621-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/{managementConditionId}
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="24621-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="24621-119">Optional query parameters</span></span>
<span data-ttu-id="24621-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="24621-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="24621-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="24621-121">Request headers</span></span>
|<span data-ttu-id="24621-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="24621-122">Header</span></span>|<span data-ttu-id="24621-123">Wert</span><span class="sxs-lookup"><span data-stu-id="24621-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24621-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="24621-124">Authorization</span></span>|<span data-ttu-id="24621-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="24621-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24621-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="24621-126">Accept</span></span>|<span data-ttu-id="24621-127">application/json</span><span class="sxs-lookup"><span data-stu-id="24621-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24621-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="24621-128">Request body</span></span>
<span data-ttu-id="24621-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="24621-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24621-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="24621-130">Response</span></span>
<span data-ttu-id="24621-131">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="24621-131">If successful, this method returns a `200 OK` response code and [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24621-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="24621-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="24621-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="24621-133">Request</span></span>
<span data-ttu-id="24621-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="24621-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
```

### <a name="response"></a><span data-ttu-id="24621-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="24621-135">Response</span></span>
<span data-ttu-id="24621-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="24621-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




