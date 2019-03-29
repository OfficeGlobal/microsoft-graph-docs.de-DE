---
title: Auflisten von „localizedNotificationMessage“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs localizedNotificationMessage auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: be8bf0b1a24dc62472e8449e8b93476b7fe74e15
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30965550"
---
# <a name="list-localizednotificationmessages"></a><span data-ttu-id="80bae-103">Auflisten von „localizedNotificationMessage“</span><span class="sxs-lookup"><span data-stu-id="80bae-103">List localizedNotificationMessages</span></span>

> <span data-ttu-id="80bae-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="80bae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="80bae-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="80bae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80bae-106">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) auf.</span><span class="sxs-lookup"><span data-stu-id="80bae-106">List properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80bae-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="80bae-107">Prerequisites</span></span>
<span data-ttu-id="80bae-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80bae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80bae-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="80bae-110">Permission type</span></span>|<span data-ttu-id="80bae-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="80bae-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80bae-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="80bae-112">Delegated (work or school account)</span></span>|<span data-ttu-id="80bae-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="80bae-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="80bae-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="80bae-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80bae-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="80bae-115">Not supported.</span></span>|
|<span data-ttu-id="80bae-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="80bae-116">Application</span></span>|<span data-ttu-id="80bae-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="80bae-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80bae-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="80bae-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="80bae-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="80bae-119">Request headers</span></span>
|<span data-ttu-id="80bae-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="80bae-120">Header</span></span>|<span data-ttu-id="80bae-121">Wert</span><span class="sxs-lookup"><span data-stu-id="80bae-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80bae-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="80bae-122">Authorization</span></span>|<span data-ttu-id="80bae-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="80bae-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80bae-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="80bae-124">Accept</span></span>|<span data-ttu-id="80bae-125">application/json</span><span class="sxs-lookup"><span data-stu-id="80bae-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80bae-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="80bae-126">Request body</span></span>
<span data-ttu-id="80bae-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="80bae-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80bae-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="80bae-128">Response</span></span>
<span data-ttu-id="80bae-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="80bae-129">If successful, this method returns a `200 OK` response code and a collection of [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80bae-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="80bae-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="80bae-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="80bae-131">Request</span></span>
<span data-ttu-id="80bae-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="80bae-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

### <a name="response"></a><span data-ttu-id="80bae-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="80bae-133">Response</span></span>
<span data-ttu-id="80bae-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="80bae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




