---
title: deviceComplianceActionItem aktualisieren
description: Aktualisieren der Eigenschaften eines deviceComplianceActionItem-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 028b8365cd30a39f34dc0cc4dac9867bd122ac07
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979704"
---
# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="46115-103">deviceComplianceActionItem aktualisieren</span><span class="sxs-lookup"><span data-stu-id="46115-103">Update deviceComplianceActionItem</span></span>

> <span data-ttu-id="46115-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="46115-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46115-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="46115-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46115-106">Aktualisieren der Eigenschaften eines [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="46115-106">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46115-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="46115-107">Prerequisites</span></span>
<span data-ttu-id="46115-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46115-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46115-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="46115-110">Permission type</span></span>|<span data-ttu-id="46115-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="46115-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46115-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="46115-112">Delegated (work or school account)</span></span>|<span data-ttu-id="46115-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46115-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="46115-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="46115-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46115-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="46115-115">Not supported.</span></span>|
|<span data-ttu-id="46115-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="46115-116">Application</span></span>|<span data-ttu-id="46115-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="46115-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46115-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="46115-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="46115-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="46115-119">Request headers</span></span>
|<span data-ttu-id="46115-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="46115-120">Header</span></span>|<span data-ttu-id="46115-121">Wert</span><span class="sxs-lookup"><span data-stu-id="46115-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46115-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="46115-122">Authorization</span></span>|<span data-ttu-id="46115-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="46115-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46115-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="46115-124">Accept</span></span>|<span data-ttu-id="46115-125">application/json</span><span class="sxs-lookup"><span data-stu-id="46115-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46115-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="46115-126">Request body</span></span>
<span data-ttu-id="46115-127">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekt des Typs [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) an.</span><span class="sxs-lookup"><span data-stu-id="46115-127">In the request body, supply a JSON representation for the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="46115-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="46115-128">The following table shows the properties that are required when you create the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

|<span data-ttu-id="46115-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="46115-129">Property</span></span>|<span data-ttu-id="46115-130">Typ</span><span class="sxs-lookup"><span data-stu-id="46115-130">Type</span></span>|<span data-ttu-id="46115-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="46115-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46115-132">id</span><span class="sxs-lookup"><span data-stu-id="46115-132">id</span></span>|<span data-ttu-id="46115-133">String</span><span class="sxs-lookup"><span data-stu-id="46115-133">String</span></span>|<span data-ttu-id="46115-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="46115-134">Key of the entity.</span></span>|
|<span data-ttu-id="46115-135">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="46115-135">gracePeriodHours</span></span>|<span data-ttu-id="46115-136">Int32</span><span class="sxs-lookup"><span data-stu-id="46115-136">Int32</span></span>|<span data-ttu-id="46115-137">Die Anzahl der Stunden, bis die Aktion erzwungen wird.</span><span class="sxs-lookup"><span data-stu-id="46115-137">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="46115-138">Gültige Werte: 0 bis 8760</span><span class="sxs-lookup"><span data-stu-id="46115-138">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="46115-139">actionType</span><span class="sxs-lookup"><span data-stu-id="46115-139">actionType</span></span>|[<span data-ttu-id="46115-140">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="46115-140">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="46115-141">Welche Aktion ergriffen werden soll.</span><span class="sxs-lookup"><span data-stu-id="46115-141">What action to take.</span></span> <span data-ttu-id="46115-142">Mögliche Werte: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span><span class="sxs-lookup"><span data-stu-id="46115-142">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="46115-143">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="46115-143">notificationTemplateId</span></span>|<span data-ttu-id="46115-144">String</span><span class="sxs-lookup"><span data-stu-id="46115-144">String</span></span>|<span data-ttu-id="46115-145">Auswahl der verwendeten Benachrichtigungsvorlage</span><span class="sxs-lookup"><span data-stu-id="46115-145">What notification Message template to use</span></span>|
|<span data-ttu-id="46115-146">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="46115-146">notificationMessageCCList</span></span>|<span data-ttu-id="46115-147">String collection</span><span class="sxs-lookup"><span data-stu-id="46115-147">String collection</span></span>|<span data-ttu-id="46115-148">Liste der Gruppen-IDs, die festlegt, wer in der Benachrichtigungs-E-Mail in CC gesetzt wird</span><span class="sxs-lookup"><span data-stu-id="46115-148">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="46115-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="46115-149">Response</span></span>
<span data-ttu-id="46115-150">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="46115-150">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46115-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="46115-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="46115-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="46115-152">Request</span></span>
<span data-ttu-id="46115-153">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="46115-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
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

### <a name="response"></a><span data-ttu-id="46115-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="46115-154">Response</span></span>
<span data-ttu-id="46115-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="46115-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




