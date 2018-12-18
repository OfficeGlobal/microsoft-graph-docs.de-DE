---
title: localizedNotificationMessage erstellen
description: Erstellen eines neuen localizedNotificationMessage-Objekts.
author: tfitzmac
ms.openlocfilehash: 8bc782f69e769e32acd29932b4f224c7cf764c04
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353543"
---
# <a name="create-localizednotificationmessage"></a><span data-ttu-id="cd2a7-103">localizedNotificationMessage erstellen</span><span class="sxs-lookup"><span data-stu-id="cd2a7-103">Create localizedNotificationMessage</span></span>

> <span data-ttu-id="cd2a7-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="cd2a7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cd2a7-105">Erstellen eines neuen [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="cd2a7-105">Create a new [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cd2a7-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cd2a7-106">Prerequisites</span></span>
<span data-ttu-id="cd2a7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd2a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd2a7-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cd2a7-109">Permission type</span></span>|<span data-ttu-id="cd2a7-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cd2a7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd2a7-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cd2a7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cd2a7-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd2a7-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cd2a7-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cd2a7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd2a7-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cd2a7-114">Not supported.</span></span>|
|<span data-ttu-id="cd2a7-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cd2a7-115">Application</span></span>|<span data-ttu-id="cd2a7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cd2a7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd2a7-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd2a7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="cd2a7-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cd2a7-118">Request headers</span></span>
|<span data-ttu-id="cd2a7-119">Header</span><span class="sxs-lookup"><span data-stu-id="cd2a7-119">Header</span></span>|<span data-ttu-id="cd2a7-120">Wert</span><span class="sxs-lookup"><span data-stu-id="cd2a7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd2a7-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="cd2a7-121">Authorization</span></span>|<span data-ttu-id="cd2a7-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cd2a7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd2a7-123">Accept</span><span class="sxs-lookup"><span data-stu-id="cd2a7-123">Accept</span></span>|<span data-ttu-id="cd2a7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cd2a7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd2a7-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cd2a7-125">Request body</span></span>
<span data-ttu-id="cd2a7-126">Geben Sie im Anforderungstext eine JSON Darstellung für das localizedNotificationMessage-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="cd2a7-126">In the request body, supply a JSON representation for the localizedNotificationMessage object.</span></span>

<span data-ttu-id="cd2a7-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der localizedNotificationMessage erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="cd2a7-127">The following table shows the properties that are required when you create the localizedNotificationMessage.</span></span>

|<span data-ttu-id="cd2a7-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cd2a7-128">Property</span></span>|<span data-ttu-id="cd2a7-129">Typ</span><span class="sxs-lookup"><span data-stu-id="cd2a7-129">Type</span></span>|<span data-ttu-id="cd2a7-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cd2a7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd2a7-131">id</span><span class="sxs-lookup"><span data-stu-id="cd2a7-131">id</span></span>|<span data-ttu-id="cd2a7-132">String</span><span class="sxs-lookup"><span data-stu-id="cd2a7-132">String</span></span>|<span data-ttu-id="cd2a7-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="cd2a7-133">Key of the entity.</span></span>|
|<span data-ttu-id="cd2a7-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cd2a7-134">lastModifiedDateTime</span></span>|<span data-ttu-id="cd2a7-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd2a7-135">DateTimeOffset</span></span>|<span data-ttu-id="cd2a7-136">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="cd2a7-136">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="cd2a7-137">Gebietsschema</span><span class="sxs-lookup"><span data-stu-id="cd2a7-137">locale</span></span>|<span data-ttu-id="cd2a7-138">String</span><span class="sxs-lookup"><span data-stu-id="cd2a7-138">String</span></span>|<span data-ttu-id="cd2a7-139">Das Gebietsschema für das diese Nachricht bestimmt ist.</span><span class="sxs-lookup"><span data-stu-id="cd2a7-139">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="cd2a7-140">Betreff</span><span class="sxs-lookup"><span data-stu-id="cd2a7-140">subject</span></span>|<span data-ttu-id="cd2a7-141">String</span><span class="sxs-lookup"><span data-stu-id="cd2a7-141">String</span></span>|<span data-ttu-id="cd2a7-142">Die Vorlage für den Betreff der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="cd2a7-142">The Message Template Subject.</span></span>|
|<span data-ttu-id="cd2a7-143">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="cd2a7-143">messageTemplate</span></span>|<span data-ttu-id="cd2a7-144">String</span><span class="sxs-lookup"><span data-stu-id="cd2a7-144">String</span></span>|<span data-ttu-id="cd2a7-145">Die Vorlage für den Inhalt der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="cd2a7-145">The Message Template content.</span></span>|
|<span data-ttu-id="cd2a7-146">isDefault</span><span class="sxs-lookup"><span data-stu-id="cd2a7-146">isDefault</span></span>|<span data-ttu-id="cd2a7-147">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="cd2a7-147">Boolean</span></span>|<span data-ttu-id="cd2a7-148">Die Kennzeichnung gibt an, ob dies das Standard-Gebietsschema für die Fallbacksprache ist.</span><span class="sxs-lookup"><span data-stu-id="cd2a7-148">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="cd2a7-149">Dieser Kennzeichnung kann nur festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="cd2a7-149">This flag can only be set.</span></span> <span data-ttu-id="cd2a7-150">Um die Festlegung aufzuheben, setzen Sie diese Eigenschaft bei einer anderen lokalisierten Benachrichtigung auf „true“.</span><span class="sxs-lookup"><span data-stu-id="cd2a7-150">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="cd2a7-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd2a7-151">Response</span></span>
<span data-ttu-id="cd2a7-152">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="cd2a7-152">If successful, this method returns a `201 Created` response code and a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd2a7-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cd2a7-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="cd2a7-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd2a7-154">Request</span></span>
<span data-ttu-id="cd2a7-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cd2a7-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cd2a7-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd2a7-156">Response</span></span>
<span data-ttu-id="cd2a7-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cd2a7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



