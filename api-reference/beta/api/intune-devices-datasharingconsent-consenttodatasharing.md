---
title: ConsentToDataSharing Aktion
description: Noch nicht dokumentiert
ms.openlocfilehash: dfd5cd5c536b25c82588f5895c11135f574a5c59
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065693"
---
# <a name="consenttodatasharing-action"></a><span data-ttu-id="7f4ec-103">ConsentToDataSharing Aktion</span><span class="sxs-lookup"><span data-stu-id="7f4ec-103">consentToDataSharing action</span></span>

> <span data-ttu-id="7f4ec-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7f4ec-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f4ec-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7f4ec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7f4ec-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7f4ec-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7f4ec-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="7f4ec-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7f4ec-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7f4ec-108">Prerequisites</span></span>
<span data-ttu-id="7f4ec-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f4ec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f4ec-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7f4ec-111">Permission type</span></span>|<span data-ttu-id="7f4ec-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7f4ec-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f4ec-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7f4ec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7f4ec-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f4ec-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7f4ec-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7f4ec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f4ec-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7f4ec-116">Not supported.</span></span>|
|<span data-ttu-id="7f4ec-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7f4ec-117">Application</span></span>|<span data-ttu-id="7f4ec-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7f4ec-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f4ec-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7f4ec-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/dataSharingConsents/{dataSharingConsentId}/consentToDataSharing
```

## <a name="request-headers"></a><span data-ttu-id="7f4ec-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7f4ec-120">Request headers</span></span>
|<span data-ttu-id="7f4ec-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7f4ec-121">Header</span></span>|<span data-ttu-id="7f4ec-122">Wert</span><span class="sxs-lookup"><span data-stu-id="7f4ec-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f4ec-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f4ec-123">Authorization</span></span>|<span data-ttu-id="7f4ec-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7f4ec-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f4ec-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7f4ec-125">Accept</span></span>|<span data-ttu-id="7f4ec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7f4ec-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f4ec-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7f4ec-127">Request body</span></span>
<span data-ttu-id="7f4ec-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7f4ec-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f4ec-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="7f4ec-129">Response</span></span>
<span data-ttu-id="7f4ec-130">Wenn erfolgreich ist, diese Aktion gibt eine `200 OK` Antwortcode und eine [DataSharingConsent](../resources/intune-devices-datasharingconsent.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="7f4ec-130">If successful, this action returns a `200 OK` response code and a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f4ec-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7f4ec-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="7f4ec-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7f4ec-132">Request</span></span>
<span data-ttu-id="7f4ec-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7f4ec-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents/{dataSharingConsentId}/consentToDataSharing
```

### <a name="response"></a><span data-ttu-id="7f4ec-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="7f4ec-134">Response</span></span>
<span data-ttu-id="7f4ec-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7f4ec-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





