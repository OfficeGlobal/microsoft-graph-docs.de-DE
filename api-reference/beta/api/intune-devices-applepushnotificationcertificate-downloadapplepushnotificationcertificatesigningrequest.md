---
title: Funktion „downloadApplePushNotificationCertificateSigningRequest“
description: Diese Funktion lädt die Signieranforderung für das Apple Push Notification-Zertifikat herunter.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 94126d7372497abfc2318ad5029eab27b64d0087
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953646"
---
# <a name="downloadapplepushnotificationcertificatesigningrequest-function"></a><span data-ttu-id="21551-103">Funktion „downloadApplePushNotificationCertificateSigningRequest“</span><span class="sxs-lookup"><span data-stu-id="21551-103">downloadApplePushNotificationCertificateSigningRequest function</span></span>

> <span data-ttu-id="21551-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="21551-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="21551-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="21551-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="21551-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="21551-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21551-107">Diese Funktion lädt die Signieranforderung für das Apple Push Notification-Zertifikat herunter.</span><span class="sxs-lookup"><span data-stu-id="21551-107">Download Apple push notification certificate signing request</span></span>
## <a name="prerequisites"></a><span data-ttu-id="21551-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="21551-108">Prerequisites</span></span>
<span data-ttu-id="21551-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21551-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21551-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="21551-111">Permission type</span></span>|<span data-ttu-id="21551-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="21551-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21551-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="21551-113">Delegated (work or school account)</span></span>|<span data-ttu-id="21551-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21551-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="21551-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="21551-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21551-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="21551-116">Not supported.</span></span>|
|<span data-ttu-id="21551-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="21551-117">Application</span></span>|<span data-ttu-id="21551-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="21551-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21551-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="21551-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

## <a name="request-headers"></a><span data-ttu-id="21551-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="21551-120">Request headers</span></span>
|<span data-ttu-id="21551-121">Header</span><span class="sxs-lookup"><span data-stu-id="21551-121">Header</span></span>|<span data-ttu-id="21551-122">Wert</span><span class="sxs-lookup"><span data-stu-id="21551-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21551-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="21551-123">Authorization</span></span>|<span data-ttu-id="21551-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="21551-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21551-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="21551-125">Accept</span></span>|<span data-ttu-id="21551-126">application/json</span><span class="sxs-lookup"><span data-stu-id="21551-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21551-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="21551-127">Request body</span></span>
<span data-ttu-id="21551-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="21551-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21551-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="21551-129">Response</span></span>
<span data-ttu-id="21551-130">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `200 OK` und ein Objekt des Typs „String“ im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="21551-130">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21551-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="21551-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="21551-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="21551-132">Request</span></span>
<span data-ttu-id="21551-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="21551-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate/downloadApplePushNotificationCertificateSigningRequest
```

### <a name="response"></a><span data-ttu-id="21551-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="21551-134">Response</span></span>
<span data-ttu-id="21551-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="21551-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 85

{
  "value": "Download Apple Push Notification Certificate Signing Request value"
}
```





