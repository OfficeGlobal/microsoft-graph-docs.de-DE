---
title: ManagementConditionStatements aufListen
description: AufListen von Eigenschaften und Beziehungen der managementConditionStatement-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 06c115638cb6e4e4dd12800ed19d512592874a32
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154656"
---
# <a name="list-managementconditionstatements"></a><span data-ttu-id="afdb9-103">ManagementConditionStatements aufListen</span><span class="sxs-lookup"><span data-stu-id="afdb9-103">List managementConditionStatements</span></span>

> <span data-ttu-id="afdb9-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="afdb9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="afdb9-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="afdb9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="afdb9-106">AufListen von Eigenschaften und Beziehungen der [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="afdb9-106">List properties and relationships of the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="afdb9-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="afdb9-107">Prerequisites</span></span>
<span data-ttu-id="afdb9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="afdb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="afdb9-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="afdb9-110">Permission type</span></span>|<span data-ttu-id="afdb9-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="afdb9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="afdb9-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="afdb9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="afdb9-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="afdb9-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="afdb9-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="afdb9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="afdb9-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="afdb9-115">Not supported.</span></span>|
|<span data-ttu-id="afdb9-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="afdb9-116">Application</span></span>|<span data-ttu-id="afdb9-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="afdb9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="afdb9-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="afdb9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditionStatements
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements
```

## <a name="request-headers"></a><span data-ttu-id="afdb9-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="afdb9-119">Request headers</span></span>
|<span data-ttu-id="afdb9-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="afdb9-120">Header</span></span>|<span data-ttu-id="afdb9-121">Wert</span><span class="sxs-lookup"><span data-stu-id="afdb9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="afdb9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="afdb9-122">Authorization</span></span>|<span data-ttu-id="afdb9-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="afdb9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="afdb9-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="afdb9-124">Accept</span></span>|<span data-ttu-id="afdb9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="afdb9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="afdb9-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="afdb9-126">Request body</span></span>
<span data-ttu-id="afdb9-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="afdb9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="afdb9-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="afdb9-128">Response</span></span>
<span data-ttu-id="afdb9-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="afdb9-129">If successful, this method returns a `200 OK` response code and a collection of [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afdb9-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="afdb9-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="afdb9-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="afdb9-131">Request</span></span>
<span data-ttu-id="afdb9-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="afdb9-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements
```

### <a name="response"></a><span data-ttu-id="afdb9-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="afdb9-133">Response</span></span>
<span data-ttu-id="afdb9-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="afdb9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




