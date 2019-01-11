---
title: deviceComplianceActionItem aktualisieren
description: Aktualisieren der Eigenschaften eines deviceComplianceActionItem-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6502980f1bbb5474fd1805ea9d8ec7365befd130
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841972"
---
# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="31a35-103">deviceComplianceActionItem aktualisieren</span><span class="sxs-lookup"><span data-stu-id="31a35-103">Update deviceComplianceActionItem</span></span>

> <span data-ttu-id="31a35-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="31a35-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31a35-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="31a35-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="31a35-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="31a35-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="31a35-107">Aktualisieren der Eigenschaften eines [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="31a35-107">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="31a35-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="31a35-108">Prerequisites</span></span>
<span data-ttu-id="31a35-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31a35-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31a35-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="31a35-111">Permission type</span></span>|<span data-ttu-id="31a35-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="31a35-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31a35-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="31a35-113">Delegated (work or school account)</span></span>|<span data-ttu-id="31a35-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31a35-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="31a35-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="31a35-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31a35-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="31a35-116">Not supported.</span></span>|
|<span data-ttu-id="31a35-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="31a35-117">Application</span></span>|<span data-ttu-id="31a35-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="31a35-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="31a35-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="31a35-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="31a35-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="31a35-120">Request headers</span></span>
|<span data-ttu-id="31a35-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="31a35-121">Header</span></span>|<span data-ttu-id="31a35-122">Wert</span><span class="sxs-lookup"><span data-stu-id="31a35-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31a35-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="31a35-123">Authorization</span></span>|<span data-ttu-id="31a35-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="31a35-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31a35-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="31a35-125">Accept</span></span>|<span data-ttu-id="31a35-126">application/json</span><span class="sxs-lookup"><span data-stu-id="31a35-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31a35-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="31a35-127">Request body</span></span>
<span data-ttu-id="31a35-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekt des Typs [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) an.</span><span class="sxs-lookup"><span data-stu-id="31a35-128">In the request body, supply a JSON representation for the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="31a35-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="31a35-129">The following table shows the properties that are required when you create the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

|<span data-ttu-id="31a35-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="31a35-130">Property</span></span>|<span data-ttu-id="31a35-131">Typ</span><span class="sxs-lookup"><span data-stu-id="31a35-131">Type</span></span>|<span data-ttu-id="31a35-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="31a35-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31a35-133">id</span><span class="sxs-lookup"><span data-stu-id="31a35-133">id</span></span>|<span data-ttu-id="31a35-134">String</span><span class="sxs-lookup"><span data-stu-id="31a35-134">String</span></span>|<span data-ttu-id="31a35-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="31a35-135">Key of the entity.</span></span>|
|<span data-ttu-id="31a35-136">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="31a35-136">gracePeriodHours</span></span>|<span data-ttu-id="31a35-137">Int32</span><span class="sxs-lookup"><span data-stu-id="31a35-137">Int32</span></span>|<span data-ttu-id="31a35-138">Anzahl Stunden, die gewartet wird, bis die Aktion erzwungen wird.</span><span class="sxs-lookup"><span data-stu-id="31a35-138">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="31a35-139">Gültige Werte: 0 bis 8760.</span><span class="sxs-lookup"><span data-stu-id="31a35-139">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="31a35-140">actionType</span><span class="sxs-lookup"><span data-stu-id="31a35-140">actionType</span></span>|[<span data-ttu-id="31a35-141">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="31a35-141">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="31a35-142">Welche Aktion erfolgen soll.</span><span class="sxs-lookup"><span data-stu-id="31a35-142">What action to take.</span></span> <span data-ttu-id="31a35-143">Mögliche Werte sind: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification` und `remoteLock`.</span><span class="sxs-lookup"><span data-stu-id="31a35-143">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="31a35-144">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="31a35-144">notificationTemplateId</span></span>|<span data-ttu-id="31a35-145">String</span><span class="sxs-lookup"><span data-stu-id="31a35-145">String</span></span>|<span data-ttu-id="31a35-146">Benachrichtigungs-E-Mail-Vorlage, die verwendet werden soll</span><span class="sxs-lookup"><span data-stu-id="31a35-146">What notification Message template to use</span></span>|
|<span data-ttu-id="31a35-147">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="31a35-147">notificationMessageCCList</span></span>|<span data-ttu-id="31a35-148">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="31a35-148">String collection</span></span>|<span data-ttu-id="31a35-149">Liste der Gruppen-IDs, die festlegt, wer in der Benachrichtigungs-E-Mail in CC gesetzt wird</span><span class="sxs-lookup"><span data-stu-id="31a35-149">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="31a35-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="31a35-150">Response</span></span>
<span data-ttu-id="31a35-151">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="31a35-151">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31a35-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="31a35-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="31a35-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="31a35-153">Request</span></span>
<span data-ttu-id="31a35-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="31a35-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="31a35-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="31a35-155">Response</span></span>
<span data-ttu-id="31a35-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="31a35-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





