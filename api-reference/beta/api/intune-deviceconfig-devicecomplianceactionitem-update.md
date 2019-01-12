---
title: deviceComplianceActionItem aktualisieren
description: Aktualisieren der Eigenschaften eines deviceComplianceActionItem-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c117c13d9519f3a81bd98096304bc2477ac31933
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942409"
---
# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="9b725-103">deviceComplianceActionItem aktualisieren</span><span class="sxs-lookup"><span data-stu-id="9b725-103">Update deviceComplianceActionItem</span></span>

> <span data-ttu-id="9b725-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9b725-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b725-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9b725-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9b725-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9b725-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9b725-107">Aktualisieren der Eigenschaften eines [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9b725-107">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9b725-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9b725-108">Prerequisites</span></span>
<span data-ttu-id="9b725-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b725-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b725-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9b725-111">Permission type</span></span>|<span data-ttu-id="9b725-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9b725-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b725-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9b725-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9b725-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b725-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9b725-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9b725-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b725-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9b725-116">Not supported.</span></span>|
|<span data-ttu-id="9b725-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9b725-117">Application</span></span>|<span data-ttu-id="9b725-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9b725-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b725-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9b725-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="9b725-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9b725-120">Request headers</span></span>
|<span data-ttu-id="9b725-121">Header</span><span class="sxs-lookup"><span data-stu-id="9b725-121">Header</span></span>|<span data-ttu-id="9b725-122">Wert</span><span class="sxs-lookup"><span data-stu-id="9b725-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b725-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b725-123">Authorization</span></span>|<span data-ttu-id="9b725-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9b725-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b725-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9b725-125">Accept</span></span>|<span data-ttu-id="9b725-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9b725-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b725-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9b725-127">Request body</span></span>
<span data-ttu-id="9b725-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekt des Typs [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) an.</span><span class="sxs-lookup"><span data-stu-id="9b725-128">In the request body, supply a JSON representation for the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="9b725-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="9b725-129">The following table shows the properties that are required when you create the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

|<span data-ttu-id="9b725-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9b725-130">Property</span></span>|<span data-ttu-id="9b725-131">Typ</span><span class="sxs-lookup"><span data-stu-id="9b725-131">Type</span></span>|<span data-ttu-id="9b725-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9b725-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b725-133">id</span><span class="sxs-lookup"><span data-stu-id="9b725-133">id</span></span>|<span data-ttu-id="9b725-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9b725-134">String</span></span>|<span data-ttu-id="9b725-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="9b725-135">Key of the entity.</span></span>|
|<span data-ttu-id="9b725-136">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="9b725-136">gracePeriodHours</span></span>|<span data-ttu-id="9b725-137">Int32</span><span class="sxs-lookup"><span data-stu-id="9b725-137">Int32</span></span>|<span data-ttu-id="9b725-138">Anzahl Stunden, die gewartet wird, bis die Aktion erzwungen wird.</span><span class="sxs-lookup"><span data-stu-id="9b725-138">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="9b725-139">Gültige Werte: 0 bis 8760.</span><span class="sxs-lookup"><span data-stu-id="9b725-139">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="9b725-140">actionType</span><span class="sxs-lookup"><span data-stu-id="9b725-140">actionType</span></span>|[<span data-ttu-id="9b725-141">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="9b725-141">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="9b725-142">Welche Aktion erfolgen soll.</span><span class="sxs-lookup"><span data-stu-id="9b725-142">What action to take.</span></span> <span data-ttu-id="9b725-143">Mögliche Werte sind: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification` und `remoteLock`.</span><span class="sxs-lookup"><span data-stu-id="9b725-143">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="9b725-144">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="9b725-144">notificationTemplateId</span></span>|<span data-ttu-id="9b725-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9b725-145">String</span></span>|<span data-ttu-id="9b725-146">Benachrichtigungs-E-Mail-Vorlage, die verwendet werden soll</span><span class="sxs-lookup"><span data-stu-id="9b725-146">What notification Message template to use</span></span>|
|<span data-ttu-id="9b725-147">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="9b725-147">notificationMessageCCList</span></span>|<span data-ttu-id="9b725-148">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="9b725-148">String collection</span></span>|<span data-ttu-id="9b725-149">Liste der Gruppen-IDs, die festlegt, wer in der Benachrichtigungs-E-Mail in CC gesetzt wird</span><span class="sxs-lookup"><span data-stu-id="9b725-149">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="9b725-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="9b725-150">Response</span></span>
<span data-ttu-id="9b725-151">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9b725-151">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b725-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9b725-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="9b725-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9b725-153">Request</span></span>
<span data-ttu-id="9b725-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9b725-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9b725-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="9b725-155">Response</span></span>
<span data-ttu-id="9b725-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9b725-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





