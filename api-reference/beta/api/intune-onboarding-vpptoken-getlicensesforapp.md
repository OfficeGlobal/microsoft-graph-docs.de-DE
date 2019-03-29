---
title: getLicensesForApp-Funktion
description: Noch nicht dokumentiert.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 679f44364dc5d534fa58e874502b5b51609a995f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975952"
---
# <a name="getlicensesforapp-function"></a><span data-ttu-id="cd85b-103">getLicensesForApp-Funktion</span><span class="sxs-lookup"><span data-stu-id="cd85b-103">getLicensesForApp function</span></span>

> <span data-ttu-id="cd85b-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cd85b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd85b-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="cd85b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd85b-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="cd85b-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd85b-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cd85b-107">Prerequisites</span></span>
<span data-ttu-id="cd85b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd85b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd85b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cd85b-110">Permission type</span></span>|<span data-ttu-id="cd85b-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cd85b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd85b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cd85b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cd85b-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="cd85b-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="cd85b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cd85b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd85b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cd85b-115">Not supported.</span></span>|
|<span data-ttu-id="cd85b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cd85b-116">Application</span></span>|<span data-ttu-id="cd85b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cd85b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd85b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd85b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens/getLicensesForApp
```

## <a name="request-headers"></a><span data-ttu-id="cd85b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cd85b-119">Request headers</span></span>
|<span data-ttu-id="cd85b-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="cd85b-120">Header</span></span>|<span data-ttu-id="cd85b-121">Wert</span><span class="sxs-lookup"><span data-stu-id="cd85b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd85b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd85b-122">Authorization</span></span>|<span data-ttu-id="cd85b-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cd85b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd85b-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="cd85b-124">Accept</span></span>|<span data-ttu-id="cd85b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cd85b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd85b-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cd85b-126">Request body</span></span>
<span data-ttu-id="cd85b-127">Stellen Sie in der URL der Anforderung die folgenden Abfrageparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="cd85b-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="cd85b-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="cd85b-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="cd85b-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cd85b-129">Property</span></span>|<span data-ttu-id="cd85b-130">Typ</span><span class="sxs-lookup"><span data-stu-id="cd85b-130">Type</span></span>|<span data-ttu-id="cd85b-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cd85b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd85b-132">bundleId</span><span class="sxs-lookup"><span data-stu-id="cd85b-132">bundleId</span></span>|<span data-ttu-id="cd85b-133">String</span><span class="sxs-lookup"><span data-stu-id="cd85b-133">String</span></span>|<span data-ttu-id="cd85b-134">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="cd85b-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="cd85b-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd85b-135">Response</span></span>
<span data-ttu-id="cd85b-136">Bei erfolgreicher Ausführung gibt die Funktion den `200 OK` Antwortcode und eine [vppTokenLicenseSummary](../resources/intune-onboarding-vpptokenlicensesummary.md) -Auflistung im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="cd85b-136">If successful, this function returns a `200 OK` response code and a [vppTokenLicenseSummary](../resources/intune-onboarding-vpptokenlicensesummary.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd85b-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cd85b-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd85b-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd85b-138">Request</span></span>
<span data-ttu-id="cd85b-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cd85b-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/getLicensesForApp(bundleId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="cd85b-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd85b-140">Response</span></span>
<span data-ttu-id="cd85b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cd85b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 298

{
  "value": [
    {
      "@odata.type": "microsoft.graph.vppTokenLicenseSummary",
      "vppTokenId": "Vpp Token Id value",
      "appleId": "Apple Id value",
      "organizationName": "Organization Name value",
      "availableLicenseCount": 5,
      "usedLicenseCount": 0
    }
  ]
}
```




