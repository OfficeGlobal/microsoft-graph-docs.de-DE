---
title: Auflisten von „androidForWorkEnrollmentProfile“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs androidForWorkEnrollmentProfile auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0ed7322017a8755d0b95289e550ffa8dd97ff959
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170448"
---
# <a name="list-androidforworkenrollmentprofiles"></a><span data-ttu-id="92b90-103">Auflisten von „androidForWorkEnrollmentProfile“</span><span class="sxs-lookup"><span data-stu-id="92b90-103">List androidForWorkEnrollmentProfiles</span></span>

> <span data-ttu-id="92b90-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="92b90-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92b90-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="92b90-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92b90-106">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) auf.</span><span class="sxs-lookup"><span data-stu-id="92b90-106">List properties and relationships of the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92b90-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="92b90-107">Prerequisites</span></span>
<span data-ttu-id="92b90-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="92b90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="92b90-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="92b90-110">Permission type</span></span>|<span data-ttu-id="92b90-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="92b90-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92b90-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="92b90-112">Delegated (work or school account)</span></span>|<span data-ttu-id="92b90-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="92b90-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="92b90-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="92b90-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92b90-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="92b90-115">Not supported.</span></span>|
|<span data-ttu-id="92b90-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="92b90-116">Application</span></span>|<span data-ttu-id="92b90-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="92b90-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="92b90-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="92b90-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="92b90-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="92b90-119">Request headers</span></span>
|<span data-ttu-id="92b90-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="92b90-120">Header</span></span>|<span data-ttu-id="92b90-121">Wert</span><span class="sxs-lookup"><span data-stu-id="92b90-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92b90-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="92b90-122">Authorization</span></span>|<span data-ttu-id="92b90-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="92b90-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92b90-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="92b90-124">Accept</span></span>|<span data-ttu-id="92b90-125">application/json</span><span class="sxs-lookup"><span data-stu-id="92b90-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92b90-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="92b90-126">Request body</span></span>
<span data-ttu-id="92b90-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="92b90-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92b90-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="92b90-128">Response</span></span>
<span data-ttu-id="92b90-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="92b90-129">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92b90-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="92b90-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="92b90-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="92b90-131">Request</span></span>
<span data-ttu-id="92b90-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="92b90-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidForWorkEnrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="92b90-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="92b90-133">Response</span></span>
<span data-ttu-id="92b90-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="92b90-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 765

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
      "accountId": "Account Id value",
      "id": "e6742553-2553-e674-5325-74e6532574e6",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "tokenValue": "Token Value value",
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




