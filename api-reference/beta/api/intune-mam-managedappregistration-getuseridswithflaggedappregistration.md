---
title: Funktion getUserIdsWithFlaggedAppRegistration
description: Noch nicht dokumentiert
author: tfitzmac
ms.openlocfilehash: 7f57ab3af48ac7e815b914be3339435d6be58fc4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329379"
---
# <a name="getuseridswithflaggedappregistration-function"></a><span data-ttu-id="a10f1-103">Funktion getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="a10f1-103">getUserIdsWithFlaggedAppRegistration function</span></span>

> <span data-ttu-id="a10f1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a10f1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a10f1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a10f1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a10f1-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a10f1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a10f1-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="a10f1-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a10f1-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a10f1-108">Prerequisites</span></span>
<span data-ttu-id="a10f1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a10f1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a10f1-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a10f1-111">Permission type</span></span>|<span data-ttu-id="a10f1-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a10f1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a10f1-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a10f1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a10f1-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a10f1-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a10f1-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a10f1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a10f1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a10f1-116">Not supported.</span></span>|
|<span data-ttu-id="a10f1-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a10f1-117">Application</span></span>|<span data-ttu-id="a10f1-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a10f1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a10f1-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a10f1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

## <a name="request-headers"></a><span data-ttu-id="a10f1-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a10f1-120">Request headers</span></span>
|<span data-ttu-id="a10f1-121">Header</span><span class="sxs-lookup"><span data-stu-id="a10f1-121">Header</span></span>|<span data-ttu-id="a10f1-122">Wert</span><span class="sxs-lookup"><span data-stu-id="a10f1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a10f1-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="a10f1-123">Authorization</span></span>|<span data-ttu-id="a10f1-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a10f1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a10f1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a10f1-125">Accept</span></span>|<span data-ttu-id="a10f1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a10f1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a10f1-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a10f1-127">Request body</span></span>
<span data-ttu-id="a10f1-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a10f1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a10f1-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="a10f1-129">Response</span></span>
<span data-ttu-id="a10f1-130">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und eine Collection von Objekten des Typs „String“ im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a10f1-130">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a10f1-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a10f1-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a10f1-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a10f1-132">Request</span></span>
<span data-ttu-id="a10f1-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a10f1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

### <a name="response"></a><span data-ttu-id="a10f1-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="a10f1-134">Response</span></span>
<span data-ttu-id="a10f1-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a10f1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 79

{
  "value": [
    "Get User Ids With Flagged App Registration value"
  ]
}
```





