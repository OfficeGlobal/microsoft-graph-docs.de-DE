---
title: telecomExpenseManagementPartners auflisten
description: Auflisten von Eigenschaften und Beziehungen der telecomExpenseManagementPartner-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f86d5c65bf1a2b6a8d31f347a4797485db0974f5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970759"
---
# <a name="list-telecomexpensemanagementpartners"></a><span data-ttu-id="2318c-103">telecomExpenseManagementPartners auflisten</span><span class="sxs-lookup"><span data-stu-id="2318c-103">List telecomExpenseManagementPartners</span></span>

> <span data-ttu-id="2318c-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2318c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2318c-105">Auflisten von Eigenschaften und Beziehungen der [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="2318c-105">List properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2318c-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2318c-106">Prerequisites</span></span>
<span data-ttu-id="2318c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2318c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2318c-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2318c-109">Permission type</span></span>|<span data-ttu-id="2318c-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2318c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2318c-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2318c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2318c-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2318c-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2318c-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2318c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2318c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2318c-114">Not supported.</span></span>|
|<span data-ttu-id="2318c-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2318c-115">Application</span></span>|<span data-ttu-id="2318c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2318c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2318c-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2318c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="2318c-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2318c-118">Request headers</span></span>
|<span data-ttu-id="2318c-119">Header</span><span class="sxs-lookup"><span data-stu-id="2318c-119">Header</span></span>|<span data-ttu-id="2318c-120">Wert</span><span class="sxs-lookup"><span data-stu-id="2318c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2318c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2318c-121">Authorization</span></span>|<span data-ttu-id="2318c-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2318c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2318c-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2318c-123">Accept</span></span>|<span data-ttu-id="2318c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2318c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2318c-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2318c-125">Request body</span></span>
<span data-ttu-id="2318c-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2318c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2318c-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="2318c-127">Response</span></span>
<span data-ttu-id="2318c-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Sammlung von Objekten des Typs [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2318c-128">If successful, this method returns a `200 OK` response code and a collection of [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2318c-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2318c-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="2318c-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2318c-130">Request</span></span>
<span data-ttu-id="2318c-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2318c-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners
```

### <a name="response"></a><span data-ttu-id="2318c-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="2318c-132">Response</span></span>
<span data-ttu-id="2318c-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2318c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 358

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
      "id": "47a3b399-b399-47a3-99b3-a34799b3a347",
      "displayName": "Display Name value",
      "url": "Url value",
      "appAuthorized": true,
      "enabled": true,
      "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
    }
  ]
}
```



