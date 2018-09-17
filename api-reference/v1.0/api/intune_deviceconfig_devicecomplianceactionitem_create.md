# <a name="create-devicecomplianceactionitem"></a><span data-ttu-id="77661-101">Erstellen von „deviceComplianceActionItem“</span><span class="sxs-lookup"><span data-stu-id="77661-101">Create deviceComplianceActionItem</span></span>

> <span data-ttu-id="77661-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="77661-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="77661-103">Diese Methode erstellt ein neues Objekt des Typs [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="77661-103">Create a new [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="77661-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="77661-104">Prerequisites</span></span>
<span data-ttu-id="77661-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="77661-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="77661-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="77661-107">Permission type</span></span>|<span data-ttu-id="77661-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="77661-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77661-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="77661-109">Delegated (work or school account)</span></span>|<span data-ttu-id="77661-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77661-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="77661-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="77661-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77661-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="77661-112">Not supported.</span></span>|
|<span data-ttu-id="77661-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="77661-113">Application</span></span>|<span data-ttu-id="77661-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="77661-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77661-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="77661-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="77661-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="77661-116">Request headers</span></span>
|<span data-ttu-id="77661-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="77661-117">Header</span></span>|<span data-ttu-id="77661-118">Wert</span><span class="sxs-lookup"><span data-stu-id="77661-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77661-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="77661-119">Authorization</span></span>|<span data-ttu-id="77661-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="77661-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77661-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="77661-121">Accept</span></span>|<span data-ttu-id="77661-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="77661-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77661-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="77661-123">Request body</span></span>
<span data-ttu-id="77661-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekt des Typs „deviceComplianceActionItem“ an.</span><span class="sxs-lookup"><span data-stu-id="77661-124">In the request body, supply a JSON representation for the deviceComplianceActionItem object.</span></span>

<span data-ttu-id="77661-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceComplianceActionItem“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="77661-125">The following table shows the properties that are required when you create the deviceComplianceActionItem.</span></span>

|<span data-ttu-id="77661-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="77661-126">Property</span></span>|<span data-ttu-id="77661-127">Typ</span><span class="sxs-lookup"><span data-stu-id="77661-127">Type</span></span>|<span data-ttu-id="77661-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77661-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77661-129">ID</span><span class="sxs-lookup"><span data-stu-id="77661-129">id</span></span>|<span data-ttu-id="77661-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="77661-130">String</span></span>|<span data-ttu-id="77661-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="77661-131">Key of the entity.</span></span>|
|<span data-ttu-id="77661-132">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="77661-132">gracePeriodHours</span></span>|<span data-ttu-id="77661-133">Int32</span><span class="sxs-lookup"><span data-stu-id="77661-133">Int32</span></span>|<span data-ttu-id="77661-134">Anzahl Stunden, die gewartet wird, bis die Aktion erzwungen wird.</span><span class="sxs-lookup"><span data-stu-id="77661-134">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="77661-135">Gültige Werte: 0 bis 8760.</span><span class="sxs-lookup"><span data-stu-id="77661-135">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="77661-136">actionType</span><span class="sxs-lookup"><span data-stu-id="77661-136">actionType</span></span>|[<span data-ttu-id="77661-137">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="77661-137">deviceComplianceActionType</span></span>](../resources/intune_deviceconfig_devicecomplianceactiontype.md)|<span data-ttu-id="77661-138">Zu ergreifende Maßnahme.</span><span class="sxs-lookup"><span data-stu-id="77661-138">What action to take.</span></span> <span data-ttu-id="77661-139">Mögliche Werte sind: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles` und `pushNotification`.</span><span class="sxs-lookup"><span data-stu-id="77661-139">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span></span>|
|<span data-ttu-id="77661-140">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="77661-140">notificationTemplateId</span></span>|<span data-ttu-id="77661-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="77661-141">String</span></span>|<span data-ttu-id="77661-142">Benachrichtigungs-E-Mail-Vorlage, die verwendet werden soll</span><span class="sxs-lookup"><span data-stu-id="77661-142">What notification Message template to use</span></span>|
|<span data-ttu-id="77661-143">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="77661-143">notificationMessageCCList</span></span>|<span data-ttu-id="77661-144">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="77661-144">String collection</span></span>|<span data-ttu-id="77661-145">Liste der Gruppen-IDs, die festlegt, wer in der Benachrichtigungs-E-Mail in CC gesetzt wird</span><span class="sxs-lookup"><span data-stu-id="77661-145">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="77661-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="77661-146">Response</span></span>
<span data-ttu-id="77661-147">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="77661-147">If successful, this method returns a `201 Created` response code and a [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77661-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="77661-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="77661-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="77661-149">Request</span></span>
<span data-ttu-id="77661-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="77661-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
Content-type: application/json
Content-length: 271

{
  "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
  "gracePeriodHours": 0,
  "actionType": "notification",
  "notificationTemplateId": "Notification Template Id value",
  "notificationMessageCCList": [
    "Notification Message CCList value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="77661-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="77661-151">Response</span></span>
<span data-ttu-id="77661-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="77661-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 320

{
  "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
  "id": "e01a1893-1893-e01a-9318-1ae093181ae0",
  "gracePeriodHours": 0,
  "actionType": "notification",
  "notificationTemplateId": "Notification Template Id value",
  "notificationMessageCCList": [
    "Notification Message CCList value"
  ]
}
```








