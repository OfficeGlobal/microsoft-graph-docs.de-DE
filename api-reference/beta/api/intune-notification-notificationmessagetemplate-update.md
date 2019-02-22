---
title: notificationMessageTemplate aktualisieren
description: Aktualisiert die Eigenschaften von Objekten des Typs notificationMessageTemplate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4705a42db30e527933651aa0c85422ec4b3bcf38
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153921"
---
# <a name="update-notificationmessagetemplate"></a><span data-ttu-id="105f9-103">notificationMessageTemplate aktualisieren</span><span class="sxs-lookup"><span data-stu-id="105f9-103">Update notificationMessageTemplate</span></span>

> <span data-ttu-id="105f9-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="105f9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="105f9-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="105f9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="105f9-106">Aktualisiert die Eigenschaften von Objekten des Typs [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="105f9-106">Update the properties of a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="105f9-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="105f9-107">Prerequisites</span></span>
<span data-ttu-id="105f9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="105f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="105f9-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="105f9-110">Permission type</span></span>|<span data-ttu-id="105f9-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="105f9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="105f9-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="105f9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="105f9-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="105f9-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="105f9-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="105f9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="105f9-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="105f9-115">Not supported.</span></span>|
|<span data-ttu-id="105f9-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="105f9-116">Application</span></span>|<span data-ttu-id="105f9-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="105f9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="105f9-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="105f9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="105f9-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="105f9-119">Request headers</span></span>
|<span data-ttu-id="105f9-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="105f9-120">Header</span></span>|<span data-ttu-id="105f9-121">Wert</span><span class="sxs-lookup"><span data-stu-id="105f9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="105f9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="105f9-122">Authorization</span></span>|<span data-ttu-id="105f9-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="105f9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="105f9-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="105f9-124">Accept</span></span>|<span data-ttu-id="105f9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="105f9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="105f9-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="105f9-126">Request body</span></span>
<span data-ttu-id="105f9-127">Geben Sie im Anforderungstext eine JSON Darstellung für das [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="105f9-127">In the request body, supply a JSON representation for the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

<span data-ttu-id="105f9-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="105f9-128">The following table shows the properties that are required when you create the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>

|<span data-ttu-id="105f9-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="105f9-129">Property</span></span>|<span data-ttu-id="105f9-130">Typ</span><span class="sxs-lookup"><span data-stu-id="105f9-130">Type</span></span>|<span data-ttu-id="105f9-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="105f9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="105f9-132">id</span><span class="sxs-lookup"><span data-stu-id="105f9-132">id</span></span>|<span data-ttu-id="105f9-133">String</span><span class="sxs-lookup"><span data-stu-id="105f9-133">String</span></span>|<span data-ttu-id="105f9-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="105f9-134">Key of the entity.</span></span>|
|<span data-ttu-id="105f9-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="105f9-135">lastModifiedDateTime</span></span>|<span data-ttu-id="105f9-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="105f9-136">DateTimeOffset</span></span>|<span data-ttu-id="105f9-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="105f9-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="105f9-138">displayName</span><span class="sxs-lookup"><span data-stu-id="105f9-138">displayName</span></span>|<span data-ttu-id="105f9-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="105f9-139">String</span></span>|<span data-ttu-id="105f9-140">Anzeigename für die Benachrichtigungs-E-Mail-Vorlage</span><span class="sxs-lookup"><span data-stu-id="105f9-140">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="105f9-141">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="105f9-141">defaultLocale</span></span>|<span data-ttu-id="105f9-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="105f9-142">String</span></span>|<span data-ttu-id="105f9-143">Standardgebietsschema, das verwendet wird, wenn das angeforderte Gebietsschema nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="105f9-143">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="105f9-144">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="105f9-144">brandingOptions</span></span>|[<span data-ttu-id="105f9-145">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="105f9-145">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="105f9-146">Optionen für das Branding der Nachrichtenvorlage.</span><span class="sxs-lookup"><span data-stu-id="105f9-146">The Message Template Branding Options.</span></span> <span data-ttu-id="105f9-147">Das Branding wird in der Intune-Verwaltungskonsole definiert.</span><span class="sxs-lookup"><span data-stu-id="105f9-147">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="105f9-148">Mögliche Werte sind: `none`, `includeCompanyLogo`, `includeCompanyName` und `includeContactInformation`.</span><span class="sxs-lookup"><span data-stu-id="105f9-148">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|
|<span data-ttu-id="105f9-149">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="105f9-149">roleScopeTagIds</span></span>|<span data-ttu-id="105f9-150">String collection</span><span class="sxs-lookup"><span data-stu-id="105f9-150">String collection</span></span>|<span data-ttu-id="105f9-151">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="105f9-151">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="105f9-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="105f9-152">Response</span></span>
<span data-ttu-id="105f9-153">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="105f9-153">If successful, this method returns a `200 OK` response code and an updated [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="105f9-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="105f9-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="105f9-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="105f9-155">Request</span></span>
<span data-ttu-id="105f9-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="105f9-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
Content-type: application/json
Content-length: 259

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="105f9-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="105f9-157">Response</span></span>
<span data-ttu-id="105f9-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="105f9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 372

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "id": "e1db399b-399b-e1db-9b39-dbe19b39dbe1",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




