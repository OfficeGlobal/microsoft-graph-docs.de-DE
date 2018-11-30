---
title: syncLicenses-Aktion
description: Synchronisiert Lizenzen, die einem bestimmten appleVolumePurchaseProgramToken zugeordnet sind
ms.openlocfilehash: 167fbb16b9377e3134c1a4403433449341e21562
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020062"
---
# <a name="synclicenses-action"></a><span data-ttu-id="7b8d5-103">syncLicenses-Aktion</span><span class="sxs-lookup"><span data-stu-id="7b8d5-103">syncLicenses action</span></span>

> <span data-ttu-id="7b8d5-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7b8d5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7b8d5-105">Synchronisiert Lizenzen, die einem bestimmten appleVolumePurchaseProgramToken zugeordnet sind</span><span class="sxs-lookup"><span data-stu-id="7b8d5-105">Syncs licenses associated with a specific appleVolumePurchaseProgramToken</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7b8d5-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7b8d5-106">Prerequisites</span></span>
<span data-ttu-id="7b8d5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b8d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b8d5-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7b8d5-109">Permission type</span></span>|<span data-ttu-id="7b8d5-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7b8d5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b8d5-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7b8d5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7b8d5-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b8d5-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7b8d5-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7b8d5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b8d5-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7b8d5-114">Not supported.</span></span>|
|<span data-ttu-id="7b8d5-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7b8d5-115">Application</span></span>|<span data-ttu-id="7b8d5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7b8d5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b8d5-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b8d5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

## <a name="request-headers"></a><span data-ttu-id="7b8d5-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7b8d5-118">Request headers</span></span>
|<span data-ttu-id="7b8d5-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7b8d5-119">Header</span></span>|<span data-ttu-id="7b8d5-120">Wert</span><span class="sxs-lookup"><span data-stu-id="7b8d5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b8d5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b8d5-121">Authorization</span></span>|<span data-ttu-id="7b8d5-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7b8d5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b8d5-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7b8d5-123">Accept</span></span>|<span data-ttu-id="7b8d5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7b8d5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b8d5-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7b8d5-125">Request body</span></span>
<span data-ttu-id="7b8d5-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7b8d5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b8d5-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b8d5-127">Response</span></span>
<span data-ttu-id="7b8d5-128">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `200 OK` und ein Objekt des Typs [vppToken](../resources/intune-onboarding-vpptoken.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7b8d5-128">If successful, this action returns a `200 OK` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b8d5-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7b8d5-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="7b8d5-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b8d5-130">Request</span></span>
<span data-ttu-id="7b8d5-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7b8d5-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

### <a name="response"></a><span data-ttu-id="7b8d5-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b8d5-132">Response</span></span>
<span data-ttu-id="7b8d5-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7b8d5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



