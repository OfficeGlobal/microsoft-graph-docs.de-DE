---
title: telecomExpenseManagementPartners auflisten
description: Auflisten von Eigenschaften und Beziehungen der telecomExpenseManagementPartner-Objekte.
author: tfitzmac
ms.openlocfilehash: bb13ad66211ba4cac6b9f1bfa5de5890ba51ebed
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329722"
---
# <a name="list-telecomexpensemanagementpartners"></a><span data-ttu-id="1e50d-103">telecomExpenseManagementPartners auflisten</span><span class="sxs-lookup"><span data-stu-id="1e50d-103">List telecomExpenseManagementPartners</span></span>

> <span data-ttu-id="1e50d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1e50d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e50d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1e50d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1e50d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1e50d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e50d-107">Auflisten von Eigenschaften und Beziehungen der [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="1e50d-107">List properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1e50d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1e50d-108">Prerequisites</span></span>
<span data-ttu-id="1e50d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e50d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e50d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1e50d-111">Permission type</span></span>|<span data-ttu-id="1e50d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1e50d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e50d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1e50d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1e50d-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e50d-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="1e50d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1e50d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e50d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1e50d-116">Not supported.</span></span>|
|<span data-ttu-id="1e50d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1e50d-117">Application</span></span>|<span data-ttu-id="1e50d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1e50d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e50d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1e50d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="1e50d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1e50d-120">Request headers</span></span>
|<span data-ttu-id="1e50d-121">Header</span><span class="sxs-lookup"><span data-stu-id="1e50d-121">Header</span></span>|<span data-ttu-id="1e50d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="1e50d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e50d-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1e50d-123">Authorization</span></span>|<span data-ttu-id="1e50d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1e50d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e50d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1e50d-125">Accept</span></span>|<span data-ttu-id="1e50d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1e50d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e50d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1e50d-127">Request body</span></span>
<span data-ttu-id="1e50d-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1e50d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e50d-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="1e50d-129">Response</span></span>
<span data-ttu-id="1e50d-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Sammlung von Objekten des Typs [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1e50d-130">If successful, this method returns a `200 OK` response code and a collection of [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e50d-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1e50d-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="1e50d-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1e50d-132">Request</span></span>
<span data-ttu-id="1e50d-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1e50d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/telecomExpenseManagementPartners
```

### <a name="response"></a><span data-ttu-id="1e50d-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="1e50d-134">Response</span></span>
<span data-ttu-id="1e50d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1e50d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





