---
title: Abrufen von „localizedNotificationMessage“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs localizedNotificationMessage.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7f9a02823fefa3087a8e9e32d093900a2da63fc1
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30977023"
---
# <a name="get-localizednotificationmessage"></a><span data-ttu-id="6c9fc-103">Abrufen von „localizedNotificationMessage“</span><span class="sxs-lookup"><span data-stu-id="6c9fc-103">Get localizedNotificationMessage</span></span>

> <span data-ttu-id="6c9fc-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6c9fc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c9fc-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6c9fc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c9fc-106">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="6c9fc-106">Read properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c9fc-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6c9fc-107">Prerequisites</span></span>
<span data-ttu-id="6c9fc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c9fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c9fc-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6c9fc-110">Permission type</span></span>|<span data-ttu-id="6c9fc-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6c9fc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c9fc-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6c9fc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6c9fc-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c9fc-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="6c9fc-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6c9fc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c9fc-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6c9fc-115">Not supported.</span></span>|
|<span data-ttu-id="6c9fc-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6c9fc-116">Application</span></span>|<span data-ttu-id="6c9fc-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6c9fc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c9fc-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6c9fc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6c9fc-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6c9fc-119">Optional query parameters</span></span>
<span data-ttu-id="6c9fc-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6c9fc-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6c9fc-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6c9fc-121">Request headers</span></span>
|<span data-ttu-id="6c9fc-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6c9fc-122">Header</span></span>|<span data-ttu-id="6c9fc-123">Wert</span><span class="sxs-lookup"><span data-stu-id="6c9fc-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c9fc-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c9fc-124">Authorization</span></span>|<span data-ttu-id="6c9fc-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6c9fc-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c9fc-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6c9fc-126">Accept</span></span>|<span data-ttu-id="6c9fc-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6c9fc-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c9fc-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6c9fc-128">Request body</span></span>
<span data-ttu-id="6c9fc-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6c9fc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c9fc-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="6c9fc-130">Response</span></span>
<span data-ttu-id="6c9fc-131">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6c9fc-131">If successful, this method returns a `200 OK` response code and [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c9fc-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6c9fc-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c9fc-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6c9fc-133">Request</span></span>
<span data-ttu-id="6c9fc-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6c9fc-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

### <a name="response"></a><span data-ttu-id="6c9fc-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="6c9fc-135">Response</span></span>
<span data-ttu-id="6c9fc-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6c9fc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "value": {
    "@odata.type": "#microsoft.graph.localizedNotificationMessage",
    "id": "7a777708-7708-7a77-0877-777a0877777a",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "locale": "Locale value",
    "subject": "Subject value",
    "messageTemplate": "Message Template value",
    "isDefault": true
  }
}
```




