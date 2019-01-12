---
title: Funktion „downloadApplePushNotificationCertificateSigningRequest“
description: Diese Funktion lädt die Signieranforderung für das Apple Push Notification-Zertifikat herunter.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ffe34e641875a7c059f0c68f4471f17afa0f2cf9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978697"
---
# <a name="downloadapplepushnotificationcertificatesigningrequest-function"></a><span data-ttu-id="5572a-103">Funktion „downloadApplePushNotificationCertificateSigningRequest“</span><span class="sxs-lookup"><span data-stu-id="5572a-103">downloadApplePushNotificationCertificateSigningRequest function</span></span>

> <span data-ttu-id="5572a-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5572a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5572a-105">Diese Funktion lädt die Signieranforderung für das Apple Push Notification-Zertifikat herunter.</span><span class="sxs-lookup"><span data-stu-id="5572a-105">Download Apple push notification certificate signing request</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5572a-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5572a-106">Prerequisites</span></span>
<span data-ttu-id="5572a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5572a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5572a-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5572a-109">Permission type</span></span>|<span data-ttu-id="5572a-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5572a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5572a-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5572a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5572a-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5572a-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5572a-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5572a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5572a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5572a-114">Not supported.</span></span>|
|<span data-ttu-id="5572a-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5572a-115">Application</span></span>|<span data-ttu-id="5572a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5572a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5572a-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5572a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

## <a name="request-headers"></a><span data-ttu-id="5572a-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5572a-118">Request headers</span></span>
|<span data-ttu-id="5572a-119">Header</span><span class="sxs-lookup"><span data-stu-id="5572a-119">Header</span></span>|<span data-ttu-id="5572a-120">Wert</span><span class="sxs-lookup"><span data-stu-id="5572a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5572a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5572a-121">Authorization</span></span>|<span data-ttu-id="5572a-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5572a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5572a-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5572a-123">Accept</span></span>|<span data-ttu-id="5572a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5572a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5572a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5572a-125">Request body</span></span>
<span data-ttu-id="5572a-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5572a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5572a-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="5572a-127">Response</span></span>
<span data-ttu-id="5572a-128">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `200 OK` und ein Objekt des Typs „String“ im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5572a-128">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5572a-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5572a-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="5572a-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5572a-130">Request</span></span>
<span data-ttu-id="5572a-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5572a-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

### <a name="response"></a><span data-ttu-id="5572a-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="5572a-132">Response</span></span>
<span data-ttu-id="5572a-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5572a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 85

{
  "value": "Download Apple Push Notification Certificate Signing Request value"
}
```



