---
title: notificationMessageTemplate erstellen
description: Erstellt neue Objekte des Typs notificationMessageTemplate.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f16d9e679533e56e59393f967b9b192b74f3607b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419821"
---
# <a name="create-notificationmessagetemplate"></a><span data-ttu-id="18bdd-103">notificationMessageTemplate erstellen</span><span class="sxs-lookup"><span data-stu-id="18bdd-103">Create notificationMessageTemplate</span></span>

> <span data-ttu-id="18bdd-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="18bdd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="18bdd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="18bdd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="18bdd-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="18bdd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18bdd-107">Erstellt neue Objekte des Typs [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="18bdd-107">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18bdd-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="18bdd-108">Prerequisites</span></span>
<span data-ttu-id="18bdd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="18bdd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="18bdd-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="18bdd-111">Permission type</span></span>|<span data-ttu-id="18bdd-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="18bdd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18bdd-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="18bdd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="18bdd-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18bdd-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="18bdd-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="18bdd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18bdd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="18bdd-116">Not supported.</span></span>|
|<span data-ttu-id="18bdd-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="18bdd-117">Application</span></span>|<span data-ttu-id="18bdd-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="18bdd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18bdd-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="18bdd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="18bdd-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="18bdd-120">Request headers</span></span>
|<span data-ttu-id="18bdd-121">Header</span><span class="sxs-lookup"><span data-stu-id="18bdd-121">Header</span></span>|<span data-ttu-id="18bdd-122">Wert</span><span class="sxs-lookup"><span data-stu-id="18bdd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18bdd-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="18bdd-123">Authorization</span></span>|<span data-ttu-id="18bdd-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="18bdd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18bdd-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="18bdd-125">Accept</span></span>|<span data-ttu-id="18bdd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="18bdd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18bdd-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="18bdd-127">Request body</span></span>
<span data-ttu-id="18bdd-128">Geben Sie im Anforderungstext eine JSON Darstellung für das notificationMessageTemplate-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="18bdd-128">In the request body, supply a JSON representation for the notificationMessageTemplate object.</span></span>

<span data-ttu-id="18bdd-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der notificationMessageTemplate erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="18bdd-129">The following table shows the properties that are required when you create the notificationMessageTemplate.</span></span>

|<span data-ttu-id="18bdd-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="18bdd-130">Property</span></span>|<span data-ttu-id="18bdd-131">Typ</span><span class="sxs-lookup"><span data-stu-id="18bdd-131">Type</span></span>|<span data-ttu-id="18bdd-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="18bdd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18bdd-133">id</span><span class="sxs-lookup"><span data-stu-id="18bdd-133">id</span></span>|<span data-ttu-id="18bdd-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="18bdd-134">String</span></span>|<span data-ttu-id="18bdd-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="18bdd-135">Key of the entity.</span></span>|
|<span data-ttu-id="18bdd-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="18bdd-136">lastModifiedDateTime</span></span>|<span data-ttu-id="18bdd-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18bdd-137">DateTimeOffset</span></span>|<span data-ttu-id="18bdd-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="18bdd-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="18bdd-139">displayName</span><span class="sxs-lookup"><span data-stu-id="18bdd-139">displayName</span></span>|<span data-ttu-id="18bdd-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="18bdd-140">String</span></span>|<span data-ttu-id="18bdd-141">Anzeigename für die Benachrichtigungs-E-Mail-Vorlage</span><span class="sxs-lookup"><span data-stu-id="18bdd-141">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="18bdd-142">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="18bdd-142">defaultLocale</span></span>|<span data-ttu-id="18bdd-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="18bdd-143">String</span></span>|<span data-ttu-id="18bdd-144">Standardgebietsschema, das verwendet wird, wenn das angeforderte Gebietsschema nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="18bdd-144">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="18bdd-145">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="18bdd-145">brandingOptions</span></span>|[<span data-ttu-id="18bdd-146">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="18bdd-146">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="18bdd-147">Optionen für das Branding der Nachrichtenvorlage.</span><span class="sxs-lookup"><span data-stu-id="18bdd-147">The Message Template Branding Options.</span></span> <span data-ttu-id="18bdd-148">Das Branding wird in der Intune-Verwaltungskonsole definiert.</span><span class="sxs-lookup"><span data-stu-id="18bdd-148">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="18bdd-149">Mögliche Werte sind: `none`, `includeCompanyLogo`, `includeCompanyName` und `includeContactInformation`.</span><span class="sxs-lookup"><span data-stu-id="18bdd-149">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|
|<span data-ttu-id="18bdd-150">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="18bdd-150">roleScopeTagIds</span></span>|<span data-ttu-id="18bdd-151">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="18bdd-151">String collection</span></span>|<span data-ttu-id="18bdd-152">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="18bdd-152">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="18bdd-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="18bdd-153">Response</span></span>
<span data-ttu-id="18bdd-154">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="18bdd-154">If successful, this method returns a `201 Created` response code and a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18bdd-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="18bdd-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="18bdd-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="18bdd-156">Request</span></span>
<span data-ttu-id="18bdd-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="18bdd-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates
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

### <a name="response"></a><span data-ttu-id="18bdd-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="18bdd-158">Response</span></span>
<span data-ttu-id="18bdd-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="18bdd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




