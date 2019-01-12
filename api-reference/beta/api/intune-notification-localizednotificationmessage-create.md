---
title: localizedNotificationMessage erstellen
description: Erstellen eines neuen localizedNotificationMessage-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bf0187177a80428924af6276eaf9df6f6456e2d2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950795"
---
# <a name="create-localizednotificationmessage"></a><span data-ttu-id="acee9-103">localizedNotificationMessage erstellen</span><span class="sxs-lookup"><span data-stu-id="acee9-103">Create localizedNotificationMessage</span></span>

> <span data-ttu-id="acee9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="acee9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="acee9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="acee9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="acee9-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="acee9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="acee9-107">Erstellen eines neuen [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="acee9-107">Create a new [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="acee9-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="acee9-108">Prerequisites</span></span>
<span data-ttu-id="acee9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="acee9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acee9-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="acee9-111">Permission type</span></span>|<span data-ttu-id="acee9-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="acee9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="acee9-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="acee9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="acee9-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acee9-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="acee9-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="acee9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="acee9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="acee9-116">Not supported.</span></span>|
|<span data-ttu-id="acee9-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="acee9-117">Application</span></span>|<span data-ttu-id="acee9-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="acee9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="acee9-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="acee9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="acee9-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="acee9-120">Request headers</span></span>
|<span data-ttu-id="acee9-121">Header</span><span class="sxs-lookup"><span data-stu-id="acee9-121">Header</span></span>|<span data-ttu-id="acee9-122">Wert</span><span class="sxs-lookup"><span data-stu-id="acee9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="acee9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="acee9-123">Authorization</span></span>|<span data-ttu-id="acee9-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="acee9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="acee9-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="acee9-125">Accept</span></span>|<span data-ttu-id="acee9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="acee9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="acee9-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="acee9-127">Request body</span></span>
<span data-ttu-id="acee9-128">Geben Sie im Anforderungstext eine JSON Darstellung für das localizedNotificationMessage-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="acee9-128">In the request body, supply a JSON representation for the localizedNotificationMessage object.</span></span>

<span data-ttu-id="acee9-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der localizedNotificationMessage erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="acee9-129">The following table shows the properties that are required when you create the localizedNotificationMessage.</span></span>

|<span data-ttu-id="acee9-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="acee9-130">Property</span></span>|<span data-ttu-id="acee9-131">Typ</span><span class="sxs-lookup"><span data-stu-id="acee9-131">Type</span></span>|<span data-ttu-id="acee9-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="acee9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="acee9-133">id</span><span class="sxs-lookup"><span data-stu-id="acee9-133">id</span></span>|<span data-ttu-id="acee9-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="acee9-134">String</span></span>|<span data-ttu-id="acee9-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="acee9-135">Key of the entity.</span></span>|
|<span data-ttu-id="acee9-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="acee9-136">lastModifiedDateTime</span></span>|<span data-ttu-id="acee9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="acee9-137">DateTimeOffset</span></span>|<span data-ttu-id="acee9-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="acee9-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="acee9-139">Gebietsschema</span><span class="sxs-lookup"><span data-stu-id="acee9-139">locale</span></span>|<span data-ttu-id="acee9-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="acee9-140">String</span></span>|<span data-ttu-id="acee9-141">Das Gebietsschema für das diese Nachricht bestimmt ist.</span><span class="sxs-lookup"><span data-stu-id="acee9-141">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="acee9-142">Betreff</span><span class="sxs-lookup"><span data-stu-id="acee9-142">subject</span></span>|<span data-ttu-id="acee9-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="acee9-143">String</span></span>|<span data-ttu-id="acee9-144">Die Vorlage für den Betreff der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="acee9-144">The Message Template Subject.</span></span>|
|<span data-ttu-id="acee9-145">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="acee9-145">messageTemplate</span></span>|<span data-ttu-id="acee9-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="acee9-146">String</span></span>|<span data-ttu-id="acee9-147">Die Vorlage für den Inhalt der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="acee9-147">The Message Template content.</span></span>|
|<span data-ttu-id="acee9-148">isDefault</span><span class="sxs-lookup"><span data-stu-id="acee9-148">isDefault</span></span>|<span data-ttu-id="acee9-149">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="acee9-149">Boolean</span></span>|<span data-ttu-id="acee9-150">Die Kennzeichnung gibt an, ob dies das Standard-Gebietsschema für die Fallbacksprache ist.</span><span class="sxs-lookup"><span data-stu-id="acee9-150">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="acee9-151">Dieser Kennzeichnung kann nur festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="acee9-151">This flag can only be set.</span></span> <span data-ttu-id="acee9-152">Um die Festlegung aufzuheben, setzen Sie diese Eigenschaft bei einer anderen lokalisierten Benachrichtigung auf „true“.</span><span class="sxs-lookup"><span data-stu-id="acee9-152">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="acee9-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="acee9-153">Response</span></span>
<span data-ttu-id="acee9-154">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="acee9-154">If successful, this method returns a `201 Created` response code and a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="acee9-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="acee9-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="acee9-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="acee9-156">Request</span></span>
<span data-ttu-id="acee9-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="acee9-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
Content-type: application/json
Content-length: 264

{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "locale": "Locale value",
  "subject": "Subject value",
  "messageTemplate": "Message Template value",
  "isDefault": true
}
```

### <a name="response"></a><span data-ttu-id="acee9-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="acee9-158">Response</span></span>
<span data-ttu-id="acee9-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="acee9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





