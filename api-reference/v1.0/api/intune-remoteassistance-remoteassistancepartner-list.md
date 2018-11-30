---
title: remoteAssistancePartners auflisten
description: Auflisten von Eigenschaften und Beziehungen der remoteAssistancePartner-Objekte.
ms.openlocfilehash: 4f3095cf9f031a7dd6f0046fc9cdfdc28e2fb673
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018037"
---
# <a name="list-remoteassistancepartners"></a><span data-ttu-id="be45b-103">remoteAssistancePartners auflisten</span><span class="sxs-lookup"><span data-stu-id="be45b-103">List remoteAssistancePartners</span></span>

> <span data-ttu-id="be45b-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="be45b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be45b-105">Auflisten von Eigenschaften und Beziehungen der [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="be45b-105">List properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="be45b-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="be45b-106">Prerequisites</span></span>
<span data-ttu-id="be45b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be45b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be45b-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="be45b-109">Permission type</span></span>|<span data-ttu-id="be45b-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="be45b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be45b-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="be45b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="be45b-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="be45b-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="be45b-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="be45b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be45b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="be45b-114">Not supported.</span></span>|
|<span data-ttu-id="be45b-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="be45b-115">Application</span></span>|<span data-ttu-id="be45b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="be45b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be45b-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="be45b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="be45b-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="be45b-118">Request headers</span></span>
|<span data-ttu-id="be45b-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="be45b-119">Header</span></span>|<span data-ttu-id="be45b-120">Wert</span><span class="sxs-lookup"><span data-stu-id="be45b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be45b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="be45b-121">Authorization</span></span>|<span data-ttu-id="be45b-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="be45b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be45b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="be45b-123">Accept</span></span>|<span data-ttu-id="be45b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="be45b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be45b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="be45b-125">Request body</span></span>
<span data-ttu-id="be45b-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="be45b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be45b-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="be45b-127">Response</span></span>
<span data-ttu-id="be45b-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Sammlung von Objekten des Typs [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="be45b-128">If successful, this method returns a `200 OK` response code and a collection of [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be45b-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="be45b-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="be45b-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="be45b-130">Request</span></span>
<span data-ttu-id="be45b-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="be45b-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners
```

### <a name="response"></a><span data-ttu-id="be45b-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="be45b-132">Response</span></span>
<span data-ttu-id="be45b-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="be45b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



