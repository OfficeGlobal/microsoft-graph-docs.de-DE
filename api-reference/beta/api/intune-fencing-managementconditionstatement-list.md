---
title: ManagementConditionStatements aufListen
description: AufListen von Eigenschaften und Beziehungen der managementConditionStatement-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 463984d270c66c14352014caa12430a561528383
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988959"
---
# <a name="list-managementconditionstatements"></a><span data-ttu-id="59994-103">ManagementConditionStatements aufListen</span><span class="sxs-lookup"><span data-stu-id="59994-103">List managementConditionStatements</span></span>

> <span data-ttu-id="59994-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="59994-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59994-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="59994-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59994-106">AufListen von Eigenschaften und Beziehungen der [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="59994-106">List properties and relationships of the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="59994-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="59994-107">Prerequisites</span></span>
<span data-ttu-id="59994-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59994-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59994-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="59994-110">Permission type</span></span>|<span data-ttu-id="59994-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="59994-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59994-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="59994-112">Delegated (work or school account)</span></span>|<span data-ttu-id="59994-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="59994-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="59994-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="59994-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59994-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="59994-115">Not supported.</span></span>|
|<span data-ttu-id="59994-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="59994-116">Application</span></span>|<span data-ttu-id="59994-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="59994-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="59994-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="59994-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditionStatements
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements
```

## <a name="request-headers"></a><span data-ttu-id="59994-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="59994-119">Request headers</span></span>
|<span data-ttu-id="59994-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="59994-120">Header</span></span>|<span data-ttu-id="59994-121">Wert</span><span class="sxs-lookup"><span data-stu-id="59994-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59994-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="59994-122">Authorization</span></span>|<span data-ttu-id="59994-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="59994-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59994-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="59994-124">Accept</span></span>|<span data-ttu-id="59994-125">application/json</span><span class="sxs-lookup"><span data-stu-id="59994-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59994-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="59994-126">Request body</span></span>
<span data-ttu-id="59994-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="59994-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59994-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="59994-128">Response</span></span>
<span data-ttu-id="59994-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="59994-129">If successful, this method returns a `200 OK` response code and a collection of [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59994-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="59994-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="59994-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="59994-131">Request</span></span>
<span data-ttu-id="59994-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="59994-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements
```

### <a name="response"></a><span data-ttu-id="59994-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="59994-133">Response</span></span>
<span data-ttu-id="59994-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="59994-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




