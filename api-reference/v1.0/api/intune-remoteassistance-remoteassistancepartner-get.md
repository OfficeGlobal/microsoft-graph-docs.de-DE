---
title: remoteAssistancePartner abrufen
description: Lesen von Eigenschaften und Beziehungen des remoteAssistancePartner-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 75531111b9fc6c8bc6571eee5ec3e8e149f5f813
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942136"
---
# <a name="get-remoteassistancepartner"></a><span data-ttu-id="c9612-103">remoteAssistancePartner abrufen</span><span class="sxs-lookup"><span data-stu-id="c9612-103">Get remoteAssistancePartner</span></span>

> <span data-ttu-id="c9612-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c9612-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c9612-105">Lesen von Eigenschaften und Beziehungen des [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c9612-105">Read properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c9612-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c9612-106">Prerequisites</span></span>
<span data-ttu-id="c9612-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9612-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9612-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c9612-109">Permission type</span></span>|<span data-ttu-id="c9612-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c9612-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9612-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c9612-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c9612-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c9612-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="c9612-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c9612-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9612-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c9612-114">Not supported.</span></span>|
|<span data-ttu-id="c9612-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c9612-115">Application</span></span>|<span data-ttu-id="c9612-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c9612-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9612-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c9612-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c9612-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c9612-118">Optional query parameters</span></span>
<span data-ttu-id="c9612-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c9612-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c9612-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c9612-120">Request headers</span></span>
|<span data-ttu-id="c9612-121">Header</span><span class="sxs-lookup"><span data-stu-id="c9612-121">Header</span></span>|<span data-ttu-id="c9612-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c9612-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9612-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9612-123">Authorization</span></span>|<span data-ttu-id="c9612-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c9612-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9612-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c9612-125">Accept</span></span>|<span data-ttu-id="c9612-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c9612-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9612-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c9612-127">Request body</span></span>
<span data-ttu-id="c9612-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c9612-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9612-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="c9612-129">Response</span></span>
<span data-ttu-id="c9612-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c9612-130">If successful, this method returns a `200 OK` response code and [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9612-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c9612-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="c9612-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c9612-132">Request</span></span>
<span data-ttu-id="c9612-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c9612-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

### <a name="response"></a><span data-ttu-id="c9612-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="c9612-134">Response</span></span>
<span data-ttu-id="c9612-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c9612-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "value": {
    "@odata.type": "#microsoft.graph.remoteAssistancePartner",
    "id": "7443c8b9-c8b9-7443-b9c8-4374b9c84374",
    "displayName": "Display Name value",
    "onboardingUrl": "https://example.com/onboardingUrl/",
    "onboardingStatus": "onboarding",
    "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
  }
}
```



