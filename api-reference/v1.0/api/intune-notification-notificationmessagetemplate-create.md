---
title: notificationMessageTemplate erstellen
description: Erstellt neue Objekte des Typs notificationMessageTemplate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6a79dc797bd91ea58ea6997d18d789c0e6c6e297
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250257"
---
# <a name="create-notificationmessagetemplate"></a><span data-ttu-id="f7ef7-103">notificationMessageTemplate erstellen</span><span class="sxs-lookup"><span data-stu-id="f7ef7-103">Create notificationMessageTemplate</span></span>

> <span data-ttu-id="f7ef7-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f7ef7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7ef7-105">Erstellt neue Objekte des Typs [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="f7ef7-105">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7ef7-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f7ef7-106">Prerequisites</span></span>
<span data-ttu-id="f7ef7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f7ef7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f7ef7-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f7ef7-109">Permission type</span></span>|<span data-ttu-id="f7ef7-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f7ef7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7ef7-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f7ef7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f7ef7-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7ef7-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f7ef7-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f7ef7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7ef7-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f7ef7-114">Not supported.</span></span>|
|<span data-ttu-id="f7ef7-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f7ef7-115">Application</span></span>|<span data-ttu-id="f7ef7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f7ef7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7ef7-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f7ef7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="f7ef7-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f7ef7-118">Request headers</span></span>
|<span data-ttu-id="f7ef7-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f7ef7-119">Header</span></span>|<span data-ttu-id="f7ef7-120">Wert</span><span class="sxs-lookup"><span data-stu-id="f7ef7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7ef7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7ef7-121">Authorization</span></span>|<span data-ttu-id="f7ef7-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f7ef7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7ef7-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f7ef7-123">Accept</span></span>|<span data-ttu-id="f7ef7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f7ef7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7ef7-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f7ef7-125">Request body</span></span>
<span data-ttu-id="f7ef7-126">Geben Sie im Anforderungstext eine JSON Darstellung für das notificationMessageTemplate-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="f7ef7-126">In the request body, supply a JSON representation for the notificationMessageTemplate object.</span></span>

<span data-ttu-id="f7ef7-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der notificationMessageTemplate erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="f7ef7-127">The following table shows the properties that are required when you create the notificationMessageTemplate.</span></span>

|<span data-ttu-id="f7ef7-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f7ef7-128">Property</span></span>|<span data-ttu-id="f7ef7-129">Typ</span><span class="sxs-lookup"><span data-stu-id="f7ef7-129">Type</span></span>|<span data-ttu-id="f7ef7-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f7ef7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7ef7-131">id</span><span class="sxs-lookup"><span data-stu-id="f7ef7-131">id</span></span>|<span data-ttu-id="f7ef7-132">String</span><span class="sxs-lookup"><span data-stu-id="f7ef7-132">String</span></span>|<span data-ttu-id="f7ef7-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f7ef7-133">Key of the entity.</span></span>|
|<span data-ttu-id="f7ef7-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f7ef7-134">lastModifiedDateTime</span></span>|<span data-ttu-id="f7ef7-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7ef7-135">DateTimeOffset</span></span>|<span data-ttu-id="f7ef7-136">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f7ef7-136">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="f7ef7-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f7ef7-137">displayName</span></span>|<span data-ttu-id="f7ef7-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f7ef7-138">String</span></span>|<span data-ttu-id="f7ef7-139">Anzeigename für die Benachrichtigungs-E-Mail-Vorlage</span><span class="sxs-lookup"><span data-stu-id="f7ef7-139">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="f7ef7-140">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="f7ef7-140">defaultLocale</span></span>|<span data-ttu-id="f7ef7-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f7ef7-141">String</span></span>|<span data-ttu-id="f7ef7-142">Standardgebietsschema, das verwendet wird, wenn das angeforderte Gebietsschema nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="f7ef7-142">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="f7ef7-143">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="f7ef7-143">brandingOptions</span></span>|[<span data-ttu-id="f7ef7-144">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="f7ef7-144">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="f7ef7-145">Optionen für das Branding der Nachrichtenvorlage.</span><span class="sxs-lookup"><span data-stu-id="f7ef7-145">The Message Template Branding Options.</span></span> <span data-ttu-id="f7ef7-146">Das Branding wird in der Intune-Verwaltungskonsole definiert.</span><span class="sxs-lookup"><span data-stu-id="f7ef7-146">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="f7ef7-147">Mögliche Werte sind: `none`, `includeCompanyLogo`, `includeCompanyName` und `includeContactInformation`.</span><span class="sxs-lookup"><span data-stu-id="f7ef7-147">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|



## <a name="response"></a><span data-ttu-id="f7ef7-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="f7ef7-148">Response</span></span>
<span data-ttu-id="f7ef7-149">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f7ef7-149">If successful, this method returns a `201 Created` response code and a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7ef7-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f7ef7-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7ef7-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f7ef7-151">Request</span></span>
<span data-ttu-id="f7ef7-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f7ef7-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates
Content-type: application/json
Content-length: 197

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo"
}
```

### <a name="response"></a><span data-ttu-id="f7ef7-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="f7ef7-153">Response</span></span>
<span data-ttu-id="f7ef7-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f7ef7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 310

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "id": "e1db399b-399b-e1db-9b39-dbe19b39dbe1",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo"
}
```



