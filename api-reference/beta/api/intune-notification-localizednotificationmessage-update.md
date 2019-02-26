---
title: localizedNotificationMessage aktualisieren
description: Aktualisieren der Eigenschaften eines LocalizedNotificationMessage-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 492802765d53826ea01477b988582a58bf771d31
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142287"
---
# <a name="update-localizednotificationmessage"></a><span data-ttu-id="c778c-103">localizedNotificationMessage aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c778c-103">Update localizedNotificationMessage</span></span>

> <span data-ttu-id="c778c-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c778c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c778c-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c778c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c778c-106">Aktualisieren der Eigenschaften eines [LocalizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c778c-106">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c778c-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c778c-107">Prerequisites</span></span>
<span data-ttu-id="c778c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c778c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c778c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c778c-110">Permission type</span></span>|<span data-ttu-id="c778c-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c778c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c778c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c778c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c778c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c778c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c778c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c778c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c778c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c778c-115">Not supported.</span></span>|
|<span data-ttu-id="c778c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c778c-116">Application</span></span>|<span data-ttu-id="c778c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c778c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c778c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c778c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="c778c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c778c-119">Request headers</span></span>
|<span data-ttu-id="c778c-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c778c-120">Header</span></span>|<span data-ttu-id="c778c-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c778c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c778c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c778c-122">Authorization</span></span>|<span data-ttu-id="c778c-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c778c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c778c-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c778c-124">Accept</span></span>|<span data-ttu-id="c778c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c778c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c778c-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c778c-126">Request body</span></span>
<span data-ttu-id="c778c-127">Geben Sie im Anforderungstext eine JSON Darstellung für das [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="c778c-127">In the request body, supply a JSON representation for the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

<span data-ttu-id="c778c-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c778c-128">The following table shows the properties that are required when you create the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>

|<span data-ttu-id="c778c-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c778c-129">Property</span></span>|<span data-ttu-id="c778c-130">Typ</span><span class="sxs-lookup"><span data-stu-id="c778c-130">Type</span></span>|<span data-ttu-id="c778c-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c778c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c778c-132">id</span><span class="sxs-lookup"><span data-stu-id="c778c-132">id</span></span>|<span data-ttu-id="c778c-133">String</span><span class="sxs-lookup"><span data-stu-id="c778c-133">String</span></span>|<span data-ttu-id="c778c-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c778c-134">Key of the entity.</span></span>|
|<span data-ttu-id="c778c-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c778c-135">lastModifiedDateTime</span></span>|<span data-ttu-id="c778c-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c778c-136">DateTimeOffset</span></span>|<span data-ttu-id="c778c-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c778c-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="c778c-138">Gebietsschema</span><span class="sxs-lookup"><span data-stu-id="c778c-138">locale</span></span>|<span data-ttu-id="c778c-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c778c-139">String</span></span>|<span data-ttu-id="c778c-140">Das Gebietsschema für das diese Nachricht bestimmt ist.</span><span class="sxs-lookup"><span data-stu-id="c778c-140">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="c778c-141">Betreff</span><span class="sxs-lookup"><span data-stu-id="c778c-141">subject</span></span>|<span data-ttu-id="c778c-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c778c-142">String</span></span>|<span data-ttu-id="c778c-143">Die Vorlage für den Betreff der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="c778c-143">The Message Template Subject.</span></span>|
|<span data-ttu-id="c778c-144">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="c778c-144">messageTemplate</span></span>|<span data-ttu-id="c778c-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c778c-145">String</span></span>|<span data-ttu-id="c778c-146">Die Vorlage für den Inhalt der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="c778c-146">The Message Template content.</span></span>|
|<span data-ttu-id="c778c-147">isDefault</span><span class="sxs-lookup"><span data-stu-id="c778c-147">isDefault</span></span>|<span data-ttu-id="c778c-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="c778c-148">Boolean</span></span>|<span data-ttu-id="c778c-149">Die Kennzeichnung gibt an, ob dies das Standard-Gebietsschema für die Fallbacksprache ist.</span><span class="sxs-lookup"><span data-stu-id="c778c-149">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="c778c-150">Dieser Kennzeichnung kann nur festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="c778c-150">This flag can only be set.</span></span> <span data-ttu-id="c778c-151">Um die Festlegung aufzuheben, setzen Sie diese Eigenschaft bei einer anderen lokalisierten Benachrichtigung auf „true“.</span><span class="sxs-lookup"><span data-stu-id="c778c-151">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="c778c-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="c778c-152">Response</span></span>
<span data-ttu-id="c778c-153">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c778c-153">If successful, this method returns a `200 OK` response code and an updated [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c778c-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c778c-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="c778c-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c778c-155">Request</span></span>
<span data-ttu-id="c778c-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c778c-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
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

### <a name="response"></a><span data-ttu-id="c778c-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="c778c-157">Response</span></span>
<span data-ttu-id="c778c-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c778c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




