---
title: localizedNotificationMessage aktualisieren
description: Aktualisieren der Eigenschaften eines LocalizedNotificationMessage-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7b67dabbe08d9fb8c85f1a955d6233915912fdf4
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30969099"
---
# <a name="update-localizednotificationmessage"></a><span data-ttu-id="56886-103">localizedNotificationMessage aktualisieren</span><span class="sxs-lookup"><span data-stu-id="56886-103">Update localizedNotificationMessage</span></span>

> <span data-ttu-id="56886-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="56886-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56886-105">Aktualisieren der Eigenschaften eines [LocalizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="56886-105">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="56886-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="56886-106">Prerequisites</span></span>
<span data-ttu-id="56886-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56886-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56886-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="56886-109">Permission type</span></span>|<span data-ttu-id="56886-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="56886-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56886-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="56886-111">Delegated (work or school account)</span></span>|<span data-ttu-id="56886-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56886-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="56886-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="56886-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56886-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="56886-114">Not supported.</span></span>|
|<span data-ttu-id="56886-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="56886-115">Application</span></span>|<span data-ttu-id="56886-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="56886-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56886-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="56886-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="56886-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="56886-118">Request headers</span></span>
|<span data-ttu-id="56886-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="56886-119">Header</span></span>|<span data-ttu-id="56886-120">Wert</span><span class="sxs-lookup"><span data-stu-id="56886-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56886-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="56886-121">Authorization</span></span>|<span data-ttu-id="56886-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="56886-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56886-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="56886-123">Accept</span></span>|<span data-ttu-id="56886-124">application/json</span><span class="sxs-lookup"><span data-stu-id="56886-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56886-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="56886-125">Request body</span></span>
<span data-ttu-id="56886-126">Geben Sie im Anforderungstext eine JSON Darstellung für das [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="56886-126">In the request body, supply a JSON representation for the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

<span data-ttu-id="56886-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="56886-127">The following table shows the properties that are required when you create the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>

|<span data-ttu-id="56886-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="56886-128">Property</span></span>|<span data-ttu-id="56886-129">Typ</span><span class="sxs-lookup"><span data-stu-id="56886-129">Type</span></span>|<span data-ttu-id="56886-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="56886-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56886-131">id</span><span class="sxs-lookup"><span data-stu-id="56886-131">id</span></span>|<span data-ttu-id="56886-132">String</span><span class="sxs-lookup"><span data-stu-id="56886-132">String</span></span>|<span data-ttu-id="56886-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="56886-133">Key of the entity.</span></span>|
|<span data-ttu-id="56886-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="56886-134">lastModifiedDateTime</span></span>|<span data-ttu-id="56886-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56886-135">DateTimeOffset</span></span>|<span data-ttu-id="56886-136">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="56886-136">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="56886-137">Gebietsschema</span><span class="sxs-lookup"><span data-stu-id="56886-137">locale</span></span>|<span data-ttu-id="56886-138">String</span><span class="sxs-lookup"><span data-stu-id="56886-138">String</span></span>|<span data-ttu-id="56886-139">Das Gebietsschema für das diese Nachricht bestimmt ist.</span><span class="sxs-lookup"><span data-stu-id="56886-139">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="56886-140">subject</span><span class="sxs-lookup"><span data-stu-id="56886-140">subject</span></span>|<span data-ttu-id="56886-141">String</span><span class="sxs-lookup"><span data-stu-id="56886-141">String</span></span>|<span data-ttu-id="56886-142">Die Vorlage für den Betreff der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="56886-142">The Message Template Subject.</span></span>|
|<span data-ttu-id="56886-143">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="56886-143">messageTemplate</span></span>|<span data-ttu-id="56886-144">String</span><span class="sxs-lookup"><span data-stu-id="56886-144">String</span></span>|<span data-ttu-id="56886-145">Die Vorlage für den Inhalt der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="56886-145">The Message Template content.</span></span>|
|<span data-ttu-id="56886-146">isDefault</span><span class="sxs-lookup"><span data-stu-id="56886-146">isDefault</span></span>|<span data-ttu-id="56886-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="56886-147">Boolean</span></span>|<span data-ttu-id="56886-148">Die Kennzeichnung gibt an, ob dies das Standard-Gebietsschema für die Fallbacksprache ist.</span><span class="sxs-lookup"><span data-stu-id="56886-148">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="56886-149">Dieser Kennzeichnung kann nur festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="56886-149">This flag can only be set.</span></span> <span data-ttu-id="56886-150">Um die Festlegung aufzuheben, setzen Sie diese Eigenschaft bei einer anderen lokalisierten Benachrichtigung auf „true“.</span><span class="sxs-lookup"><span data-stu-id="56886-150">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="56886-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="56886-151">Response</span></span>
<span data-ttu-id="56886-152">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="56886-152">If successful, this method returns a `200 OK` response code and an updated [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56886-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="56886-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="56886-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="56886-154">Request</span></span>
<span data-ttu-id="56886-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="56886-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="56886-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="56886-156">Response</span></span>
<span data-ttu-id="56886-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="56886-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



