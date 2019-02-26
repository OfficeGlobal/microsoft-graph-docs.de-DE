---
title: onpremisesConditionalAccessSettings abrufen
description: Lesen von Eigenschaften und Beziehungen des onPremisesConditionalAccessSettings-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 309e50407a62b0c4dbb6bde11a42fa49d2920343
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252763"
---
# <a name="get-onpremisesconditionalaccesssettings"></a><span data-ttu-id="53889-103">onpremisesConditionalAccessSettings abrufen</span><span class="sxs-lookup"><span data-stu-id="53889-103">Get onPremisesConditionalAccessSettings</span></span>

> <span data-ttu-id="53889-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="53889-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53889-105">Lesen von Eigenschaften und Beziehungen des [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="53889-105">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53889-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="53889-106">Prerequisites</span></span>
<span data-ttu-id="53889-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="53889-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="53889-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="53889-109">Permission type</span></span>|<span data-ttu-id="53889-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="53889-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53889-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="53889-111">Delegated (work or school account)</span></span>|<span data-ttu-id="53889-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="53889-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="53889-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="53889-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53889-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53889-114">Not supported.</span></span>|
|<span data-ttu-id="53889-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="53889-115">Application</span></span>|<span data-ttu-id="53889-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53889-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53889-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="53889-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/conditionalAccessSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="53889-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="53889-118">Optional query parameters</span></span>
<span data-ttu-id="53889-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="53889-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="53889-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="53889-120">Request headers</span></span>
|<span data-ttu-id="53889-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="53889-121">Header</span></span>|<span data-ttu-id="53889-122">Wert</span><span class="sxs-lookup"><span data-stu-id="53889-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53889-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="53889-123">Authorization</span></span>|<span data-ttu-id="53889-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="53889-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53889-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="53889-125">Accept</span></span>|<span data-ttu-id="53889-126">application/json</span><span class="sxs-lookup"><span data-stu-id="53889-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53889-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="53889-127">Request body</span></span>
<span data-ttu-id="53889-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="53889-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53889-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="53889-129">Response</span></span>
<span data-ttu-id="53889-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="53889-130">If successful, this method returns a `200 OK` response code and [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53889-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="53889-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="53889-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="53889-132">Request</span></span>
<span data-ttu-id="53889-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="53889-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/conditionalAccessSettings
```

### <a name="response"></a><span data-ttu-id="53889-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="53889-134">Response</span></span>
<span data-ttu-id="53889-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="53889-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 363

{
  "value": {
    "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
    "id": "a0efde21-de21-a0ef-21de-efa021deefa0",
    "enabled": true,
    "includedGroups": [
      "77c9d466-d466-77c9-66d4-c97766d4c977"
    ],
    "excludedGroups": [
      "2a0afae4-fae4-2a0a-e4fa-0a2ae4fa0a2a"
    ],
    "overrideDefaultRule": true
  }
}
```



