---
title: GetManagementConditionsForPlatform-Funktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 16e60527c17d443ab75ff189fcbd8177e60a7ecb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975792"
---
# <a name="getmanagementconditionsforplatform-function"></a><span data-ttu-id="e2a59-103">GetManagementConditionsForPlatform-Funktion</span><span class="sxs-lookup"><span data-stu-id="e2a59-103">getManagementConditionsForPlatform function</span></span>

> <span data-ttu-id="e2a59-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e2a59-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2a59-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e2a59-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e2a59-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e2a59-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e2a59-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="e2a59-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e2a59-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e2a59-108">Prerequisites</span></span>
<span data-ttu-id="e2a59-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2a59-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2a59-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e2a59-111">Permission type</span></span>|<span data-ttu-id="e2a59-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e2a59-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2a59-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e2a59-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e2a59-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2a59-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e2a59-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e2a59-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2a59-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e2a59-116">Not supported.</span></span>|
|<span data-ttu-id="e2a59-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e2a59-117">Application</span></span>|<span data-ttu-id="e2a59-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e2a59-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2a59-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e2a59-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/getManagementConditionsForPlatform
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/getManagementConditionsForPlatform
```

## <a name="request-headers"></a><span data-ttu-id="e2a59-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e2a59-120">Request headers</span></span>
|<span data-ttu-id="e2a59-121">Header</span><span class="sxs-lookup"><span data-stu-id="e2a59-121">Header</span></span>|<span data-ttu-id="e2a59-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e2a59-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2a59-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2a59-123">Authorization</span></span>|<span data-ttu-id="e2a59-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e2a59-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2a59-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e2a59-125">Accept</span></span>|<span data-ttu-id="e2a59-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e2a59-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2a59-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e2a59-127">Request body</span></span>
<span data-ttu-id="e2a59-128">Geben Sie in der Anforderungs-URL die folgenden Abfrageparameter mit Werten an.</span><span class="sxs-lookup"><span data-stu-id="e2a59-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="e2a59-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="e2a59-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="e2a59-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e2a59-130">Property</span></span>|<span data-ttu-id="e2a59-131">Typ</span><span class="sxs-lookup"><span data-stu-id="e2a59-131">Type</span></span>|<span data-ttu-id="e2a59-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e2a59-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2a59-133">Plattform</span><span class="sxs-lookup"><span data-stu-id="e2a59-133">platform</span></span>|[<span data-ttu-id="e2a59-134">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="e2a59-134">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="e2a59-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="e2a59-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e2a59-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="e2a59-136">Response</span></span>
<span data-ttu-id="e2a59-137">Wenn erfolgreich, diese Funktion gibt eine `200 OK` Antwortcode und eine [ManagementCondition](../resources/intune-fencing-managementcondition.md) -Auflistung im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="e2a59-137">If successful, this function returns a `200 OK` response code and a [managementCondition](../resources/intune-fencing-managementcondition.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2a59-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e2a59-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="e2a59-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e2a59-139">Request</span></span>
<span data-ttu-id="e2a59-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e2a59-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/getManagementConditionsForPlatform(platform='parameterValue')
```

### <a name="response"></a><span data-ttu-id="e2a59-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="e2a59-141">Response</span></span>
<span data-ttu-id="e2a59-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e2a59-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 504

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managementCondition",
      "id": "5cb49381-9381-5cb4-8193-b45c8193b45c",
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





