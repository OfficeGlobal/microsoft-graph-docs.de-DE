---
title: localizedNotificationMessage erstellen
description: Erstellen eines neuen localizedNotificationMessage-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cd9b2568ccf80d2000271d597baf0a6ace6bf9ca
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968064"
---
# <a name="create-localizednotificationmessage"></a><span data-ttu-id="b3e45-103">localizedNotificationMessage erstellen</span><span class="sxs-lookup"><span data-stu-id="b3e45-103">Create localizedNotificationMessage</span></span>

> <span data-ttu-id="b3e45-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b3e45-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3e45-105">Erstellen eines neuen [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b3e45-105">Create a new [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b3e45-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b3e45-106">Prerequisites</span></span>
<span data-ttu-id="b3e45-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3e45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3e45-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b3e45-109">Permission type</span></span>|<span data-ttu-id="b3e45-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b3e45-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3e45-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b3e45-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b3e45-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3e45-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b3e45-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b3e45-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3e45-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b3e45-114">Not supported.</span></span>|
|<span data-ttu-id="b3e45-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b3e45-115">Application</span></span>|<span data-ttu-id="b3e45-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b3e45-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3e45-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b3e45-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="b3e45-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b3e45-118">Request headers</span></span>
|<span data-ttu-id="b3e45-119">Header</span><span class="sxs-lookup"><span data-stu-id="b3e45-119">Header</span></span>|<span data-ttu-id="b3e45-120">Wert</span><span class="sxs-lookup"><span data-stu-id="b3e45-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3e45-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3e45-121">Authorization</span></span>|<span data-ttu-id="b3e45-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b3e45-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3e45-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b3e45-123">Accept</span></span>|<span data-ttu-id="b3e45-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b3e45-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3e45-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b3e45-125">Request body</span></span>
<span data-ttu-id="b3e45-126">Geben Sie im Anforderungstext eine JSON Darstellung für das localizedNotificationMessage-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="b3e45-126">In the request body, supply a JSON representation for the localizedNotificationMessage object.</span></span>

<span data-ttu-id="b3e45-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der localizedNotificationMessage erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b3e45-127">The following table shows the properties that are required when you create the localizedNotificationMessage.</span></span>

|<span data-ttu-id="b3e45-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b3e45-128">Property</span></span>|<span data-ttu-id="b3e45-129">Typ</span><span class="sxs-lookup"><span data-stu-id="b3e45-129">Type</span></span>|<span data-ttu-id="b3e45-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b3e45-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3e45-131">id</span><span class="sxs-lookup"><span data-stu-id="b3e45-131">id</span></span>|<span data-ttu-id="b3e45-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b3e45-132">String</span></span>|<span data-ttu-id="b3e45-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b3e45-133">Key of the entity.</span></span>|
|<span data-ttu-id="b3e45-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3e45-134">lastModifiedDateTime</span></span>|<span data-ttu-id="b3e45-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3e45-135">DateTimeOffset</span></span>|<span data-ttu-id="b3e45-136">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b3e45-136">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="b3e45-137">Gebietsschema</span><span class="sxs-lookup"><span data-stu-id="b3e45-137">locale</span></span>|<span data-ttu-id="b3e45-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b3e45-138">String</span></span>|<span data-ttu-id="b3e45-139">Das Gebietsschema für das diese Nachricht bestimmt ist.</span><span class="sxs-lookup"><span data-stu-id="b3e45-139">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="b3e45-140">Betreff</span><span class="sxs-lookup"><span data-stu-id="b3e45-140">subject</span></span>|<span data-ttu-id="b3e45-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b3e45-141">String</span></span>|<span data-ttu-id="b3e45-142">Die Vorlage für den Betreff der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="b3e45-142">The Message Template Subject.</span></span>|
|<span data-ttu-id="b3e45-143">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="b3e45-143">messageTemplate</span></span>|<span data-ttu-id="b3e45-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b3e45-144">String</span></span>|<span data-ttu-id="b3e45-145">Die Vorlage für den Inhalt der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="b3e45-145">The Message Template content.</span></span>|
|<span data-ttu-id="b3e45-146">isDefault</span><span class="sxs-lookup"><span data-stu-id="b3e45-146">isDefault</span></span>|<span data-ttu-id="b3e45-147">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b3e45-147">Boolean</span></span>|<span data-ttu-id="b3e45-148">Die Kennzeichnung gibt an, ob dies das Standard-Gebietsschema für die Fallbacksprache ist.</span><span class="sxs-lookup"><span data-stu-id="b3e45-148">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="b3e45-149">Dieser Kennzeichnung kann nur festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="b3e45-149">This flag can only be set.</span></span> <span data-ttu-id="b3e45-150">Um die Festlegung aufzuheben, setzen Sie diese Eigenschaft bei einer anderen lokalisierten Benachrichtigung auf „true“.</span><span class="sxs-lookup"><span data-stu-id="b3e45-150">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="b3e45-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="b3e45-151">Response</span></span>
<span data-ttu-id="b3e45-152">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b3e45-152">If successful, this method returns a `201 Created` response code and a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3e45-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b3e45-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="b3e45-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b3e45-154">Request</span></span>
<span data-ttu-id="b3e45-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b3e45-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
Content-type: application/json
Content-length: 200

{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "locale": "Locale value",
  "subject": "Subject value",
  "messageTemplate": "Message Template value",
  "isDefault": true
}
```

### <a name="response"></a><span data-ttu-id="b3e45-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="b3e45-156">Response</span></span>
<span data-ttu-id="b3e45-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b3e45-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 313

{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "id": "7a777708-7708-7a77-0877-777a0877777a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "locale": "Locale value",
  "subject": "Subject value",
  "messageTemplate": "Message Template value",
  "isDefault": true
}
```



