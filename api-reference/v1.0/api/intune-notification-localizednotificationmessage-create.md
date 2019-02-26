---
title: localizedNotificationMessage erstellen
description: Erstellen eines neuen localizedNotificationMessage-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8b4b793e149bc2973b85735769af70aa20a2d29a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259269"
---
# <a name="create-localizednotificationmessage"></a><span data-ttu-id="254c5-103">localizedNotificationMessage erstellen</span><span class="sxs-lookup"><span data-stu-id="254c5-103">Create localizedNotificationMessage</span></span>

> <span data-ttu-id="254c5-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="254c5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="254c5-105">Erstellen eines neuen [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="254c5-105">Create a new [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="254c5-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="254c5-106">Prerequisites</span></span>
<span data-ttu-id="254c5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="254c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="254c5-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="254c5-109">Permission type</span></span>|<span data-ttu-id="254c5-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="254c5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="254c5-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="254c5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="254c5-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="254c5-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="254c5-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="254c5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="254c5-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="254c5-114">Not supported.</span></span>|
|<span data-ttu-id="254c5-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="254c5-115">Application</span></span>|<span data-ttu-id="254c5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="254c5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="254c5-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="254c5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="254c5-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="254c5-118">Request headers</span></span>
|<span data-ttu-id="254c5-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="254c5-119">Header</span></span>|<span data-ttu-id="254c5-120">Wert</span><span class="sxs-lookup"><span data-stu-id="254c5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="254c5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="254c5-121">Authorization</span></span>|<span data-ttu-id="254c5-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="254c5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="254c5-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="254c5-123">Accept</span></span>|<span data-ttu-id="254c5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="254c5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="254c5-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="254c5-125">Request body</span></span>
<span data-ttu-id="254c5-126">Geben Sie im Anforderungstext eine JSON Darstellung für das localizedNotificationMessage-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="254c5-126">In the request body, supply a JSON representation for the localizedNotificationMessage object.</span></span>

<span data-ttu-id="254c5-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der localizedNotificationMessage erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="254c5-127">The following table shows the properties that are required when you create the localizedNotificationMessage.</span></span>

|<span data-ttu-id="254c5-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="254c5-128">Property</span></span>|<span data-ttu-id="254c5-129">Typ</span><span class="sxs-lookup"><span data-stu-id="254c5-129">Type</span></span>|<span data-ttu-id="254c5-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="254c5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="254c5-131">id</span><span class="sxs-lookup"><span data-stu-id="254c5-131">id</span></span>|<span data-ttu-id="254c5-132">String</span><span class="sxs-lookup"><span data-stu-id="254c5-132">String</span></span>|<span data-ttu-id="254c5-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="254c5-133">Key of the entity.</span></span>|
|<span data-ttu-id="254c5-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="254c5-134">lastModifiedDateTime</span></span>|<span data-ttu-id="254c5-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="254c5-135">DateTimeOffset</span></span>|<span data-ttu-id="254c5-136">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="254c5-136">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="254c5-137">Gebietsschema</span><span class="sxs-lookup"><span data-stu-id="254c5-137">locale</span></span>|<span data-ttu-id="254c5-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="254c5-138">String</span></span>|<span data-ttu-id="254c5-139">Das Gebietsschema für das diese Nachricht bestimmt ist.</span><span class="sxs-lookup"><span data-stu-id="254c5-139">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="254c5-140">Betreff</span><span class="sxs-lookup"><span data-stu-id="254c5-140">subject</span></span>|<span data-ttu-id="254c5-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="254c5-141">String</span></span>|<span data-ttu-id="254c5-142">Die Vorlage für den Betreff der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="254c5-142">The Message Template Subject.</span></span>|
|<span data-ttu-id="254c5-143">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="254c5-143">messageTemplate</span></span>|<span data-ttu-id="254c5-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="254c5-144">String</span></span>|<span data-ttu-id="254c5-145">Die Vorlage für den Inhalt der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="254c5-145">The Message Template content.</span></span>|
|<span data-ttu-id="254c5-146">isDefault</span><span class="sxs-lookup"><span data-stu-id="254c5-146">isDefault</span></span>|<span data-ttu-id="254c5-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="254c5-147">Boolean</span></span>|<span data-ttu-id="254c5-148">Die Kennzeichnung gibt an, ob dies das Standard-Gebietsschema für die Fallbacksprache ist.</span><span class="sxs-lookup"><span data-stu-id="254c5-148">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="254c5-149">Dieser Kennzeichnung kann nur festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="254c5-149">This flag can only be set.</span></span> <span data-ttu-id="254c5-150">Um die Festlegung aufzuheben, setzen Sie diese Eigenschaft bei einer anderen lokalisierten Benachrichtigung auf „true“.</span><span class="sxs-lookup"><span data-stu-id="254c5-150">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="254c5-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="254c5-151">Response</span></span>
<span data-ttu-id="254c5-152">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="254c5-152">If successful, this method returns a `201 Created` response code and a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="254c5-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="254c5-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="254c5-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="254c5-154">Request</span></span>
<span data-ttu-id="254c5-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="254c5-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="254c5-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="254c5-156">Response</span></span>
<span data-ttu-id="254c5-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="254c5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



