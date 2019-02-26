---
title: localizedNotificationMessage löschen
description: Löschen einer localizedNotificationMessage.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d0a9a7b6cd795fa3e989a27539640e05a7ad909f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263098"
---
# <a name="delete-localizednotificationmessage"></a><span data-ttu-id="e6479-103">localizedNotificationMessage löschen</span><span class="sxs-lookup"><span data-stu-id="e6479-103">Delete localizedNotificationMessage</span></span>

> <span data-ttu-id="e6479-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e6479-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6479-105">Löschen einer [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="e6479-105">Deletes a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6479-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e6479-106">Prerequisites</span></span>
<span data-ttu-id="e6479-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e6479-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e6479-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e6479-109">Permission type</span></span>|<span data-ttu-id="e6479-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e6479-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6479-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e6479-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e6479-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6479-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e6479-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e6479-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6479-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e6479-114">Not supported.</span></span>|
|<span data-ttu-id="e6479-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e6479-115">Application</span></span>|<span data-ttu-id="e6479-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e6479-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6479-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e6479-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="e6479-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e6479-118">Request headers</span></span>
|<span data-ttu-id="e6479-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e6479-119">Header</span></span>|<span data-ttu-id="e6479-120">Wert</span><span class="sxs-lookup"><span data-stu-id="e6479-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6479-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6479-121">Authorization</span></span>|<span data-ttu-id="e6479-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e6479-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6479-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e6479-123">Accept</span></span>|<span data-ttu-id="e6479-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e6479-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6479-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e6479-125">Request body</span></span>
<span data-ttu-id="e6479-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e6479-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6479-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="e6479-127">Response</span></span>
<span data-ttu-id="e6479-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e6479-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e6479-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e6479-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6479-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e6479-130">Request</span></span>
<span data-ttu-id="e6479-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e6479-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

### <a name="response"></a><span data-ttu-id="e6479-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="e6479-132">Response</span></span>
<span data-ttu-id="e6479-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e6479-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



