---
title: deviceComplianceActionItem aktualisieren
description: Aktualisieren der Eigenschaften eines deviceComplianceActionItem-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5da502820ccf13b0494a6914811db698ff8abc65
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254023"
---
# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="637ac-103">deviceComplianceActionItem aktualisieren</span><span class="sxs-lookup"><span data-stu-id="637ac-103">Update deviceComplianceActionItem</span></span>

> <span data-ttu-id="637ac-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="637ac-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="637ac-105">Aktualisieren der Eigenschaften eines [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="637ac-105">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="637ac-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="637ac-106">Prerequisites</span></span>
<span data-ttu-id="637ac-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="637ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="637ac-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="637ac-109">Permission type</span></span>|<span data-ttu-id="637ac-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="637ac-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="637ac-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="637ac-111">Delegated (work or school account)</span></span>|<span data-ttu-id="637ac-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="637ac-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="637ac-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="637ac-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="637ac-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="637ac-114">Not supported.</span></span>|
|<span data-ttu-id="637ac-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="637ac-115">Application</span></span>|<span data-ttu-id="637ac-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="637ac-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="637ac-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="637ac-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="637ac-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="637ac-118">Request headers</span></span>
|<span data-ttu-id="637ac-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="637ac-119">Header</span></span>|<span data-ttu-id="637ac-120">Wert</span><span class="sxs-lookup"><span data-stu-id="637ac-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="637ac-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="637ac-121">Authorization</span></span>|<span data-ttu-id="637ac-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="637ac-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="637ac-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="637ac-123">Accept</span></span>|<span data-ttu-id="637ac-124">application/json</span><span class="sxs-lookup"><span data-stu-id="637ac-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="637ac-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="637ac-125">Request body</span></span>
<span data-ttu-id="637ac-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekt des Typs [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) an.</span><span class="sxs-lookup"><span data-stu-id="637ac-126">In the request body, supply a JSON representation for the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="637ac-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="637ac-127">The following table shows the properties that are required when you create the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

|<span data-ttu-id="637ac-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="637ac-128">Property</span></span>|<span data-ttu-id="637ac-129">Typ</span><span class="sxs-lookup"><span data-stu-id="637ac-129">Type</span></span>|<span data-ttu-id="637ac-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="637ac-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="637ac-131">id</span><span class="sxs-lookup"><span data-stu-id="637ac-131">id</span></span>|<span data-ttu-id="637ac-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="637ac-132">String</span></span>|<span data-ttu-id="637ac-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="637ac-133">Key of the entity.</span></span>|
|<span data-ttu-id="637ac-134">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="637ac-134">gracePeriodHours</span></span>|<span data-ttu-id="637ac-135">Int32</span><span class="sxs-lookup"><span data-stu-id="637ac-135">Int32</span></span>|<span data-ttu-id="637ac-136">Anzahl Stunden, die gewartet wird, bis die Aktion erzwungen wird.</span><span class="sxs-lookup"><span data-stu-id="637ac-136">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="637ac-137">Gültige Werte: 0 bis 8760.</span><span class="sxs-lookup"><span data-stu-id="637ac-137">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="637ac-138">actionType</span><span class="sxs-lookup"><span data-stu-id="637ac-138">actionType</span></span>|[<span data-ttu-id="637ac-139">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="637ac-139">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="637ac-140">Welche Aktion ergriffen werden soll.</span><span class="sxs-lookup"><span data-stu-id="637ac-140">What action to take.</span></span> <span data-ttu-id="637ac-141">Mögliche Werte sind: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles` und `pushNotification`.</span><span class="sxs-lookup"><span data-stu-id="637ac-141">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span></span>|
|<span data-ttu-id="637ac-142">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="637ac-142">notificationTemplateId</span></span>|<span data-ttu-id="637ac-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="637ac-143">String</span></span>|<span data-ttu-id="637ac-144">Benachrichtigungs-E-Mail-Vorlage, die verwendet werden soll</span><span class="sxs-lookup"><span data-stu-id="637ac-144">What notification Message template to use</span></span>|
|<span data-ttu-id="637ac-145">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="637ac-145">notificationMessageCCList</span></span>|<span data-ttu-id="637ac-146">String collection</span><span class="sxs-lookup"><span data-stu-id="637ac-146">String collection</span></span>|<span data-ttu-id="637ac-147">Liste der Gruppen-IDs, die festlegt, wer in der Benachrichtigungs-E-Mail in CC gesetzt wird</span><span class="sxs-lookup"><span data-stu-id="637ac-147">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="637ac-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="637ac-148">Response</span></span>
<span data-ttu-id="637ac-149">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="637ac-149">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="637ac-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="637ac-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="637ac-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="637ac-151">Request</span></span>
<span data-ttu-id="637ac-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="637ac-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
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

### <a name="response"></a><span data-ttu-id="637ac-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="637ac-153">Response</span></span>
<span data-ttu-id="637ac-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="637ac-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



