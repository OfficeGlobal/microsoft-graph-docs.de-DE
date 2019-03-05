---
title: Auflisten von „localizedNotificationMessage“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs localizedNotificationMessage auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 563b324eca95f5b5b26eaeb00d192467055cb13b
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252231"
---
# <a name="list-localizednotificationmessages"></a><span data-ttu-id="b59c9-103">Auflisten von „localizedNotificationMessage“</span><span class="sxs-lookup"><span data-stu-id="b59c9-103">List localizedNotificationMessages</span></span>

> <span data-ttu-id="b59c9-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b59c9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b59c9-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) auf.</span><span class="sxs-lookup"><span data-stu-id="b59c9-105">List properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b59c9-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b59c9-106">Prerequisites</span></span>
<span data-ttu-id="b59c9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b59c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b59c9-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b59c9-109">Permission type</span></span>|<span data-ttu-id="b59c9-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b59c9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b59c9-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b59c9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b59c9-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b59c9-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b59c9-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b59c9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b59c9-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b59c9-114">Not supported.</span></span>|
|<span data-ttu-id="b59c9-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b59c9-115">Application</span></span>|<span data-ttu-id="b59c9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b59c9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b59c9-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b59c9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="b59c9-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b59c9-118">Request headers</span></span>
|<span data-ttu-id="b59c9-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b59c9-119">Header</span></span>|<span data-ttu-id="b59c9-120">Wert</span><span class="sxs-lookup"><span data-stu-id="b59c9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b59c9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b59c9-121">Authorization</span></span>|<span data-ttu-id="b59c9-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b59c9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b59c9-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b59c9-123">Accept</span></span>|<span data-ttu-id="b59c9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b59c9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b59c9-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b59c9-125">Request body</span></span>
<span data-ttu-id="b59c9-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b59c9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b59c9-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="b59c9-127">Response</span></span>
<span data-ttu-id="b59c9-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b59c9-128">If successful, this method returns a `200 OK` response code and a collection of [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b59c9-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b59c9-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="b59c9-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b59c9-130">Request</span></span>
<span data-ttu-id="b59c9-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b59c9-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

### <a name="response"></a><span data-ttu-id="b59c9-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="b59c9-132">Response</span></span>
<span data-ttu-id="b59c9-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b59c9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 374

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.localizedNotificationMessage",
      "id": "7a777708-7708-7a77-0877-777a0877777a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "locale": "Locale value",
      "subject": "Subject value",
      "messageTemplate": "Message Template value",
      "isDefault": true
    }
  ]
}
```



