---
title: localizedNotificationMessage aktualisieren
description: Aktualisieren der Eigenschaften eines LocalizedNotificationMessage-Objekts.
ms.openlocfilehash: a3dfc54c0bdd65004e98dfc942e58e24ef7238f9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016825"
---
# <a name="update-localizednotificationmessage"></a><span data-ttu-id="8f9de-103">localizedNotificationMessage aktualisieren</span><span class="sxs-lookup"><span data-stu-id="8f9de-103">Update localizedNotificationMessage</span></span>

> <span data-ttu-id="8f9de-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8f9de-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8f9de-105">Aktualisieren der Eigenschaften eines [LocalizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8f9de-105">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8f9de-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8f9de-106">Prerequisites</span></span>
<span data-ttu-id="8f9de-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f9de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f9de-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8f9de-109">Permission type</span></span>|<span data-ttu-id="8f9de-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8f9de-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f9de-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8f9de-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8f9de-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f9de-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8f9de-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8f9de-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f9de-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8f9de-114">Not supported.</span></span>|
|<span data-ttu-id="8f9de-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8f9de-115">Application</span></span>|<span data-ttu-id="8f9de-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8f9de-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f9de-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8f9de-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="8f9de-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8f9de-118">Request headers</span></span>
|<span data-ttu-id="8f9de-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8f9de-119">Header</span></span>|<span data-ttu-id="8f9de-120">Wert</span><span class="sxs-lookup"><span data-stu-id="8f9de-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f9de-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f9de-121">Authorization</span></span>|<span data-ttu-id="8f9de-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8f9de-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f9de-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8f9de-123">Accept</span></span>|<span data-ttu-id="8f9de-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8f9de-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f9de-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8f9de-125">Request body</span></span>
<span data-ttu-id="8f9de-126">Geben Sie im Anforderungstext eine JSON Darstellung für das [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="8f9de-126">In the request body, supply a JSON representation for the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

<span data-ttu-id="8f9de-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="8f9de-127">The following table shows the properties that are required when you create the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>

|<span data-ttu-id="8f9de-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8f9de-128">Property</span></span>|<span data-ttu-id="8f9de-129">Typ</span><span class="sxs-lookup"><span data-stu-id="8f9de-129">Type</span></span>|<span data-ttu-id="8f9de-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8f9de-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f9de-131">id</span><span class="sxs-lookup"><span data-stu-id="8f9de-131">id</span></span>|<span data-ttu-id="8f9de-132">String</span><span class="sxs-lookup"><span data-stu-id="8f9de-132">String</span></span>|<span data-ttu-id="8f9de-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8f9de-133">Key of the entity.</span></span>|
|<span data-ttu-id="8f9de-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8f9de-134">lastModifiedDateTime</span></span>|<span data-ttu-id="8f9de-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f9de-135">DateTimeOffset</span></span>|<span data-ttu-id="8f9de-136">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8f9de-136">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="8f9de-137">Gebietsschema</span><span class="sxs-lookup"><span data-stu-id="8f9de-137">locale</span></span>|<span data-ttu-id="8f9de-138">String</span><span class="sxs-lookup"><span data-stu-id="8f9de-138">String</span></span>|<span data-ttu-id="8f9de-139">Das Gebietsschema für das diese Nachricht bestimmt ist.</span><span class="sxs-lookup"><span data-stu-id="8f9de-139">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="8f9de-140">Betreff</span><span class="sxs-lookup"><span data-stu-id="8f9de-140">subject</span></span>|<span data-ttu-id="8f9de-141">String</span><span class="sxs-lookup"><span data-stu-id="8f9de-141">String</span></span>|<span data-ttu-id="8f9de-142">Die Vorlage für den Betreff der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="8f9de-142">The Message Template Subject.</span></span>|
|<span data-ttu-id="8f9de-143">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="8f9de-143">messageTemplate</span></span>|<span data-ttu-id="8f9de-144">String</span><span class="sxs-lookup"><span data-stu-id="8f9de-144">String</span></span>|<span data-ttu-id="8f9de-145">Die Vorlage für den Inhalt der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="8f9de-145">The Message Template content.</span></span>|
|<span data-ttu-id="8f9de-146">isDefault</span><span class="sxs-lookup"><span data-stu-id="8f9de-146">isDefault</span></span>|<span data-ttu-id="8f9de-147">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8f9de-147">Boolean</span></span>|<span data-ttu-id="8f9de-148">Die Kennzeichnung gibt an, ob dies das Standard-Gebietsschema für die Fallbacksprache ist.</span><span class="sxs-lookup"><span data-stu-id="8f9de-148">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="8f9de-149">Dieser Kennzeichnung kann nur festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="8f9de-149">This flag can only be set.</span></span> <span data-ttu-id="8f9de-150">Um die Festlegung aufzuheben, setzen Sie diese Eigenschaft bei einer anderen lokalisierten Benachrichtigung auf „true“.</span><span class="sxs-lookup"><span data-stu-id="8f9de-150">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="8f9de-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="8f9de-151">Response</span></span>
<span data-ttu-id="8f9de-152">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8f9de-152">If successful, this method returns a `200 OK` response code and an updated [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f9de-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8f9de-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="8f9de-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8f9de-154">Request</span></span>
<span data-ttu-id="8f9de-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8f9de-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
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

### <a name="response"></a><span data-ttu-id="8f9de-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="8f9de-156">Response</span></span>
<span data-ttu-id="8f9de-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8f9de-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



