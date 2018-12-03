---
title: Liste androidDeviceOwnerEnrollmentProfiles
description: Listeneigenschaften und Beziehungen der AndroidDeviceOwnerEnrollmentProfile-Objekte.
ms.openlocfilehash: cba0ec4d450e866eaf849536f905dfdc3e00a20c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061891"
---
# <a name="list-androiddeviceownerenrollmentprofiles"></a><span data-ttu-id="3e232-103">Liste androidDeviceOwnerEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="3e232-103">List androidDeviceOwnerEnrollmentProfiles</span></span>

> <span data-ttu-id="3e232-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3e232-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e232-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3e232-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3e232-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3e232-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3e232-107">Listeneigenschaften und Beziehungen der [AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="3e232-107">List properties and relationships of the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3e232-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3e232-108">Prerequisites</span></span>
<span data-ttu-id="3e232-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e232-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e232-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3e232-111">Permission type</span></span>|<span data-ttu-id="3e232-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3e232-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e232-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3e232-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3e232-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3e232-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3e232-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3e232-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e232-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3e232-116">Not supported.</span></span>|
|<span data-ttu-id="3e232-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3e232-117">Application</span></span>|<span data-ttu-id="3e232-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3e232-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e232-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e232-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="3e232-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3e232-120">Request headers</span></span>
|<span data-ttu-id="3e232-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3e232-121">Header</span></span>|<span data-ttu-id="3e232-122">Wert</span><span class="sxs-lookup"><span data-stu-id="3e232-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e232-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e232-123">Authorization</span></span>|<span data-ttu-id="3e232-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3e232-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e232-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3e232-125">Accept</span></span>|<span data-ttu-id="3e232-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3e232-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e232-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3e232-127">Request body</span></span>
<span data-ttu-id="3e232-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3e232-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e232-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e232-129">Response</span></span>
<span data-ttu-id="3e232-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="3e232-130">If successful, this method returns a `200 OK` response code and a collection of [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e232-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3e232-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="3e232-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e232-132">Request</span></span>
<span data-ttu-id="3e232-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3e232-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="3e232-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e232-134">Response</span></span>
<span data-ttu-id="3e232-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3e232-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





