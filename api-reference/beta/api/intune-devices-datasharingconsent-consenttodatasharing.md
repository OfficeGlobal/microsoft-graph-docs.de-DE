---
title: consentToDataSharing-Aktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a4fae52a9bcffa7ed500df63c2350f121a196626
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161019"
---
# <a name="consenttodatasharing-action"></a><span data-ttu-id="cb913-103">consentToDataSharing-Aktion</span><span class="sxs-lookup"><span data-stu-id="cb913-103">consentToDataSharing action</span></span>

> <span data-ttu-id="cb913-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cb913-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb913-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="cb913-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb913-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="cb913-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb913-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cb913-107">Prerequisites</span></span>
<span data-ttu-id="cb913-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="cb913-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cb913-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cb913-110">Permission type</span></span>|<span data-ttu-id="cb913-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cb913-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb913-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cb913-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cb913-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb913-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cb913-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cb913-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb913-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cb913-115">Not supported.</span></span>|
|<span data-ttu-id="cb913-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cb913-116">Application</span></span>|<span data-ttu-id="cb913-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cb913-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb913-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cb913-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/dataSharingConsents/{dataSharingConsentId}/consentToDataSharing
```

## <a name="request-headers"></a><span data-ttu-id="cb913-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cb913-119">Request headers</span></span>
|<span data-ttu-id="cb913-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="cb913-120">Header</span></span>|<span data-ttu-id="cb913-121">Wert</span><span class="sxs-lookup"><span data-stu-id="cb913-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb913-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb913-122">Authorization</span></span>|<span data-ttu-id="cb913-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cb913-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb913-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="cb913-124">Accept</span></span>|<span data-ttu-id="cb913-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cb913-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb913-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cb913-126">Request body</span></span>
<span data-ttu-id="cb913-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cb913-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb913-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="cb913-128">Response</span></span>
<span data-ttu-id="cb913-129">Bei erfolgreicher Ausführung gibt die Aktion den `200 OK` Antwortcode und eine [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="cb913-129">If successful, this action returns a `200 OK` response code and a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb913-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cb913-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb913-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cb913-131">Request</span></span>
<span data-ttu-id="cb913-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cb913-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents/{dataSharingConsentId}/consentToDataSharing
```

### <a name="response"></a><span data-ttu-id="cb913-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="cb913-133">Response</span></span>
<span data-ttu-id="cb913-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cb913-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 417

{
  "value": {
    "@odata.type": "#microsoft.graph.dataSharingConsent",
    "id": "333387f7-87f7-3333-f787-3333f7873333",
    "serviceDisplayName": "Service Display Name value",
    "termsUrl": "https://example.com/termsUrl/",
    "granted": true,
    "grantDateTime": "2016-12-31T23:59:55.7154191-08:00",
    "grantedByUpn": "Granted By Upn value",
    "grantedByUserId": "Granted By User Id value"
  }
}
```




