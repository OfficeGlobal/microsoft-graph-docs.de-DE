---
title: GetManagementConditionStatementsForPlatform-Funktion
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cf8e3daec196adc6b9124d91e66b82ab78a03337
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419667"
---
# <a name="getmanagementconditionstatementsforplatform-function"></a><span data-ttu-id="0bf40-103">GetManagementConditionStatementsForPlatform-Funktion</span><span class="sxs-lookup"><span data-stu-id="0bf40-103">getManagementConditionStatementsForPlatform function</span></span>

> <span data-ttu-id="0bf40-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="0bf40-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0bf40-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0bf40-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0bf40-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0bf40-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0bf40-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="0bf40-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0bf40-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0bf40-108">Prerequisites</span></span>
<span data-ttu-id="0bf40-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0bf40-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0bf40-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0bf40-111">Permission type</span></span>|<span data-ttu-id="0bf40-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0bf40-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0bf40-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0bf40-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0bf40-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0bf40-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0bf40-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0bf40-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0bf40-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0bf40-116">Not supported.</span></span>|
|<span data-ttu-id="0bf40-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0bf40-117">Application</span></span>|<span data-ttu-id="0bf40-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0bf40-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0bf40-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0bf40-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditionStatements/getManagementConditionStatementsForPlatform
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/getManagementConditionStatementsForPlatform
```

## <a name="request-headers"></a><span data-ttu-id="0bf40-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0bf40-120">Request headers</span></span>
|<span data-ttu-id="0bf40-121">Header</span><span class="sxs-lookup"><span data-stu-id="0bf40-121">Header</span></span>|<span data-ttu-id="0bf40-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0bf40-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0bf40-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="0bf40-123">Authorization</span></span>|<span data-ttu-id="0bf40-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0bf40-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0bf40-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0bf40-125">Accept</span></span>|<span data-ttu-id="0bf40-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0bf40-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bf40-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0bf40-127">Request body</span></span>
<span data-ttu-id="0bf40-128">Geben Sie in der Anforderungs-URL die folgenden Abfrageparameter mit Werten an.</span><span class="sxs-lookup"><span data-stu-id="0bf40-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="0bf40-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="0bf40-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="0bf40-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0bf40-130">Property</span></span>|<span data-ttu-id="0bf40-131">Typ</span><span class="sxs-lookup"><span data-stu-id="0bf40-131">Type</span></span>|<span data-ttu-id="0bf40-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0bf40-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bf40-133">Plattform</span><span class="sxs-lookup"><span data-stu-id="0bf40-133">platform</span></span>|[<span data-ttu-id="0bf40-134">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="0bf40-134">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="0bf40-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="0bf40-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0bf40-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="0bf40-136">Response</span></span>
<span data-ttu-id="0bf40-137">Wenn erfolgreich, diese Funktion gibt eine `200 OK` Antwortcode und eine [ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Auflistung im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="0bf40-137">If successful, this function returns a `200 OK` response code and a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bf40-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0bf40-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="0bf40-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0bf40-139">Request</span></span>
<span data-ttu-id="0bf40-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0bf40-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/getManagementConditionStatementsForPlatform(platform='parameterValue')
```

### <a name="response"></a><span data-ttu-id="0bf40-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="0bf40-141">Response</span></span>
<span data-ttu-id="0bf40-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0bf40-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




