---
title: onpremisesConditionalAccessSettings abrufen
description: Lesen von Eigenschaften und Beziehungen des onPremisesConditionalAccessSettings-Objekts.
author: tfitzmac
ms.openlocfilehash: 31f5bb9804c8a4a469d877727f073919dfdff73e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332354"
---
# <a name="get-onpremisesconditionalaccesssettings"></a><span data-ttu-id="b2b59-103">onpremisesConditionalAccessSettings abrufen</span><span class="sxs-lookup"><span data-stu-id="b2b59-103">Get onPremisesConditionalAccessSettings</span></span>

> <span data-ttu-id="b2b59-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b2b59-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b2b59-105">Lesen von Eigenschaften und Beziehungen des [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b2b59-105">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b2b59-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b2b59-106">Prerequisites</span></span>
<span data-ttu-id="b2b59-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2b59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2b59-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b2b59-109">Permission type</span></span>|<span data-ttu-id="b2b59-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b2b59-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2b59-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b2b59-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b2b59-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2b59-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b2b59-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b2b59-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2b59-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b2b59-114">Not supported.</span></span>|
|<span data-ttu-id="b2b59-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b2b59-115">Application</span></span>|<span data-ttu-id="b2b59-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b2b59-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2b59-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b2b59-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/conditionalAccessSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b2b59-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b2b59-118">Optional query parameters</span></span>
<span data-ttu-id="b2b59-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b2b59-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b2b59-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b2b59-120">Request headers</span></span>
|<span data-ttu-id="b2b59-121">Header</span><span class="sxs-lookup"><span data-stu-id="b2b59-121">Header</span></span>|<span data-ttu-id="b2b59-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b2b59-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2b59-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b2b59-123">Authorization</span></span>|<span data-ttu-id="b2b59-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b2b59-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2b59-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b2b59-125">Accept</span></span>|<span data-ttu-id="b2b59-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b2b59-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2b59-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b2b59-127">Request body</span></span>
<span data-ttu-id="b2b59-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b2b59-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2b59-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="b2b59-129">Response</span></span>
<span data-ttu-id="b2b59-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b2b59-130">If successful, this method returns a `200 OK` response code and [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2b59-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b2b59-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b2b59-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b2b59-132">Request</span></span>
<span data-ttu-id="b2b59-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b2b59-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/conditionalAccessSettings
```

### <a name="response"></a><span data-ttu-id="b2b59-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="b2b59-134">Response</span></span>
<span data-ttu-id="b2b59-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b2b59-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



