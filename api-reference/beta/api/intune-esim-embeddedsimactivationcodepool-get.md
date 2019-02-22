---
title: EmbeddedSIMActivationCodePool abrufen
description: Lesen von Eigenschaften und Beziehungen des embeddedSIMActivationCodePool-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 23279b5c35e929bca76b97588342cdb2eac68126
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141650"
---
# <a name="get-embeddedsimactivationcodepool"></a><span data-ttu-id="a1e61-103">EmbeddedSIMActivationCodePool abrufen</span><span class="sxs-lookup"><span data-stu-id="a1e61-103">Get embeddedSIMActivationCodePool</span></span>

> <span data-ttu-id="a1e61-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a1e61-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1e61-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a1e61-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1e61-106">Lesen von Eigenschaften und Beziehungen des [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="a1e61-106">Read properties and relationships of the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1e61-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a1e61-107">Prerequisites</span></span>
<span data-ttu-id="a1e61-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a1e61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a1e61-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a1e61-110">Permission type</span></span>|<span data-ttu-id="a1e61-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a1e61-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1e61-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a1e61-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a1e61-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1e61-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a1e61-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a1e61-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1e61-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a1e61-115">Not supported.</span></span>|
|<span data-ttu-id="a1e61-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a1e61-116">Application</span></span>|<span data-ttu-id="a1e61-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a1e61-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1e61-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a1e61-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a1e61-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a1e61-119">Optional query parameters</span></span>
<span data-ttu-id="a1e61-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a1e61-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a1e61-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a1e61-121">Request headers</span></span>
|<span data-ttu-id="a1e61-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a1e61-122">Header</span></span>|<span data-ttu-id="a1e61-123">Wert</span><span class="sxs-lookup"><span data-stu-id="a1e61-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1e61-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1e61-124">Authorization</span></span>|<span data-ttu-id="a1e61-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a1e61-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1e61-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a1e61-126">Accept</span></span>|<span data-ttu-id="a1e61-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a1e61-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1e61-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a1e61-128">Request body</span></span>
<span data-ttu-id="a1e61-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a1e61-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1e61-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="a1e61-130">Response</span></span>
<span data-ttu-id="a1e61-131">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a1e61-131">If successful, this method returns a `200 OK` response code and [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1e61-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a1e61-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1e61-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a1e61-133">Request</span></span>
<span data-ttu-id="a1e61-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a1e61-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
```

### <a name="response"></a><span data-ttu-id="a1e61-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="a1e61-135">Response</span></span>
<span data-ttu-id="a1e61-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a1e61-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 675

{
  "value": {
    "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
    "id": "ec308741-8741-ec30-4187-30ec418730ec",
    "displayName": "Display Name value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
    "activationCodes": [
      {
        "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
        "integratedCircuitCardIdentifier": "Integrated Circuit Card Identifier value",
        "matchingIdentifier": "Matching Identifier value",
        "smdpPlusServerAddress": "Smdp Plus Server Address value"
      }
    ],
    "activationCodeCount": 3
  }
}
```




