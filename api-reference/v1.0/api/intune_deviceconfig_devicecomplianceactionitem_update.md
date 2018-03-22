# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="babe5-101">deviceComplianceActionItem aktualisieren</span><span class="sxs-lookup"><span data-stu-id="babe5-101">Update deviceComplianceActionItem</span></span>

> <span data-ttu-id="babe5-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="babe5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="babe5-103">Aktualisieren der Eigenschaften eines [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="babe5-103">Update the properties of a [calendar](../resources/intune_deviceconfig_devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="babe5-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="babe5-104">Prerequisites</span></span>
<span data-ttu-id="babe5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="babe5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="babe5-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="babe5-107">Permission type</span></span>|<span data-ttu-id="babe5-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="babe5-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="babe5-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="babe5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="babe5-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="babe5-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="babe5-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="babe5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="babe5-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="babe5-112">Not supported.</span></span>|
|<span data-ttu-id="babe5-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="babe5-113">Application</span></span>|<span data-ttu-id="babe5-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="babe5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="babe5-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="babe5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="babe5-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="babe5-116">Request headers</span></span>
|<span data-ttu-id="babe5-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="babe5-117">Header</span></span>|<span data-ttu-id="babe5-118">Wert</span><span class="sxs-lookup"><span data-stu-id="babe5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="babe5-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="babe5-119">Authorization</span></span>|<span data-ttu-id="babe5-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="babe5-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="babe5-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="babe5-121">Accept</span></span>|<span data-ttu-id="babe5-122">application/json</span><span class="sxs-lookup"><span data-stu-id="babe5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="babe5-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="babe5-123">Request body</span></span>
<span data-ttu-id="babe5-124">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekt des Typs [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) an.</span><span class="sxs-lookup"><span data-stu-id="babe5-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="babe5-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="babe5-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="babe5-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="babe5-126">Property</span></span>|<span data-ttu-id="babe5-127">Typ</span><span class="sxs-lookup"><span data-stu-id="babe5-127">Type</span></span>|<span data-ttu-id="babe5-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="babe5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="babe5-129">id</span><span class="sxs-lookup"><span data-stu-id="babe5-129">id</span></span>|<span data-ttu-id="babe5-130">String</span><span class="sxs-lookup"><span data-stu-id="babe5-130">String</span></span>|<span data-ttu-id="babe5-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="babe5-131">Key of the setting.</span></span>|
|<span data-ttu-id="babe5-132">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="babe5-132">gracePeriodHours</span></span>|<span data-ttu-id="babe5-133">Int32</span><span class="sxs-lookup"><span data-stu-id="babe5-133">Int32</span></span>|<span data-ttu-id="babe5-134">Die Anzahl der Stunden, bis die Aktion erzwungen wird.</span><span class="sxs-lookup"><span data-stu-id="babe5-134">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="babe5-135">Gültige Werte: 0 bis 8760</span><span class="sxs-lookup"><span data-stu-id="babe5-135">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="babe5-136">actionType</span><span class="sxs-lookup"><span data-stu-id="babe5-136">actionType</span></span>|<span data-ttu-id="babe5-137">String</span><span class="sxs-lookup"><span data-stu-id="babe5-137">String</span></span>|<span data-ttu-id="babe5-138">Mögliche Werte für den Aktionstyp: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`.</span><span class="sxs-lookup"><span data-stu-id="babe5-138">What action to take Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`.</span></span>|
|<span data-ttu-id="babe5-139">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="babe5-139">notificationTemplateId</span></span>|<span data-ttu-id="babe5-140">String</span><span class="sxs-lookup"><span data-stu-id="babe5-140">String</span></span>|<span data-ttu-id="babe5-141">Auswahl der verwendeten Benachrichtigungsvorlage</span><span class="sxs-lookup"><span data-stu-id="babe5-141">What notification Message template to use</span></span>|
|<span data-ttu-id="babe5-142">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="babe5-142">notificationMessageCCList</span></span>|<span data-ttu-id="babe5-143">String collection</span><span class="sxs-lookup"><span data-stu-id="babe5-143">String collection</span></span>|<span data-ttu-id="babe5-144">Liste der Gruppen-IDs, die festlegt, wer in der Benachrichtigungs-E-Mail in CC gesetzt wird</span><span class="sxs-lookup"><span data-stu-id="babe5-144">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="babe5-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="babe5-145">Response</span></span>
<span data-ttu-id="babe5-146">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="babe5-146">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="babe5-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="babe5-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="babe5-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="babe5-148">Request</span></span>
<span data-ttu-id="babe5-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="babe5-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
Content-type: application/json
Content-length: 206

{
  "gracePeriodHours": 0,
  "actionType": "notification",
  "notificationTemplateId": "Notification Template Id value",
  "notificationMessageCCList": [
    "Notification Message CCList value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="babe5-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="babe5-150">Response</span></span>
<span data-ttu-id="babe5-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="babe5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



