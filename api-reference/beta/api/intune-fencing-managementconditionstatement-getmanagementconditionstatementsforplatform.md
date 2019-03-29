---
title: getManagementConditionStatementsForPlatform-Funktion
description: Noch nicht dokumentiert.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ab12a9d04cb385660932f33efd7ab4129adf889e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30981895"
---
# <a name="getmanagementconditionstatementsforplatform-function"></a><span data-ttu-id="05aa1-103">getManagementConditionStatementsForPlatform-Funktion</span><span class="sxs-lookup"><span data-stu-id="05aa1-103">getManagementConditionStatementsForPlatform function</span></span>

> <span data-ttu-id="05aa1-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="05aa1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05aa1-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="05aa1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05aa1-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="05aa1-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05aa1-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="05aa1-107">Prerequisites</span></span>
<span data-ttu-id="05aa1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05aa1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05aa1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="05aa1-110">Permission type</span></span>|<span data-ttu-id="05aa1-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="05aa1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05aa1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="05aa1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="05aa1-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="05aa1-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="05aa1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="05aa1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05aa1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="05aa1-115">Not supported.</span></span>|
|<span data-ttu-id="05aa1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="05aa1-116">Application</span></span>|<span data-ttu-id="05aa1-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="05aa1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05aa1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="05aa1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditionStatements/getManagementConditionStatementsForPlatform
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/getManagementConditionStatementsForPlatform
```

## <a name="request-headers"></a><span data-ttu-id="05aa1-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="05aa1-119">Request headers</span></span>
|<span data-ttu-id="05aa1-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="05aa1-120">Header</span></span>|<span data-ttu-id="05aa1-121">Wert</span><span class="sxs-lookup"><span data-stu-id="05aa1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05aa1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="05aa1-122">Authorization</span></span>|<span data-ttu-id="05aa1-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="05aa1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05aa1-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="05aa1-124">Accept</span></span>|<span data-ttu-id="05aa1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="05aa1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05aa1-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="05aa1-126">Request body</span></span>
<span data-ttu-id="05aa1-127">Stellen Sie in der URL der Anforderung die folgenden Abfrageparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="05aa1-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="05aa1-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="05aa1-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="05aa1-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="05aa1-129">Property</span></span>|<span data-ttu-id="05aa1-130">Typ</span><span class="sxs-lookup"><span data-stu-id="05aa1-130">Type</span></span>|<span data-ttu-id="05aa1-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="05aa1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05aa1-132">Plattform</span><span class="sxs-lookup"><span data-stu-id="05aa1-132">platform</span></span>|[<span data-ttu-id="05aa1-133">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="05aa1-133">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="05aa1-134">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="05aa1-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="05aa1-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="05aa1-135">Response</span></span>
<span data-ttu-id="05aa1-136">Bei erfolgreicher Ausführung gibt die Funktion den `200 OK` Antwortcode und eine [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Auflistung im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="05aa1-136">If successful, this function returns a `200 OK` response code and a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05aa1-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="05aa1-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="05aa1-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="05aa1-138">Request</span></span>
<span data-ttu-id="05aa1-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="05aa1-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/getManagementConditionStatementsForPlatform(platform='parameterValue')
```

### <a name="response"></a><span data-ttu-id="05aa1-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="05aa1-140">Response</span></span>
<span data-ttu-id="05aa1-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="05aa1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




