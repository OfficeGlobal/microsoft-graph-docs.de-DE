---
title: AndroidDeviceOwnerEnrollmentProfiles aufListen
description: AufListen von Eigenschaften und Beziehungen der Androiddeviceownerenrollmentprofile hinzugefügt-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b0811979a0a5a28413155916ab8eb797ff57473c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164071"
---
# <a name="list-androiddeviceownerenrollmentprofiles"></a><span data-ttu-id="ef9bf-103">AndroidDeviceOwnerEnrollmentProfiles aufListen</span><span class="sxs-lookup"><span data-stu-id="ef9bf-103">List androidDeviceOwnerEnrollmentProfiles</span></span>

> <span data-ttu-id="ef9bf-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ef9bf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef9bf-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ef9bf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef9bf-106">AufListen von Eigenschaften und Beziehungen der [androiddeviceownerenrollmentprofile hinzugefügt](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="ef9bf-106">List properties and relationships of the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef9bf-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ef9bf-107">Prerequisites</span></span>
<span data-ttu-id="ef9bf-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ef9bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ef9bf-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ef9bf-110">Permission type</span></span>|<span data-ttu-id="ef9bf-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ef9bf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef9bf-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ef9bf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ef9bf-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef9bf-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ef9bf-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ef9bf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef9bf-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ef9bf-115">Not supported.</span></span>|
|<span data-ttu-id="ef9bf-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ef9bf-116">Application</span></span>|<span data-ttu-id="ef9bf-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ef9bf-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef9bf-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ef9bf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="ef9bf-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ef9bf-119">Request headers</span></span>
|<span data-ttu-id="ef9bf-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ef9bf-120">Header</span></span>|<span data-ttu-id="ef9bf-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ef9bf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef9bf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef9bf-122">Authorization</span></span>|<span data-ttu-id="ef9bf-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ef9bf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef9bf-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ef9bf-124">Accept</span></span>|<span data-ttu-id="ef9bf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ef9bf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef9bf-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ef9bf-126">Request body</span></span>
<span data-ttu-id="ef9bf-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ef9bf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef9bf-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="ef9bf-128">Response</span></span>
<span data-ttu-id="ef9bf-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [androiddeviceownerenrollmentprofile hinzugefügt](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ef9bf-129">If successful, this method returns a `200 OK` response code and a collection of [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef9bf-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ef9bf-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef9bf-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ef9bf-131">Request</span></span>
<span data-ttu-id="ef9bf-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ef9bf-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="ef9bf-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="ef9bf-133">Response</span></span>
<span data-ttu-id="ef9bf-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ef9bf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




