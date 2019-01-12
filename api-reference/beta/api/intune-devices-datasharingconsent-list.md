---
title: Liste dataSharingConsents
description: Listeneigenschaften und Beziehungen der DataSharingConsent-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4aa781f00bc24423b8b2f67bd783d824d73298ba
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948905"
---
# <a name="list-datasharingconsents"></a><span data-ttu-id="bfdff-103">Liste dataSharingConsents</span><span class="sxs-lookup"><span data-stu-id="bfdff-103">List dataSharingConsents</span></span>

> <span data-ttu-id="bfdff-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bfdff-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bfdff-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bfdff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bfdff-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bfdff-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bfdff-107">Listeneigenschaften und Beziehungen der [DataSharingConsent](../resources/intune-devices-datasharingconsent.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="bfdff-107">List properties and relationships of the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bfdff-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bfdff-108">Prerequisites</span></span>
<span data-ttu-id="bfdff-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfdff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfdff-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bfdff-111">Permission type</span></span>|<span data-ttu-id="bfdff-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bfdff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bfdff-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bfdff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bfdff-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfdff-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bfdff-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bfdff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bfdff-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bfdff-116">Not supported.</span></span>|
|<span data-ttu-id="bfdff-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bfdff-117">Application</span></span>|<span data-ttu-id="bfdff-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bfdff-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bfdff-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bfdff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/dataSharingConsents
```

## <a name="request-headers"></a><span data-ttu-id="bfdff-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bfdff-120">Request headers</span></span>
|<span data-ttu-id="bfdff-121">Header</span><span class="sxs-lookup"><span data-stu-id="bfdff-121">Header</span></span>|<span data-ttu-id="bfdff-122">Wert</span><span class="sxs-lookup"><span data-stu-id="bfdff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bfdff-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bfdff-123">Authorization</span></span>|<span data-ttu-id="bfdff-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bfdff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bfdff-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="bfdff-125">Accept</span></span>|<span data-ttu-id="bfdff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bfdff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bfdff-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bfdff-127">Request body</span></span>
<span data-ttu-id="bfdff-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bfdff-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bfdff-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="bfdff-129">Response</span></span>
<span data-ttu-id="bfdff-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [DataSharingConsent](../resources/intune-devices-datasharingconsent.md) .</span><span class="sxs-lookup"><span data-stu-id="bfdff-130">If successful, this method returns a `200 OK` response code and a collection of [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfdff-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bfdff-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="bfdff-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bfdff-132">Request</span></span>
<span data-ttu-id="bfdff-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bfdff-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents
```

### <a name="response"></a><span data-ttu-id="bfdff-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="bfdff-134">Response</span></span>
<span data-ttu-id="bfdff-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bfdff-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 447

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.dataSharingConsent",
      "id": "333387f7-87f7-3333-f787-3333f7873333",
      "serviceDisplayName": "Service Display Name value",
      "termsUrl": "https://example.com/termsUrl/",
      "granted": true,
      "grantDateTime": "2016-12-31T23:59:55.7154191-08:00",
      "grantedByUpn": "Granted By Upn value",
      "grantedByUserId": "Granted By User Id value"
    }
  ]
}
```





