---
title: localizedNotificationMessage aktualisieren
description: Aktualisieren der Eigenschaften eines LocalizedNotificationMessage-Objekts.
ms.openlocfilehash: d61f97d44e4c5b2e6f5b17e1538620f774200a18
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059333"
---
# <a name="update-localizednotificationmessage"></a><span data-ttu-id="58523-103">localizedNotificationMessage aktualisieren</span><span class="sxs-lookup"><span data-stu-id="58523-103">Update localizedNotificationMessage</span></span>

> <span data-ttu-id="58523-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="58523-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="58523-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="58523-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="58523-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="58523-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="58523-107">Aktualisieren der Eigenschaften eines [LocalizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="58523-107">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="58523-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="58523-108">Prerequisites</span></span>
<span data-ttu-id="58523-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58523-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58523-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="58523-111">Permission type</span></span>|<span data-ttu-id="58523-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="58523-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58523-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="58523-113">Delegated (work or school account)</span></span>|<span data-ttu-id="58523-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58523-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="58523-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="58523-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58523-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="58523-116">Not supported.</span></span>|
|<span data-ttu-id="58523-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="58523-117">Application</span></span>|<span data-ttu-id="58523-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="58523-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58523-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="58523-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="58523-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="58523-120">Request headers</span></span>
|<span data-ttu-id="58523-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="58523-121">Header</span></span>|<span data-ttu-id="58523-122">Wert</span><span class="sxs-lookup"><span data-stu-id="58523-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58523-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="58523-123">Authorization</span></span>|<span data-ttu-id="58523-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="58523-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58523-125">Accept</span><span class="sxs-lookup"><span data-stu-id="58523-125">Accept</span></span>|<span data-ttu-id="58523-126">application/json</span><span class="sxs-lookup"><span data-stu-id="58523-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58523-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="58523-127">Request body</span></span>
<span data-ttu-id="58523-128">Geben Sie im Anforderungstext eine JSON Darstellung für das [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="58523-128">In the request body, supply a JSON representation for the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

<span data-ttu-id="58523-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="58523-129">The following table shows the properties that are required when you create the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>

|<span data-ttu-id="58523-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="58523-130">Property</span></span>|<span data-ttu-id="58523-131">Typ</span><span class="sxs-lookup"><span data-stu-id="58523-131">Type</span></span>|<span data-ttu-id="58523-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="58523-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58523-133">id</span><span class="sxs-lookup"><span data-stu-id="58523-133">id</span></span>|<span data-ttu-id="58523-134">String</span><span class="sxs-lookup"><span data-stu-id="58523-134">String</span></span>|<span data-ttu-id="58523-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="58523-135">Key of the entity.</span></span>|
|<span data-ttu-id="58523-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="58523-136">lastModifiedDateTime</span></span>|<span data-ttu-id="58523-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58523-137">DateTimeOffset</span></span>|<span data-ttu-id="58523-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="58523-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="58523-139">Gebietsschema</span><span class="sxs-lookup"><span data-stu-id="58523-139">locale</span></span>|<span data-ttu-id="58523-140">String</span><span class="sxs-lookup"><span data-stu-id="58523-140">String</span></span>|<span data-ttu-id="58523-141">Das Gebietsschema für das diese Nachricht bestimmt ist.</span><span class="sxs-lookup"><span data-stu-id="58523-141">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="58523-142">Betreff</span><span class="sxs-lookup"><span data-stu-id="58523-142">subject</span></span>|<span data-ttu-id="58523-143">String</span><span class="sxs-lookup"><span data-stu-id="58523-143">String</span></span>|<span data-ttu-id="58523-144">Die Vorlage für den Betreff der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="58523-144">The Message Template Subject.</span></span>|
|<span data-ttu-id="58523-145">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="58523-145">messageTemplate</span></span>|<span data-ttu-id="58523-146">String</span><span class="sxs-lookup"><span data-stu-id="58523-146">String</span></span>|<span data-ttu-id="58523-147">Die Vorlage für den Inhalt der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="58523-147">The Message Template content.</span></span>|
|<span data-ttu-id="58523-148">isDefault</span><span class="sxs-lookup"><span data-stu-id="58523-148">isDefault</span></span>|<span data-ttu-id="58523-149">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="58523-149">Boolean</span></span>|<span data-ttu-id="58523-150">Die Kennzeichnung gibt an, ob dies das Standard-Gebietsschema für die Fallbacksprache ist.</span><span class="sxs-lookup"><span data-stu-id="58523-150">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="58523-151">Dieser Kennzeichnung kann nur festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="58523-151">This flag can only be set.</span></span> <span data-ttu-id="58523-152">Um die Festlegung aufzuheben, setzen Sie diese Eigenschaft bei einer anderen lokalisierten Benachrichtigung auf „true“.</span><span class="sxs-lookup"><span data-stu-id="58523-152">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="58523-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="58523-153">Response</span></span>
<span data-ttu-id="58523-154">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="58523-154">If successful, this method returns a `200 OK` response code and an updated [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58523-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="58523-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="58523-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="58523-156">Request</span></span>
<span data-ttu-id="58523-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="58523-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
Content-type: application/json
Content-length: 197

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "locale": "Locale value",
  "subject": "Subject value",
  "messageTemplate": "Message Template value",
  "isDefault": true
}
```

### <a name="response"></a><span data-ttu-id="58523-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="58523-158">Response</span></span>
<span data-ttu-id="58523-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="58523-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





