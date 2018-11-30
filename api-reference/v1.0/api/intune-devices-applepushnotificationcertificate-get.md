---
title: Abrufen von „applePushNotificationCertificate“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs applePushNotificationCertificate.
ms.openlocfilehash: eabab534b812cd35eb4652c530b08120b699c330
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018030"
---
# <a name="get-applepushnotificationcertificate"></a><span data-ttu-id="b9ace-103">Abrufen von „applePushNotificationCertificate“</span><span class="sxs-lookup"><span data-stu-id="b9ace-103">Get applePushNotificationCertificate</span></span>

> <span data-ttu-id="b9ace-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b9ace-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b9ace-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="b9ace-105">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b9ace-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b9ace-106">Prerequisites</span></span>
<span data-ttu-id="b9ace-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9ace-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9ace-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b9ace-109">Permission type</span></span>|<span data-ttu-id="b9ace-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b9ace-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9ace-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b9ace-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b9ace-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9ace-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="b9ace-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b9ace-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9ace-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b9ace-114">Not supported.</span></span>|
|<span data-ttu-id="b9ace-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b9ace-115">Application</span></span>|<span data-ttu-id="b9ace-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b9ace-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9ace-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9ace-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/applePushNotificationCertificate
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b9ace-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b9ace-118">Optional query parameters</span></span>
<span data-ttu-id="b9ace-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b9ace-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b9ace-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b9ace-120">Request headers</span></span>
|<span data-ttu-id="b9ace-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b9ace-121">Header</span></span>|<span data-ttu-id="b9ace-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b9ace-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9ace-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9ace-123">Authorization</span></span>|<span data-ttu-id="b9ace-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b9ace-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9ace-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b9ace-125">Accept</span></span>|<span data-ttu-id="b9ace-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b9ace-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9ace-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b9ace-127">Request body</span></span>
<span data-ttu-id="b9ace-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b9ace-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9ace-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9ace-129">Response</span></span>
<span data-ttu-id="b9ace-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b9ace-130">If successful, this method returns a `200 OK` response code and [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9ace-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b9ace-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b9ace-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9ace-132">Request</span></span>
<span data-ttu-id="b9ace-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b9ace-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/applePushNotificationCertificate
```

### <a name="response"></a><span data-ttu-id="b9ace-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9ace-134">Response</span></span>
<span data-ttu-id="b9ace-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b9ace-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 417

{
  "value": {
    "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
    "id": "c4c8f047-f047-c4c8-47f0-c8c447f0c8c4",
    "appleIdentifier": "Apple Identifier value",
    "topicIdentifier": "Topic Identifier value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "certificate": "Certificate value"
  }
}
```


