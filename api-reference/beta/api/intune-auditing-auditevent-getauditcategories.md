---
title: getAuditCategories-Funktion
description: Noch nicht dokumentiert
author: tfitzmac
ms.openlocfilehash: da8313c49b37af077d0ba22e1f51204b7f8a2771
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314000"
---
# <a name="getauditcategories-function"></a><span data-ttu-id="aaff6-103">getAuditCategories-Funktion</span><span class="sxs-lookup"><span data-stu-id="aaff6-103">getAuditCategories function</span></span>

> <span data-ttu-id="aaff6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="aaff6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aaff6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="aaff6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aaff6-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="aaff6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aaff6-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="aaff6-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aaff6-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="aaff6-108">Prerequisites</span></span>
<span data-ttu-id="aaff6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aaff6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aaff6-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="aaff6-111">Permission type</span></span>|<span data-ttu-id="aaff6-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="aaff6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aaff6-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="aaff6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aaff6-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="aaff6-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="aaff6-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="aaff6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aaff6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aaff6-116">Not supported.</span></span>|
|<span data-ttu-id="aaff6-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="aaff6-117">Application</span></span>|<span data-ttu-id="aaff6-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aaff6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aaff6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aaff6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditCategories
```

## <a name="request-headers"></a><span data-ttu-id="aaff6-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="aaff6-120">Request headers</span></span>
|<span data-ttu-id="aaff6-121">Header</span><span class="sxs-lookup"><span data-stu-id="aaff6-121">Header</span></span>|<span data-ttu-id="aaff6-122">Wert</span><span class="sxs-lookup"><span data-stu-id="aaff6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aaff6-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="aaff6-123">Authorization</span></span>|<span data-ttu-id="aaff6-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="aaff6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aaff6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aaff6-125">Accept</span></span>|<span data-ttu-id="aaff6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aaff6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aaff6-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="aaff6-127">Request body</span></span>
<span data-ttu-id="aaff6-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="aaff6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aaff6-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="aaff6-129">Response</span></span>
<span data-ttu-id="aaff6-130">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und eine Collection von Objekten des Typs „String“ im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="aaff6-130">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aaff6-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="aaff6-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="aaff6-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aaff6-132">Request</span></span>
<span data-ttu-id="aaff6-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="aaff6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents/getAuditCategories
```

### <a name="response"></a><span data-ttu-id="aaff6-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="aaff6-134">Response</span></span>
<span data-ttu-id="aaff6-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aaff6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 57

{
  "value": [
    "Get Audit Categories value"
  ]
}
```





