---
title: syncLicenses-Aktion
description: Synchronisiert Lizenzen, die einem bestimmten appleVolumePurchaseProgramToken zugeordnet sind
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fafcb15fb6911cf1c8ec7c25284ac95f6d848408
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30968966"
---
# <a name="synclicenses-action"></a><span data-ttu-id="72433-103">syncLicenses-Aktion</span><span class="sxs-lookup"><span data-stu-id="72433-103">syncLicenses action</span></span>

> <span data-ttu-id="72433-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="72433-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72433-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="72433-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72433-106">Synchronisiert Lizenzen, die einem bestimmten appleVolumePurchaseProgramToken zugeordnet sind</span><span class="sxs-lookup"><span data-stu-id="72433-106">Syncs licenses associated with a specific appleVolumePurchaseProgramToken</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72433-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="72433-107">Prerequisites</span></span>
<span data-ttu-id="72433-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72433-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72433-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="72433-110">Permission type</span></span>|<span data-ttu-id="72433-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="72433-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72433-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="72433-112">Delegated (work or school account)</span></span>|<span data-ttu-id="72433-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72433-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="72433-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="72433-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72433-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="72433-115">Not supported.</span></span>|
|<span data-ttu-id="72433-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="72433-116">Application</span></span>|<span data-ttu-id="72433-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="72433-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="72433-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="72433-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

## <a name="request-headers"></a><span data-ttu-id="72433-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="72433-119">Request headers</span></span>
|<span data-ttu-id="72433-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="72433-120">Header</span></span>|<span data-ttu-id="72433-121">Wert</span><span class="sxs-lookup"><span data-stu-id="72433-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72433-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="72433-122">Authorization</span></span>|<span data-ttu-id="72433-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="72433-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72433-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="72433-124">Accept</span></span>|<span data-ttu-id="72433-125">application/json</span><span class="sxs-lookup"><span data-stu-id="72433-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72433-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="72433-126">Request body</span></span>
<span data-ttu-id="72433-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="72433-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72433-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="72433-128">Response</span></span>
<span data-ttu-id="72433-129">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `200 OK` und ein Objekt des Typs [vppToken](../resources/intune-onboarding-vpptoken.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="72433-129">If successful, this action returns a `200 OK` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72433-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="72433-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="72433-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="72433-131">Request</span></span>
<span data-ttu-id="72433-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="72433-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

### <a name="response"></a><span data-ttu-id="72433-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="72433-133">Response</span></span>
<span data-ttu-id="72433-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="72433-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1192

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
    "claimTokenManagementFromExternalMdm": true,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```




