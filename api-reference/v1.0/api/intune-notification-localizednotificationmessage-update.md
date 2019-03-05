---
title: localizedNotificationMessage aktualisieren
description: Aktualisieren der Eigenschaften eines LocalizedNotificationMessage-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dc84aaf2963598cb90aef65d34918262c1e0c92c
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250845"
---
# <a name="update-localizednotificationmessage"></a><span data-ttu-id="8e16c-103">localizedNotificationMessage aktualisieren</span><span class="sxs-lookup"><span data-stu-id="8e16c-103">Update localizedNotificationMessage</span></span>

> <span data-ttu-id="8e16c-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="8e16c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e16c-105">Aktualisieren der Eigenschaften eines [LocalizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8e16c-105">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e16c-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8e16c-106">Prerequisites</span></span>
<span data-ttu-id="8e16c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8e16c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8e16c-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8e16c-109">Permission type</span></span>|<span data-ttu-id="8e16c-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8e16c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e16c-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8e16c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8e16c-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e16c-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8e16c-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8e16c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e16c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8e16c-114">Not supported.</span></span>|
|<span data-ttu-id="8e16c-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8e16c-115">Application</span></span>|<span data-ttu-id="8e16c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8e16c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e16c-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8e16c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="8e16c-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8e16c-118">Request headers</span></span>
|<span data-ttu-id="8e16c-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8e16c-119">Header</span></span>|<span data-ttu-id="8e16c-120">Wert</span><span class="sxs-lookup"><span data-stu-id="8e16c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e16c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e16c-121">Authorization</span></span>|<span data-ttu-id="8e16c-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8e16c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e16c-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8e16c-123">Accept</span></span>|<span data-ttu-id="8e16c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8e16c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e16c-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8e16c-125">Request body</span></span>
<span data-ttu-id="8e16c-126">Geben Sie im Anforderungstext eine JSON Darstellung für das [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="8e16c-126">In the request body, supply a JSON representation for the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

<span data-ttu-id="8e16c-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="8e16c-127">The following table shows the properties that are required when you create the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>

|<span data-ttu-id="8e16c-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8e16c-128">Property</span></span>|<span data-ttu-id="8e16c-129">Typ</span><span class="sxs-lookup"><span data-stu-id="8e16c-129">Type</span></span>|<span data-ttu-id="8e16c-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8e16c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e16c-131">id</span><span class="sxs-lookup"><span data-stu-id="8e16c-131">id</span></span>|<span data-ttu-id="8e16c-132">String</span><span class="sxs-lookup"><span data-stu-id="8e16c-132">String</span></span>|<span data-ttu-id="8e16c-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8e16c-133">Key of the entity.</span></span>|
|<span data-ttu-id="8e16c-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8e16c-134">lastModifiedDateTime</span></span>|<span data-ttu-id="8e16c-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e16c-135">DateTimeOffset</span></span>|<span data-ttu-id="8e16c-136">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8e16c-136">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="8e16c-137">Gebietsschema</span><span class="sxs-lookup"><span data-stu-id="8e16c-137">locale</span></span>|<span data-ttu-id="8e16c-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8e16c-138">String</span></span>|<span data-ttu-id="8e16c-139">Das Gebietsschema für das diese Nachricht bestimmt ist.</span><span class="sxs-lookup"><span data-stu-id="8e16c-139">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="8e16c-140">Betreff</span><span class="sxs-lookup"><span data-stu-id="8e16c-140">subject</span></span>|<span data-ttu-id="8e16c-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8e16c-141">String</span></span>|<span data-ttu-id="8e16c-142">Die Vorlage für den Betreff der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="8e16c-142">The Message Template Subject.</span></span>|
|<span data-ttu-id="8e16c-143">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="8e16c-143">messageTemplate</span></span>|<span data-ttu-id="8e16c-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8e16c-144">String</span></span>|<span data-ttu-id="8e16c-145">Die Vorlage für den Inhalt der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="8e16c-145">The Message Template content.</span></span>|
|<span data-ttu-id="8e16c-146">isDefault</span><span class="sxs-lookup"><span data-stu-id="8e16c-146">isDefault</span></span>|<span data-ttu-id="8e16c-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e16c-147">Boolean</span></span>|<span data-ttu-id="8e16c-148">Die Kennzeichnung gibt an, ob dies das Standard-Gebietsschema für die Fallbacksprache ist.</span><span class="sxs-lookup"><span data-stu-id="8e16c-148">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="8e16c-149">Dieser Kennzeichnung kann nur festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="8e16c-149">This flag can only be set.</span></span> <span data-ttu-id="8e16c-150">Um die Festlegung aufzuheben, setzen Sie diese Eigenschaft bei einer anderen lokalisierten Benachrichtigung auf „true“.</span><span class="sxs-lookup"><span data-stu-id="8e16c-150">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="8e16c-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="8e16c-151">Response</span></span>
<span data-ttu-id="8e16c-152">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8e16c-152">If successful, this method returns a `200 OK` response code and an updated [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e16c-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8e16c-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e16c-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8e16c-154">Request</span></span>
<span data-ttu-id="8e16c-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8e16c-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8e16c-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="8e16c-156">Response</span></span>
<span data-ttu-id="8e16c-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8e16c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



