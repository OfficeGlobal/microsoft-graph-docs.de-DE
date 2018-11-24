# <a name="create-localizednotificationmessage"></a><span data-ttu-id="143a9-101">localizedNotificationMessage erstellen</span><span class="sxs-lookup"><span data-stu-id="143a9-101">Create localizedNotificationMessage</span></span>

> <span data-ttu-id="143a9-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="143a9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="143a9-103">Erstellen eines neuen [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="143a9-103">Create a new [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="143a9-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="143a9-104">Prerequisites</span></span>
<span data-ttu-id="143a9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="143a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="143a9-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="143a9-107">Permission type</span></span>|<span data-ttu-id="143a9-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="143a9-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="143a9-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="143a9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="143a9-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="143a9-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="143a9-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="143a9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="143a9-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="143a9-112">Not supported.</span></span>|
|<span data-ttu-id="143a9-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="143a9-113">Application</span></span>|<span data-ttu-id="143a9-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="143a9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="143a9-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="143a9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="143a9-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="143a9-116">Request headers</span></span>
|<span data-ttu-id="143a9-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="143a9-117">Header</span></span>|<span data-ttu-id="143a9-118">Wert</span><span class="sxs-lookup"><span data-stu-id="143a9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="143a9-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="143a9-119">Authorization</span></span>|<span data-ttu-id="143a9-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="143a9-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="143a9-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="143a9-121">Accept</span></span>|<span data-ttu-id="143a9-122">application/json</span><span class="sxs-lookup"><span data-stu-id="143a9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="143a9-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="143a9-123">Request body</span></span>
<span data-ttu-id="143a9-124">Geben Sie im Anforderungstext eine JSON Darstellung für das localizedNotificationMessage-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="143a9-124">In the request body, supply a JSON representation for the localizedNotificationMessage object.</span></span>

<span data-ttu-id="143a9-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der localizedNotificationMessage erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="143a9-125">The following table shows the properties that are required when you create the localizedNotificationMessage.</span></span>

|<span data-ttu-id="143a9-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="143a9-126">Property</span></span>|<span data-ttu-id="143a9-127">Typ</span><span class="sxs-lookup"><span data-stu-id="143a9-127">Type</span></span>|<span data-ttu-id="143a9-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="143a9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="143a9-129">id</span><span class="sxs-lookup"><span data-stu-id="143a9-129">id</span></span>|<span data-ttu-id="143a9-130">String</span><span class="sxs-lookup"><span data-stu-id="143a9-130">String</span></span>|<span data-ttu-id="143a9-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="143a9-131">Key of the entity.</span></span>|
|<span data-ttu-id="143a9-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="143a9-132">lastModifiedDateTime</span></span>|<span data-ttu-id="143a9-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="143a9-133">DateTimeOffset</span></span>|<span data-ttu-id="143a9-134">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="143a9-134">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="143a9-135">Gebietsschema</span><span class="sxs-lookup"><span data-stu-id="143a9-135">locale</span></span>|<span data-ttu-id="143a9-136">String</span><span class="sxs-lookup"><span data-stu-id="143a9-136">String</span></span>|<span data-ttu-id="143a9-137">Das Gebietsschema für das diese Nachricht bestimmt ist.</span><span class="sxs-lookup"><span data-stu-id="143a9-137">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="143a9-138">Betreff</span><span class="sxs-lookup"><span data-stu-id="143a9-138">subject</span></span>|<span data-ttu-id="143a9-139">String</span><span class="sxs-lookup"><span data-stu-id="143a9-139">String</span></span>|<span data-ttu-id="143a9-140">Die Vorlage für den Betreff der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="143a9-140">The Message Template Subject.</span></span>|
|<span data-ttu-id="143a9-141">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="143a9-141">messageTemplate</span></span>|<span data-ttu-id="143a9-142">String</span><span class="sxs-lookup"><span data-stu-id="143a9-142">String</span></span>|<span data-ttu-id="143a9-143">Die Vorlage für den Inhalt der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="143a9-143">The Message Template content.</span></span>|
|<span data-ttu-id="143a9-144">isDefault</span><span class="sxs-lookup"><span data-stu-id="143a9-144">isDefault</span></span>|<span data-ttu-id="143a9-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="143a9-145">Boolean</span></span>|<span data-ttu-id="143a9-146">Die Kennzeichnung gibt an, ob dies das Standard-Gebietsschema für die Fallbacksprache ist.</span><span class="sxs-lookup"><span data-stu-id="143a9-146">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="143a9-147">Dieser Kennzeichnung kann nur festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="143a9-147">This flag can only be set.</span></span> <span data-ttu-id="143a9-148">Um die Festlegung aufzuheben, setzen Sie diese Eigenschaft bei einer anderen lokalisierten Benachrichtigung auf „true“.</span><span class="sxs-lookup"><span data-stu-id="143a9-148">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="143a9-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="143a9-149">Response</span></span>
<span data-ttu-id="143a9-150">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="143a9-150">If successful, this method returns a `201 Created` response code and a [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="143a9-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="143a9-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="143a9-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="143a9-152">Request</span></span>
<span data-ttu-id="143a9-153">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="143a9-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="143a9-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="143a9-154">Response</span></span>
<span data-ttu-id="143a9-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="143a9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



