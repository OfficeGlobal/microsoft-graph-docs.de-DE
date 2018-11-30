---
title: deviceComplianceActionItem aktualisieren
description: Aktualisieren der Eigenschaften eines deviceComplianceActionItem-Objekts.
ms.openlocfilehash: 0f2d94411c88bf4e7d377150ebd59d3056b1f6c7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059271"
---
# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="51d53-103">deviceComplianceActionItem aktualisieren</span><span class="sxs-lookup"><span data-stu-id="51d53-103">Update deviceComplianceActionItem</span></span>

> <span data-ttu-id="51d53-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="51d53-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51d53-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="51d53-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="51d53-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="51d53-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51d53-107">Aktualisieren der Eigenschaften eines [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="51d53-107">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="51d53-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="51d53-108">Prerequisites</span></span>
<span data-ttu-id="51d53-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51d53-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51d53-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="51d53-111">Permission type</span></span>|<span data-ttu-id="51d53-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="51d53-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51d53-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="51d53-113">Delegated (work or school account)</span></span>|<span data-ttu-id="51d53-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51d53-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="51d53-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="51d53-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51d53-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="51d53-116">Not supported.</span></span>|
|<span data-ttu-id="51d53-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="51d53-117">Application</span></span>|<span data-ttu-id="51d53-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="51d53-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51d53-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="51d53-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="51d53-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="51d53-120">Request headers</span></span>
|<span data-ttu-id="51d53-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="51d53-121">Header</span></span>|<span data-ttu-id="51d53-122">Wert</span><span class="sxs-lookup"><span data-stu-id="51d53-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51d53-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="51d53-123">Authorization</span></span>|<span data-ttu-id="51d53-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="51d53-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51d53-125">Accept</span><span class="sxs-lookup"><span data-stu-id="51d53-125">Accept</span></span>|<span data-ttu-id="51d53-126">application/json</span><span class="sxs-lookup"><span data-stu-id="51d53-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51d53-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="51d53-127">Request body</span></span>
<span data-ttu-id="51d53-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekt des Typs [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) an.</span><span class="sxs-lookup"><span data-stu-id="51d53-128">In the request body, supply a JSON representation for the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="51d53-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="51d53-129">The following table shows the properties that are required when you create the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

|<span data-ttu-id="51d53-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="51d53-130">Property</span></span>|<span data-ttu-id="51d53-131">Typ</span><span class="sxs-lookup"><span data-stu-id="51d53-131">Type</span></span>|<span data-ttu-id="51d53-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="51d53-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51d53-133">id</span><span class="sxs-lookup"><span data-stu-id="51d53-133">id</span></span>|<span data-ttu-id="51d53-134">String</span><span class="sxs-lookup"><span data-stu-id="51d53-134">String</span></span>|<span data-ttu-id="51d53-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="51d53-135">Key of the entity.</span></span>|
|<span data-ttu-id="51d53-136">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="51d53-136">gracePeriodHours</span></span>|<span data-ttu-id="51d53-137">Int32</span><span class="sxs-lookup"><span data-stu-id="51d53-137">Int32</span></span>|<span data-ttu-id="51d53-138">Anzahl Stunden, die gewartet wird, bis die Aktion erzwungen wird.</span><span class="sxs-lookup"><span data-stu-id="51d53-138">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="51d53-139">Gültige Werte: 0 bis 8760.</span><span class="sxs-lookup"><span data-stu-id="51d53-139">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="51d53-140">actionType</span><span class="sxs-lookup"><span data-stu-id="51d53-140">actionType</span></span>|[<span data-ttu-id="51d53-141">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="51d53-141">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="51d53-142">Welche Aktion erfolgen soll.</span><span class="sxs-lookup"><span data-stu-id="51d53-142">What action to take.</span></span> <span data-ttu-id="51d53-143">Mögliche Werte sind: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification` und `remoteLock`.</span><span class="sxs-lookup"><span data-stu-id="51d53-143">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="51d53-144">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="51d53-144">notificationTemplateId</span></span>|<span data-ttu-id="51d53-145">String</span><span class="sxs-lookup"><span data-stu-id="51d53-145">String</span></span>|<span data-ttu-id="51d53-146">Benachrichtigungs-E-Mail-Vorlage, die verwendet werden soll</span><span class="sxs-lookup"><span data-stu-id="51d53-146">What notification Message template to use</span></span>|
|<span data-ttu-id="51d53-147">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="51d53-147">notificationMessageCCList</span></span>|<span data-ttu-id="51d53-148">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="51d53-148">String collection</span></span>|<span data-ttu-id="51d53-149">Liste der Gruppen-IDs, die festlegt, wer in der Benachrichtigungs-E-Mail in CC gesetzt wird</span><span class="sxs-lookup"><span data-stu-id="51d53-149">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="51d53-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="51d53-150">Response</span></span>
<span data-ttu-id="51d53-151">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="51d53-151">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51d53-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="51d53-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="51d53-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="51d53-153">Request</span></span>
<span data-ttu-id="51d53-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="51d53-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
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

### <a name="response"></a><span data-ttu-id="51d53-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="51d53-155">Response</span></span>
<span data-ttu-id="51d53-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="51d53-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





