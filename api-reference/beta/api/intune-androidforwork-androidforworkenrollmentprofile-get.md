---
title: Abrufen von „androidForWorkEnrollmentProfile“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs androidForWorkEnrollmentProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d59a84f8f5dd7d82c256fba2c7f6bcb0f75d52e7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401789"
---
# <a name="get-androidforworkenrollmentprofile"></a><span data-ttu-id="40ea9-103">Abrufen von „androidForWorkEnrollmentProfile“</span><span class="sxs-lookup"><span data-stu-id="40ea9-103">Get androidForWorkEnrollmentProfile</span></span>

> <span data-ttu-id="40ea9-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="40ea9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="40ea9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="40ea9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="40ea9-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="40ea9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40ea9-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="40ea9-107">Read properties and relationships of the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40ea9-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="40ea9-108">Prerequisites</span></span>
<span data-ttu-id="40ea9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="40ea9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="40ea9-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="40ea9-111">Permission type</span></span>|<span data-ttu-id="40ea9-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="40ea9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40ea9-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="40ea9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="40ea9-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="40ea9-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="40ea9-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="40ea9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40ea9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="40ea9-116">Not supported.</span></span>|
|<span data-ttu-id="40ea9-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="40ea9-117">Application</span></span>|<span data-ttu-id="40ea9-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="40ea9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40ea9-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="40ea9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="40ea9-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="40ea9-120">Optional query parameters</span></span>
<span data-ttu-id="40ea9-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="40ea9-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="40ea9-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="40ea9-122">Request headers</span></span>
|<span data-ttu-id="40ea9-123">Header</span><span class="sxs-lookup"><span data-stu-id="40ea9-123">Header</span></span>|<span data-ttu-id="40ea9-124">Wert</span><span class="sxs-lookup"><span data-stu-id="40ea9-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40ea9-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="40ea9-125">Authorization</span></span>|<span data-ttu-id="40ea9-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="40ea9-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40ea9-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="40ea9-127">Accept</span></span>|<span data-ttu-id="40ea9-128">application/json</span><span class="sxs-lookup"><span data-stu-id="40ea9-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40ea9-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="40ea9-129">Request body</span></span>
<span data-ttu-id="40ea9-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="40ea9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40ea9-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="40ea9-131">Response</span></span>
<span data-ttu-id="40ea9-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="40ea9-132">If successful, this method returns a `200 OK` response code and [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40ea9-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="40ea9-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="40ea9-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="40ea9-134">Request</span></span>
<span data-ttu-id="40ea9-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="40ea9-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

### <a name="response"></a><span data-ttu-id="40ea9-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="40ea9-136">Response</span></span>
<span data-ttu-id="40ea9-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="40ea9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 719

{
  "value": {
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
}
```




