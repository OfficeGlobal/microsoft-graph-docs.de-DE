---
title: remoteAssistancePartners auflisten
description: Auflisten von Eigenschaften und Beziehungen der remoteAssistancePartner-Objekte.
author: tfitzmac
ms.openlocfilehash: 3394cc67ee1027267aa22b7e95eae8ae5dfdf6fb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307168"
---
# <a name="list-remoteassistancepartners"></a><span data-ttu-id="9c898-103">remoteAssistancePartners auflisten</span><span class="sxs-lookup"><span data-stu-id="9c898-103">List remoteAssistancePartners</span></span>

> <span data-ttu-id="9c898-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9c898-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9c898-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9c898-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9c898-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9c898-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9c898-107">Auflisten von Eigenschaften und Beziehungen der [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="9c898-107">List properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9c898-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9c898-108">Prerequisites</span></span>
<span data-ttu-id="9c898-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c898-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c898-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9c898-111">Permission type</span></span>|<span data-ttu-id="9c898-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9c898-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c898-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9c898-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9c898-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c898-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="9c898-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9c898-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c898-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9c898-116">Not supported.</span></span>|
|<span data-ttu-id="9c898-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9c898-117">Application</span></span>|<span data-ttu-id="9c898-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9c898-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c898-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9c898-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="9c898-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9c898-120">Request headers</span></span>
|<span data-ttu-id="9c898-121">Header</span><span class="sxs-lookup"><span data-stu-id="9c898-121">Header</span></span>|<span data-ttu-id="9c898-122">Wert</span><span class="sxs-lookup"><span data-stu-id="9c898-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c898-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="9c898-123">Authorization</span></span>|<span data-ttu-id="9c898-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9c898-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c898-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9c898-125">Accept</span></span>|<span data-ttu-id="9c898-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9c898-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c898-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9c898-127">Request body</span></span>
<span data-ttu-id="9c898-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9c898-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c898-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="9c898-129">Response</span></span>
<span data-ttu-id="9c898-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Sammlung von Objekten des Typs [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9c898-130">If successful, this method returns a `200 OK` response code and a collection of [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c898-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9c898-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="9c898-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9c898-132">Request</span></span>
<span data-ttu-id="9c898-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9c898-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners
```

### <a name="response"></a><span data-ttu-id="9c898-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="9c898-134">Response</span></span>
<span data-ttu-id="9c898-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9c898-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 372

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.remoteAssistancePartner",
      "id": "7443c8b9-c8b9-7443-b9c8-4374b9c84374",
      "displayName": "Display Name value",
      "onboardingUrl": "https://example.com/onboardingUrl/",
      "onboardingStatus": "onboarding",
      "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
    }
  ]
}
```





