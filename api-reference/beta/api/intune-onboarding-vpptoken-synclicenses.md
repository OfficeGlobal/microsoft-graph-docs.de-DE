---
title: syncLicenses-Aktion
description: Synchronisiert Lizenzen, die einem bestimmten appleVolumePurchaseProgramToken zugeordnet sind
ms.openlocfilehash: 36b0e141c398b17319711753928312a1353d2ab5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063845"
---
# <a name="synclicenses-action"></a><span data-ttu-id="db90f-103">syncLicenses-Aktion</span><span class="sxs-lookup"><span data-stu-id="db90f-103">syncLicenses action</span></span>

> <span data-ttu-id="db90f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="db90f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="db90f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="db90f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="db90f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="db90f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="db90f-107">Synchronisiert Lizenzen, die einem bestimmten appleVolumePurchaseProgramToken zugeordnet sind</span><span class="sxs-lookup"><span data-stu-id="db90f-107">Syncs licenses associated with a specific appleVolumePurchaseProgramToken</span></span>
## <a name="prerequisites"></a><span data-ttu-id="db90f-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="db90f-108">Prerequisites</span></span>
<span data-ttu-id="db90f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db90f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db90f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="db90f-111">Permission type</span></span>|<span data-ttu-id="db90f-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="db90f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db90f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="db90f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="db90f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db90f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="db90f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="db90f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db90f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="db90f-116">Not supported.</span></span>|
|<span data-ttu-id="db90f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="db90f-117">Application</span></span>|<span data-ttu-id="db90f-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="db90f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db90f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="db90f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

## <a name="request-headers"></a><span data-ttu-id="db90f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="db90f-120">Request headers</span></span>
|<span data-ttu-id="db90f-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="db90f-121">Header</span></span>|<span data-ttu-id="db90f-122">Wert</span><span class="sxs-lookup"><span data-stu-id="db90f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db90f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="db90f-123">Authorization</span></span>|<span data-ttu-id="db90f-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="db90f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db90f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="db90f-125">Accept</span></span>|<span data-ttu-id="db90f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="db90f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db90f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="db90f-127">Request body</span></span>
<span data-ttu-id="db90f-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="db90f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db90f-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="db90f-129">Response</span></span>
<span data-ttu-id="db90f-130">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `200 OK` und ein Objekt des Typs [vppToken](../resources/intune-onboarding-vpptoken.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="db90f-130">If successful, this action returns a `200 OK` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db90f-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="db90f-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="db90f-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="db90f-132">Request</span></span>
<span data-ttu-id="db90f-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="db90f-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

### <a name="response"></a><span data-ttu-id="db90f-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="db90f-134">Response</span></span>
<span data-ttu-id="db90f-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="db90f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1124

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
    "tokenActionResults": [
      {
        "@odata.type": "microsoft.graph.vppTokenActionResult",
        "actionName": "Action Name value",
        "actionState": "pending",
        "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
        "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
      }
    ],
    "lastSyncStatus": "inProgress",
    "automaticallyUpdateApps": true,
    "countryOrRegion": "Country Or Region value",
    "dataSharingConsentGranted": true,
    "displayName": "Display Name value",
    "locationName": "Location Name value",
    "claimTokenManagementFromExternalMdm": true
  }
}
```





