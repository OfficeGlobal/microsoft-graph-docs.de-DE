---
title: notificationMessageTemplate aktualisieren
description: Aktualisiert die Eigenschaften von Objekten des Typs notificationMessageTemplate.
author: tfitzmac
ms.openlocfilehash: 02c431370560dc9785e682bc7307ee530ae1d4fd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357358"
---
# <a name="update-notificationmessagetemplate"></a><span data-ttu-id="a8f7e-103">notificationMessageTemplate aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a8f7e-103">Update notificationMessageTemplate</span></span>

> <span data-ttu-id="a8f7e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a8f7e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8f7e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a8f7e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a8f7e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a8f7e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8f7e-107">Aktualisiert die Eigenschaften von Objekten des Typs [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="a8f7e-107">Update the properties of a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a8f7e-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a8f7e-108">Prerequisites</span></span>
<span data-ttu-id="a8f7e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8f7e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8f7e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a8f7e-111">Permission type</span></span>|<span data-ttu-id="a8f7e-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a8f7e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8f7e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a8f7e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a8f7e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8f7e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a8f7e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a8f7e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8f7e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a8f7e-116">Not supported.</span></span>|
|<span data-ttu-id="a8f7e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a8f7e-117">Application</span></span>|<span data-ttu-id="a8f7e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a8f7e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8f7e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a8f7e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="a8f7e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a8f7e-120">Request headers</span></span>
|<span data-ttu-id="a8f7e-121">Header</span><span class="sxs-lookup"><span data-stu-id="a8f7e-121">Header</span></span>|<span data-ttu-id="a8f7e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="a8f7e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8f7e-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="a8f7e-123">Authorization</span></span>|<span data-ttu-id="a8f7e-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a8f7e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8f7e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a8f7e-125">Accept</span></span>|<span data-ttu-id="a8f7e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a8f7e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8f7e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a8f7e-127">Request body</span></span>
<span data-ttu-id="a8f7e-128">Geben Sie im Anforderungstext eine JSON Darstellung für das [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="a8f7e-128">In the request body, supply a JSON representation for the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

<span data-ttu-id="a8f7e-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="a8f7e-129">The following table shows the properties that are required when you create the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>

|<span data-ttu-id="a8f7e-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a8f7e-130">Property</span></span>|<span data-ttu-id="a8f7e-131">Typ</span><span class="sxs-lookup"><span data-stu-id="a8f7e-131">Type</span></span>|<span data-ttu-id="a8f7e-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a8f7e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8f7e-133">id</span><span class="sxs-lookup"><span data-stu-id="a8f7e-133">id</span></span>|<span data-ttu-id="a8f7e-134">String</span><span class="sxs-lookup"><span data-stu-id="a8f7e-134">String</span></span>|<span data-ttu-id="a8f7e-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a8f7e-135">Key of the entity.</span></span>|
|<span data-ttu-id="a8f7e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a8f7e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a8f7e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8f7e-137">DateTimeOffset</span></span>|<span data-ttu-id="a8f7e-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a8f7e-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="a8f7e-139">displayName</span><span class="sxs-lookup"><span data-stu-id="a8f7e-139">displayName</span></span>|<span data-ttu-id="a8f7e-140">String</span><span class="sxs-lookup"><span data-stu-id="a8f7e-140">String</span></span>|<span data-ttu-id="a8f7e-141">Anzeigename für die Benachrichtigungs-E-Mail-Vorlage</span><span class="sxs-lookup"><span data-stu-id="a8f7e-141">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="a8f7e-142">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="a8f7e-142">defaultLocale</span></span>|<span data-ttu-id="a8f7e-143">String</span><span class="sxs-lookup"><span data-stu-id="a8f7e-143">String</span></span>|<span data-ttu-id="a8f7e-144">Standardgebietsschema, das verwendet wird, wenn das angeforderte Gebietsschema nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="a8f7e-144">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="a8f7e-145">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="a8f7e-145">brandingOptions</span></span>|[<span data-ttu-id="a8f7e-146">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="a8f7e-146">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="a8f7e-147">Optionen für das Branding der Nachrichtenvorlage.</span><span class="sxs-lookup"><span data-stu-id="a8f7e-147">The Message Template Branding Options.</span></span> <span data-ttu-id="a8f7e-148">Das Branding wird in der Intune-Verwaltungskonsole definiert.</span><span class="sxs-lookup"><span data-stu-id="a8f7e-148">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="a8f7e-149">Mögliche Werte sind: `none`, `includeCompanyLogo`, `includeCompanyName` und `includeContactInformation`.</span><span class="sxs-lookup"><span data-stu-id="a8f7e-149">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|
|<span data-ttu-id="a8f7e-150">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a8f7e-150">roleScopeTagIds</span></span>|<span data-ttu-id="a8f7e-151">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="a8f7e-151">String collection</span></span>|<span data-ttu-id="a8f7e-152">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="a8f7e-152">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="a8f7e-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="a8f7e-153">Response</span></span>
<span data-ttu-id="a8f7e-154">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a8f7e-154">If successful, this method returns a `200 OK` response code and an updated [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8f7e-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a8f7e-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="a8f7e-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a8f7e-156">Request</span></span>
<span data-ttu-id="a8f7e-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a8f7e-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
Content-type: application/json
Content-length: 257

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="a8f7e-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="a8f7e-158">Response</span></span>
<span data-ttu-id="a8f7e-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a8f7e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





