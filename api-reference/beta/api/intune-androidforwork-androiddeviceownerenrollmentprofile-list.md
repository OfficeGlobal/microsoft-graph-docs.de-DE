---
title: Liste androidDeviceOwnerEnrollmentProfiles
description: Listeneigenschaften und Beziehungen der AndroidDeviceOwnerEnrollmentProfile-Objekte.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 79fb004fc57444f77c3110316516cb5ecec7ba31
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883160"
---
# <a name="list-androiddeviceownerenrollmentprofiles"></a><span data-ttu-id="155c2-103">Liste androidDeviceOwnerEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="155c2-103">List androidDeviceOwnerEnrollmentProfiles</span></span>

> <span data-ttu-id="155c2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="155c2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="155c2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="155c2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="155c2-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="155c2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="155c2-107">Listeneigenschaften und Beziehungen der [AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="155c2-107">List properties and relationships of the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="155c2-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="155c2-108">Prerequisites</span></span>
<span data-ttu-id="155c2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="155c2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="155c2-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="155c2-111">Permission type</span></span>|<span data-ttu-id="155c2-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="155c2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="155c2-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="155c2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="155c2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="155c2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="155c2-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="155c2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="155c2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="155c2-116">Not supported.</span></span>|
|<span data-ttu-id="155c2-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="155c2-117">Application</span></span>|<span data-ttu-id="155c2-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="155c2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="155c2-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="155c2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="155c2-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="155c2-120">Request headers</span></span>
|<span data-ttu-id="155c2-121">Header</span><span class="sxs-lookup"><span data-stu-id="155c2-121">Header</span></span>|<span data-ttu-id="155c2-122">Wert</span><span class="sxs-lookup"><span data-stu-id="155c2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="155c2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="155c2-123">Authorization</span></span>|<span data-ttu-id="155c2-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="155c2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="155c2-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="155c2-125">Accept</span></span>|<span data-ttu-id="155c2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="155c2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="155c2-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="155c2-127">Request body</span></span>
<span data-ttu-id="155c2-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="155c2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="155c2-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="155c2-129">Response</span></span>
<span data-ttu-id="155c2-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="155c2-130">If successful, this method returns a `200 OK` response code and a collection of [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="155c2-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="155c2-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="155c2-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="155c2-132">Request</span></span>
<span data-ttu-id="155c2-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="155c2-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="155c2-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="155c2-134">Response</span></span>
<span data-ttu-id="155c2-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="155c2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 838

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
      "accountId": "Account Id value",
      "id": "a8d0245e-245e-a8d0-5e24-d0a85e24d0a8",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "tokenValue": "Token Value value",
      "tokenCreationDateTime": "2017-01-01T00:01:38.5314127-08:00",
      "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
      "enrolledDeviceCount": 3,
      "qrCodeContent": "Qr Code Content value",
      "qrCodeImage": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      }
    }
  ]
}
```





