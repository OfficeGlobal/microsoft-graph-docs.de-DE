---
title: vppTokens auflisten
description: Auflisten von Eigenschaften und Beziehungen der vppToken-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f10f196912448a591d6a96559b58dec6bf4b322a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144982"
---
# <a name="list-vpptokens"></a><span data-ttu-id="c9829-103">vppTokens auflisten</span><span class="sxs-lookup"><span data-stu-id="c9829-103">List vppTokens</span></span>

> <span data-ttu-id="c9829-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c9829-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9829-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c9829-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9829-106">Auflisten von Eigenschaften und Beziehungen der [vppToken](../resources/intune-onboarding-vpptoken.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="c9829-106">List properties and relationships of the [vppToken](../resources/intune-onboarding-vpptoken.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9829-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c9829-107">Prerequisites</span></span>
<span data-ttu-id="c9829-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c9829-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c9829-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c9829-110">Permission type</span></span>|<span data-ttu-id="c9829-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c9829-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9829-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c9829-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c9829-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c9829-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="c9829-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c9829-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9829-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c9829-115">Not supported.</span></span>|
|<span data-ttu-id="c9829-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c9829-116">Application</span></span>|<span data-ttu-id="c9829-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c9829-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9829-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c9829-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a><span data-ttu-id="c9829-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c9829-119">Request headers</span></span>
|<span data-ttu-id="c9829-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c9829-120">Header</span></span>|<span data-ttu-id="c9829-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c9829-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9829-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9829-122">Authorization</span></span>|<span data-ttu-id="c9829-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c9829-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9829-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c9829-124">Accept</span></span>|<span data-ttu-id="c9829-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c9829-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9829-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c9829-126">Request body</span></span>
<span data-ttu-id="c9829-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c9829-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9829-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="c9829-128">Response</span></span>
<span data-ttu-id="c9829-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [vppToken](../resources/intune-onboarding-vpptoken.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c9829-129">If successful, this method returns a `200 OK` response code and a collection of [vppToken](../resources/intune-onboarding-vpptoken.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9829-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c9829-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9829-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c9829-131">Request</span></span>
<span data-ttu-id="c9829-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c9829-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/vppTokens
```

### <a name="response"></a><span data-ttu-id="c9829-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="c9829-133">Response</span></span>
<span data-ttu-id="c9829-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c9829-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1264

{
  "value": [
    {
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
  ]
}
```




