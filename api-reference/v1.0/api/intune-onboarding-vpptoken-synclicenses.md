---
title: syncLicenses-Aktion
description: Synchronisiert Lizenzen, die einem bestimmten appleVolumePurchaseProgramToken zugeordnet sind
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ca8f87309c316a3fe5ed42dd6b427cd2b069efd9
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254541"
---
# <a name="synclicenses-action"></a><span data-ttu-id="6043c-103">syncLicenses-Aktion</span><span class="sxs-lookup"><span data-stu-id="6043c-103">syncLicenses action</span></span>

> <span data-ttu-id="6043c-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6043c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6043c-105">Synchronisiert Lizenzen, die einem bestimmten appleVolumePurchaseProgramToken zugeordnet sind</span><span class="sxs-lookup"><span data-stu-id="6043c-105">Syncs licenses associated with a specific appleVolumePurchaseProgramToken</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6043c-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6043c-106">Prerequisites</span></span>
<span data-ttu-id="6043c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6043c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6043c-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6043c-109">Permission type</span></span>|<span data-ttu-id="6043c-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6043c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6043c-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6043c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6043c-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6043c-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6043c-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6043c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6043c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6043c-114">Not supported.</span></span>|
|<span data-ttu-id="6043c-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6043c-115">Application</span></span>|<span data-ttu-id="6043c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6043c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6043c-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6043c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

## <a name="request-headers"></a><span data-ttu-id="6043c-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6043c-118">Request headers</span></span>
|<span data-ttu-id="6043c-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6043c-119">Header</span></span>|<span data-ttu-id="6043c-120">Wert</span><span class="sxs-lookup"><span data-stu-id="6043c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6043c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6043c-121">Authorization</span></span>|<span data-ttu-id="6043c-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6043c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6043c-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6043c-123">Accept</span></span>|<span data-ttu-id="6043c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6043c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6043c-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6043c-125">Request body</span></span>
<span data-ttu-id="6043c-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6043c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6043c-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="6043c-127">Response</span></span>
<span data-ttu-id="6043c-128">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `200 OK` und ein Objekt des Typs [vppToken](../resources/intune-onboarding-vpptoken.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6043c-128">If successful, this action returns a `200 OK` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6043c-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6043c-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="6043c-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6043c-130">Request</span></span>
<span data-ttu-id="6043c-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6043c-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

### <a name="response"></a><span data-ttu-id="6043c-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="6043c-132">Response</span></span>
<span data-ttu-id="6043c-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6043c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



