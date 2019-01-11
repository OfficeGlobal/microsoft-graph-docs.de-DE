---
title: VppToken abrufen
description: Lesen von Eigenschaften und Beziehungen des vppToken-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1c96ba7d364fdd6c424a48b2d159cc65bc49057a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835532"
---
# <a name="get-vpptoken"></a><span data-ttu-id="cb6fb-103">VppToken abrufen</span><span class="sxs-lookup"><span data-stu-id="cb6fb-103">Get vppToken</span></span>

> <span data-ttu-id="cb6fb-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="cb6fb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cb6fb-105">Lesen von Eigenschaften und Beziehungen des [vppToken](../resources/intune-onboarding-vpptoken.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="cb6fb-105">Read properties and relationships of the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cb6fb-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cb6fb-106">Prerequisites</span></span>
<span data-ttu-id="cb6fb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb6fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb6fb-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cb6fb-109">Permission type</span></span>|<span data-ttu-id="cb6fb-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cb6fb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb6fb-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cb6fb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cb6fb-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="cb6fb-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="cb6fb-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cb6fb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb6fb-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cb6fb-114">Not supported.</span></span>|
|<span data-ttu-id="cb6fb-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cb6fb-115">Application</span></span>|<span data-ttu-id="cb6fb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cb6fb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb6fb-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cb6fb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cb6fb-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="cb6fb-118">Optional query parameters</span></span>
<span data-ttu-id="cb6fb-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cb6fb-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cb6fb-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cb6fb-120">Request headers</span></span>
|<span data-ttu-id="cb6fb-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="cb6fb-121">Header</span></span>|<span data-ttu-id="cb6fb-122">Wert</span><span class="sxs-lookup"><span data-stu-id="cb6fb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb6fb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb6fb-123">Authorization</span></span>|<span data-ttu-id="cb6fb-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cb6fb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb6fb-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="cb6fb-125">Accept</span></span>|<span data-ttu-id="cb6fb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cb6fb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb6fb-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cb6fb-127">Request body</span></span>
<span data-ttu-id="cb6fb-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cb6fb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb6fb-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="cb6fb-129">Response</span></span>
<span data-ttu-id="cb6fb-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [vppToken](../resources/intune-onboarding-vpptoken.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cb6fb-130">If successful, this method returns a `200 OK` response code and [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb6fb-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cb6fb-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="cb6fb-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cb6fb-132">Request</span></span>
<span data-ttu-id="cb6fb-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cb6fb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens/{vppTokenId}
```

### <a name="response"></a><span data-ttu-id="cb6fb-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="cb6fb-134">Response</span></span>
<span data-ttu-id="cb6fb-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cb6fb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 619

{
  "value": {
    "@odata.type": "#microsoft.graph.vppToken",
    "id": "9ceb2f92-2f92-9ceb-922f-eb9c922feb9c",
    "organizationName": "Organization Name value",
    "vppTokenAccountType": "education",
    "appleId": "Apple Id value",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
    "token": "Token value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "state": "valid",
    "lastSyncStatus": "inProgress",
    "automaticallyUpdateApps": true,
    "countryOrRegion": "Country Or Region value"
  }
}
```



