# <a name="create-notificationmessagetemplate"></a><span data-ttu-id="c1c67-101">notificationMessageTemplate erstellen</span><span class="sxs-lookup"><span data-stu-id="c1c67-101">Create notificationMessageTemplate</span></span>

> <span data-ttu-id="c1c67-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c1c67-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c1c67-103">Erstellt neue Objekte des Typs [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="c1c67-103">Create a new [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c1c67-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c1c67-104">Prerequisites</span></span>
<span data-ttu-id="c1c67-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c1c67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c1c67-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c1c67-107">Permission type</span></span>|<span data-ttu-id="c1c67-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c1c67-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1c67-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c1c67-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c1c67-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1c67-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c1c67-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c1c67-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1c67-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1c67-112">Not supported.</span></span>|
|<span data-ttu-id="c1c67-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c1c67-113">Application</span></span>|<span data-ttu-id="c1c67-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1c67-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1c67-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1c67-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="c1c67-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c1c67-116">Request headers</span></span>
|<span data-ttu-id="c1c67-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c1c67-117">Header</span></span>|<span data-ttu-id="c1c67-118">Wert</span><span class="sxs-lookup"><span data-stu-id="c1c67-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1c67-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1c67-119">Authorization</span></span>|<span data-ttu-id="c1c67-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c1c67-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1c67-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c1c67-121">Accept</span></span>|<span data-ttu-id="c1c67-122">application/json</span><span class="sxs-lookup"><span data-stu-id="c1c67-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1c67-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c1c67-123">Request body</span></span>
<span data-ttu-id="c1c67-124">Geben Sie im Anforderungstext eine JSON Darstellung für das notificationMessageTemplate-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="c1c67-124">In the request body, supply a JSON representation for the notificationMessageTemplate object.</span></span>

<span data-ttu-id="c1c67-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der notificationMessageTemplate erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c1c67-125">The following table shows the properties that are required when you create the notificationMessageTemplate.</span></span>

|<span data-ttu-id="c1c67-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c1c67-126">Property</span></span>|<span data-ttu-id="c1c67-127">Typ</span><span class="sxs-lookup"><span data-stu-id="c1c67-127">Type</span></span>|<span data-ttu-id="c1c67-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c1c67-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1c67-129">id</span><span class="sxs-lookup"><span data-stu-id="c1c67-129">id</span></span>|<span data-ttu-id="c1c67-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1c67-130">String</span></span>|<span data-ttu-id="c1c67-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c1c67-131">Key of the entity.</span></span>|
|<span data-ttu-id="c1c67-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1c67-132">lastModifiedDateTime</span></span>|<span data-ttu-id="c1c67-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1c67-133">DateTimeOffset</span></span>|<span data-ttu-id="c1c67-134">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c1c67-134">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="c1c67-135">displayName</span><span class="sxs-lookup"><span data-stu-id="c1c67-135">displayName</span></span>|<span data-ttu-id="c1c67-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1c67-136">String</span></span>|<span data-ttu-id="c1c67-137">Anzeigename für die Benachrichtigungs-E-Mail-Vorlage</span><span class="sxs-lookup"><span data-stu-id="c1c67-137">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="c1c67-138">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="c1c67-138">defaultLocale</span></span>|<span data-ttu-id="c1c67-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1c67-139">String</span></span>|<span data-ttu-id="c1c67-140">Standardgebietsschema, das verwendet wird, wenn das angeforderte Gebietsschema nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="c1c67-140">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="c1c67-141">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="c1c67-141">brandingOptions</span></span>|[<span data-ttu-id="c1c67-142">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="c1c67-142">notificationTemplateBrandingOptions</span></span>](../resources/intune_notification_notificationtemplatebrandingoptions.md)|<span data-ttu-id="c1c67-143">Optionen für das Branding der Nachrichtenvorlage.</span><span class="sxs-lookup"><span data-stu-id="c1c67-143">The Message Template Branding Options.</span></span> <span data-ttu-id="c1c67-144">Das Branding wird in der Intune-Verwaltungskonsole definiert.</span><span class="sxs-lookup"><span data-stu-id="c1c67-144">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="c1c67-145">Mögliche Werte: `none`, `includeCompanyLogo`, `includeCompanyName` und `includeContactInformation`.</span><span class="sxs-lookup"><span data-stu-id="c1c67-145">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|



## <a name="response"></a><span data-ttu-id="c1c67-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1c67-146">Response</span></span>
<span data-ttu-id="c1c67-147">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c1c67-147">If successful, this method returns a `201 Created` response code and a [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1c67-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c1c67-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="c1c67-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1c67-149">Request</span></span>
<span data-ttu-id="c1c67-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c1c67-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c1c67-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1c67-151">Response</span></span>
<span data-ttu-id="c1c67-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c1c67-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



