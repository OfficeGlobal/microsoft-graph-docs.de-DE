---
title: localizedNotificationMessage löschen
description: Löschen einer localizedNotificationMessage.
ms.openlocfilehash: a601930455318e08eeeb978b8fc8958a9e6375bd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059324"
---
# <a name="delete-localizednotificationmessage"></a><span data-ttu-id="e4820-103">localizedNotificationMessage löschen</span><span class="sxs-lookup"><span data-stu-id="e4820-103">Delete localizedNotificationMessage</span></span>

> <span data-ttu-id="e4820-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e4820-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4820-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e4820-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e4820-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e4820-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e4820-107">Löschen einer [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="e4820-107">Deletes a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e4820-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e4820-108">Prerequisites</span></span>
<span data-ttu-id="e4820-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4820-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4820-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e4820-111">Permission type</span></span>|<span data-ttu-id="e4820-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e4820-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4820-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e4820-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e4820-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4820-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e4820-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e4820-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4820-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e4820-116">Not supported.</span></span>|
|<span data-ttu-id="e4820-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e4820-117">Application</span></span>|<span data-ttu-id="e4820-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e4820-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4820-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e4820-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="e4820-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e4820-120">Request headers</span></span>
|<span data-ttu-id="e4820-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e4820-121">Header</span></span>|<span data-ttu-id="e4820-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e4820-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4820-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4820-123">Authorization</span></span>|<span data-ttu-id="e4820-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e4820-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4820-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e4820-125">Accept</span></span>|<span data-ttu-id="e4820-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e4820-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4820-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e4820-127">Request body</span></span>
<span data-ttu-id="e4820-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e4820-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4820-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="e4820-129">Response</span></span>
<span data-ttu-id="e4820-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e4820-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e4820-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e4820-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="e4820-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e4820-132">Request</span></span>
<span data-ttu-id="e4820-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e4820-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

### <a name="response"></a><span data-ttu-id="e4820-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="e4820-134">Response</span></span>
<span data-ttu-id="e4820-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e4820-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





