---
title: VppToken abrufen
description: Lesen von Eigenschaften und Beziehungen des vppToken-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ec39e9a6352cb4a6c61d3947bba3c00cd91b2912
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250215"
---
# <a name="get-vpptoken"></a><span data-ttu-id="eb8d1-103">VppToken abrufen</span><span class="sxs-lookup"><span data-stu-id="eb8d1-103">Get vppToken</span></span>

> <span data-ttu-id="eb8d1-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="eb8d1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb8d1-105">Lesen von Eigenschaften und Beziehungen des [vppToken](../resources/intune-onboarding-vpptoken.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="eb8d1-105">Read properties and relationships of the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb8d1-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="eb8d1-106">Prerequisites</span></span>
<span data-ttu-id="eb8d1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="eb8d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="eb8d1-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eb8d1-109">Permission type</span></span>|<span data-ttu-id="eb8d1-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="eb8d1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb8d1-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eb8d1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eb8d1-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb8d1-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="eb8d1-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eb8d1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb8d1-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eb8d1-114">Not supported.</span></span>|
|<span data-ttu-id="eb8d1-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eb8d1-115">Application</span></span>|<span data-ttu-id="eb8d1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eb8d1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb8d1-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb8d1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eb8d1-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="eb8d1-118">Optional query parameters</span></span>
<span data-ttu-id="eb8d1-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="eb8d1-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eb8d1-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eb8d1-120">Request headers</span></span>
|<span data-ttu-id="eb8d1-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="eb8d1-121">Header</span></span>|<span data-ttu-id="eb8d1-122">Wert</span><span class="sxs-lookup"><span data-stu-id="eb8d1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb8d1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb8d1-123">Authorization</span></span>|<span data-ttu-id="eb8d1-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="eb8d1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb8d1-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="eb8d1-125">Accept</span></span>|<span data-ttu-id="eb8d1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eb8d1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb8d1-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="eb8d1-127">Request body</span></span>
<span data-ttu-id="eb8d1-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="eb8d1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb8d1-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb8d1-129">Response</span></span>
<span data-ttu-id="eb8d1-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [vppToken](../resources/intune-onboarding-vpptoken.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eb8d1-130">If successful, this method returns a `200 OK` response code and [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb8d1-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eb8d1-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb8d1-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb8d1-132">Request</span></span>
<span data-ttu-id="eb8d1-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="eb8d1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens/{vppTokenId}
```

### <a name="response"></a><span data-ttu-id="eb8d1-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb8d1-134">Response</span></span>
<span data-ttu-id="eb8d1-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eb8d1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



