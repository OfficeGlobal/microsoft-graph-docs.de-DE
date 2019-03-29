---
title: NetworkManagementConditions aufListen
description: AufListen von Eigenschaften und Beziehungen der networkManagementCondition-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9f9f5fc623c669d2e8fa3e627e9d268485ff33cb
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30967139"
---
# <a name="list-networkmanagementconditions"></a><span data-ttu-id="1c0e6-103">NetworkManagementConditions aufListen</span><span class="sxs-lookup"><span data-stu-id="1c0e6-103">List networkManagementConditions</span></span>

> <span data-ttu-id="1c0e6-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1c0e6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c0e6-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1c0e6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c0e6-106">AufListen von Eigenschaften und Beziehungen der [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="1c0e6-106">List properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c0e6-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1c0e6-107">Prerequisites</span></span>
<span data-ttu-id="1c0e6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c0e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c0e6-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1c0e6-110">Permission type</span></span>|<span data-ttu-id="1c0e6-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1c0e6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c0e6-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1c0e6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1c0e6-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c0e6-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1c0e6-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1c0e6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c0e6-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1c0e6-115">Not supported.</span></span>|
|<span data-ttu-id="1c0e6-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1c0e6-116">Application</span></span>|<span data-ttu-id="1c0e6-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1c0e6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c0e6-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1c0e6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="1c0e6-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1c0e6-119">Request headers</span></span>
|<span data-ttu-id="1c0e6-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1c0e6-120">Header</span></span>|<span data-ttu-id="1c0e6-121">Wert</span><span class="sxs-lookup"><span data-stu-id="1c0e6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c0e6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c0e6-122">Authorization</span></span>|<span data-ttu-id="1c0e6-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1c0e6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c0e6-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1c0e6-124">Accept</span></span>|<span data-ttu-id="1c0e6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1c0e6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c0e6-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1c0e6-126">Request body</span></span>
<span data-ttu-id="1c0e6-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1c0e6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c0e6-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="1c0e6-128">Response</span></span>
<span data-ttu-id="1c0e6-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1c0e6-129">If successful, this method returns a `200 OK` response code and a collection of [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c0e6-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1c0e6-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c0e6-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1c0e6-131">Request</span></span>
<span data-ttu-id="1c0e6-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1c0e6-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions
```

### <a name="response"></a><span data-ttu-id="1c0e6-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="1c0e6-133">Response</span></span>
<span data-ttu-id="1c0e6-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1c0e6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 511

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.networkManagementCondition",
      "id": "c2919b8f-9b8f-c291-8f9b-91c28f9b91c2",
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
  ]
}
```




