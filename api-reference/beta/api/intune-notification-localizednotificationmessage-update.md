---
title: localizedNotificationMessage aktualisieren
description: Aktualisieren der Eigenschaften eines LocalizedNotificationMessage-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bae1ef62325a7675b626be0bc21f65e3cb45b513
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395503"
---
# <a name="update-localizednotificationmessage"></a><span data-ttu-id="5f088-103">localizedNotificationMessage aktualisieren</span><span class="sxs-lookup"><span data-stu-id="5f088-103">Update localizedNotificationMessage</span></span>

> <span data-ttu-id="5f088-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="5f088-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5f088-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f088-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5f088-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5f088-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f088-107">Aktualisieren der Eigenschaften eines [LocalizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="5f088-107">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5f088-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5f088-108">Prerequisites</span></span>
<span data-ttu-id="5f088-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5f088-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5f088-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5f088-111">Permission type</span></span>|<span data-ttu-id="5f088-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5f088-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f088-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5f088-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5f088-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f088-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5f088-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5f088-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f088-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5f088-116">Not supported.</span></span>|
|<span data-ttu-id="5f088-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5f088-117">Application</span></span>|<span data-ttu-id="5f088-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5f088-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f088-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5f088-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="5f088-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5f088-120">Request headers</span></span>
|<span data-ttu-id="5f088-121">Header</span><span class="sxs-lookup"><span data-stu-id="5f088-121">Header</span></span>|<span data-ttu-id="5f088-122">Wert</span><span class="sxs-lookup"><span data-stu-id="5f088-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f088-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="5f088-123">Authorization</span></span>|<span data-ttu-id="5f088-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5f088-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f088-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5f088-125">Accept</span></span>|<span data-ttu-id="5f088-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5f088-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f088-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5f088-127">Request body</span></span>
<span data-ttu-id="5f088-128">Geben Sie im Anforderungstext eine JSON Darstellung für das [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="5f088-128">In the request body, supply a JSON representation for the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

<span data-ttu-id="5f088-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="5f088-129">The following table shows the properties that are required when you create the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>

|<span data-ttu-id="5f088-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5f088-130">Property</span></span>|<span data-ttu-id="5f088-131">Typ</span><span class="sxs-lookup"><span data-stu-id="5f088-131">Type</span></span>|<span data-ttu-id="5f088-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5f088-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f088-133">id</span><span class="sxs-lookup"><span data-stu-id="5f088-133">id</span></span>|<span data-ttu-id="5f088-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5f088-134">String</span></span>|<span data-ttu-id="5f088-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="5f088-135">Key of the entity.</span></span>|
|<span data-ttu-id="5f088-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5f088-136">lastModifiedDateTime</span></span>|<span data-ttu-id="5f088-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f088-137">DateTimeOffset</span></span>|<span data-ttu-id="5f088-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="5f088-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="5f088-139">Gebietsschema</span><span class="sxs-lookup"><span data-stu-id="5f088-139">locale</span></span>|<span data-ttu-id="5f088-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5f088-140">String</span></span>|<span data-ttu-id="5f088-141">Das Gebietsschema für das diese Nachricht bestimmt ist.</span><span class="sxs-lookup"><span data-stu-id="5f088-141">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="5f088-142">subject</span><span class="sxs-lookup"><span data-stu-id="5f088-142">subject</span></span>|<span data-ttu-id="5f088-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5f088-143">String</span></span>|<span data-ttu-id="5f088-144">Die Vorlage für den Betreff der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="5f088-144">The Message Template Subject.</span></span>|
|<span data-ttu-id="5f088-145">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="5f088-145">messageTemplate</span></span>|<span data-ttu-id="5f088-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5f088-146">String</span></span>|<span data-ttu-id="5f088-147">Die Vorlage für den Inhalt der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="5f088-147">The Message Template content.</span></span>|
|<span data-ttu-id="5f088-148">isDefault</span><span class="sxs-lookup"><span data-stu-id="5f088-148">isDefault</span></span>|<span data-ttu-id="5f088-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f088-149">Boolean</span></span>|<span data-ttu-id="5f088-150">Die Kennzeichnung gibt an, ob dies das Standard-Gebietsschema für die Fallbacksprache ist.</span><span class="sxs-lookup"><span data-stu-id="5f088-150">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="5f088-151">Dieser Kennzeichnung kann nur festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="5f088-151">This flag can only be set.</span></span> <span data-ttu-id="5f088-152">Um die Festlegung aufzuheben, setzen Sie diese Eigenschaft bei einer anderen lokalisierten Benachrichtigung auf „true“.</span><span class="sxs-lookup"><span data-stu-id="5f088-152">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="5f088-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="5f088-153">Response</span></span>
<span data-ttu-id="5f088-154">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5f088-154">If successful, this method returns a `200 OK` response code and an updated [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f088-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5f088-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f088-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5f088-156">Request</span></span>
<span data-ttu-id="5f088-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5f088-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5f088-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="5f088-158">Response</span></span>
<span data-ttu-id="5f088-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5f088-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




