---
title: Auflisten von „androidForWorkEnrollmentProfile“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs androidForWorkEnrollmentProfile auf.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2e380beb6587f8d9af4523ef2a51c435a56de332
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402657"
---
# <a name="list-androidforworkenrollmentprofiles"></a><span data-ttu-id="49c44-103">Auflisten von „androidForWorkEnrollmentProfile“</span><span class="sxs-lookup"><span data-stu-id="49c44-103">List androidForWorkEnrollmentProfiles</span></span>

> <span data-ttu-id="49c44-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="49c44-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="49c44-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="49c44-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="49c44-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="49c44-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49c44-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) auf.</span><span class="sxs-lookup"><span data-stu-id="49c44-107">List properties and relationships of the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49c44-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="49c44-108">Prerequisites</span></span>
<span data-ttu-id="49c44-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="49c44-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="49c44-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="49c44-111">Permission type</span></span>|<span data-ttu-id="49c44-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="49c44-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49c44-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="49c44-113">Delegated (work or school account)</span></span>|<span data-ttu-id="49c44-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="49c44-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="49c44-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="49c44-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49c44-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="49c44-116">Not supported.</span></span>|
|<span data-ttu-id="49c44-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="49c44-117">Application</span></span>|<span data-ttu-id="49c44-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="49c44-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="49c44-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="49c44-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="49c44-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="49c44-120">Request headers</span></span>
|<span data-ttu-id="49c44-121">Header</span><span class="sxs-lookup"><span data-stu-id="49c44-121">Header</span></span>|<span data-ttu-id="49c44-122">Wert</span><span class="sxs-lookup"><span data-stu-id="49c44-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49c44-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="49c44-123">Authorization</span></span>|<span data-ttu-id="49c44-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="49c44-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49c44-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="49c44-125">Accept</span></span>|<span data-ttu-id="49c44-126">application/json</span><span class="sxs-lookup"><span data-stu-id="49c44-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49c44-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="49c44-127">Request body</span></span>
<span data-ttu-id="49c44-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="49c44-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49c44-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="49c44-129">Response</span></span>
<span data-ttu-id="49c44-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="49c44-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49c44-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="49c44-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="49c44-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="49c44-132">Request</span></span>
<span data-ttu-id="49c44-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="49c44-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidForWorkEnrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="49c44-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="49c44-134">Response</span></span>
<span data-ttu-id="49c44-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="49c44-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




