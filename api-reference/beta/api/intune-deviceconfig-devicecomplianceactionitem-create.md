---
title: Erstellen von „deviceComplianceActionItem“
description: Diese Methode erstellt ein neues Objekt des Typs deviceComplianceActionItem.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 282babf1cf567752885858bbb397977b095a7a34
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873612"
---
# <a name="create-devicecomplianceactionitem"></a><span data-ttu-id="46a22-103">Erstellen von „deviceComplianceActionItem“</span><span class="sxs-lookup"><span data-stu-id="46a22-103">Create deviceComplianceActionItem</span></span>

> <span data-ttu-id="46a22-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="46a22-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="46a22-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="46a22-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="46a22-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="46a22-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="46a22-107">Diese Methode erstellt ein neues Objekt des Typs [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="46a22-107">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="46a22-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="46a22-108">Prerequisites</span></span>
<span data-ttu-id="46a22-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46a22-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46a22-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="46a22-111">Permission type</span></span>|<span data-ttu-id="46a22-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="46a22-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46a22-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="46a22-113">Delegated (work or school account)</span></span>|<span data-ttu-id="46a22-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46a22-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="46a22-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="46a22-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46a22-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="46a22-116">Not supported.</span></span>|
|<span data-ttu-id="46a22-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="46a22-117">Application</span></span>|<span data-ttu-id="46a22-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="46a22-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46a22-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="46a22-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="46a22-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="46a22-120">Request headers</span></span>
|<span data-ttu-id="46a22-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="46a22-121">Header</span></span>|<span data-ttu-id="46a22-122">Wert</span><span class="sxs-lookup"><span data-stu-id="46a22-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46a22-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="46a22-123">Authorization</span></span>|<span data-ttu-id="46a22-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="46a22-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46a22-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="46a22-125">Accept</span></span>|<span data-ttu-id="46a22-126">application/json</span><span class="sxs-lookup"><span data-stu-id="46a22-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46a22-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="46a22-127">Request body</span></span>
<span data-ttu-id="46a22-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekt des Typs „deviceComplianceActionItem“ an.</span><span class="sxs-lookup"><span data-stu-id="46a22-128">In the request body, supply a JSON representation for the deviceComplianceActionItem object.</span></span>

<span data-ttu-id="46a22-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceComplianceActionItem“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="46a22-129">The following table shows the properties that are required when you create the deviceComplianceActionItem.</span></span>

|<span data-ttu-id="46a22-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="46a22-130">Property</span></span>|<span data-ttu-id="46a22-131">Typ</span><span class="sxs-lookup"><span data-stu-id="46a22-131">Type</span></span>|<span data-ttu-id="46a22-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="46a22-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46a22-133">id</span><span class="sxs-lookup"><span data-stu-id="46a22-133">id</span></span>|<span data-ttu-id="46a22-134">String</span><span class="sxs-lookup"><span data-stu-id="46a22-134">String</span></span>|<span data-ttu-id="46a22-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="46a22-135">Key of the entity.</span></span>|
|<span data-ttu-id="46a22-136">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="46a22-136">gracePeriodHours</span></span>|<span data-ttu-id="46a22-137">Int32</span><span class="sxs-lookup"><span data-stu-id="46a22-137">Int32</span></span>|<span data-ttu-id="46a22-138">Anzahl Stunden, die gewartet wird, bis die Aktion erzwungen wird.</span><span class="sxs-lookup"><span data-stu-id="46a22-138">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="46a22-139">Gültige Werte: 0 bis 8760.</span><span class="sxs-lookup"><span data-stu-id="46a22-139">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="46a22-140">actionType</span><span class="sxs-lookup"><span data-stu-id="46a22-140">actionType</span></span>|[<span data-ttu-id="46a22-141">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="46a22-141">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="46a22-142">Welche Aktion erfolgen soll.</span><span class="sxs-lookup"><span data-stu-id="46a22-142">What action to take.</span></span> <span data-ttu-id="46a22-143">Mögliche Werte sind: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification` und `remoteLock`.</span><span class="sxs-lookup"><span data-stu-id="46a22-143">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="46a22-144">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="46a22-144">notificationTemplateId</span></span>|<span data-ttu-id="46a22-145">String</span><span class="sxs-lookup"><span data-stu-id="46a22-145">String</span></span>|<span data-ttu-id="46a22-146">Benachrichtigungs-E-Mail-Vorlage, die verwendet werden soll</span><span class="sxs-lookup"><span data-stu-id="46a22-146">What notification Message template to use</span></span>|
|<span data-ttu-id="46a22-147">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="46a22-147">notificationMessageCCList</span></span>|<span data-ttu-id="46a22-148">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="46a22-148">String collection</span></span>|<span data-ttu-id="46a22-149">Liste der Gruppen-IDs, die festlegt, wer in der Benachrichtigungs-E-Mail in CC gesetzt wird</span><span class="sxs-lookup"><span data-stu-id="46a22-149">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="46a22-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="46a22-150">Response</span></span>
<span data-ttu-id="46a22-151">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="46a22-151">If successful, this method returns a `201 Created` response code and a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46a22-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="46a22-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="46a22-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="46a22-153">Request</span></span>
<span data-ttu-id="46a22-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="46a22-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
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

### <a name="response"></a><span data-ttu-id="46a22-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="46a22-155">Response</span></span>
<span data-ttu-id="46a22-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="46a22-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





