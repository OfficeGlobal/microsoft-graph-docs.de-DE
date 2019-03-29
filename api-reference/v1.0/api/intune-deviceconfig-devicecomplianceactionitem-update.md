---
title: deviceComplianceActionItem aktualisieren
description: Aktualisieren der Eigenschaften eines deviceComplianceActionItem-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 814f37faf8596b63c05993b93596f807f7e744e0
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30976113"
---
# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="de537-103">deviceComplianceActionItem aktualisieren</span><span class="sxs-lookup"><span data-stu-id="de537-103">Update deviceComplianceActionItem</span></span>

> <span data-ttu-id="de537-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="de537-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de537-105">Aktualisieren der Eigenschaften eines [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="de537-105">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de537-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="de537-106">Prerequisites</span></span>
<span data-ttu-id="de537-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de537-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de537-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="de537-109">Permission type</span></span>|<span data-ttu-id="de537-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="de537-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de537-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="de537-111">Delegated (work or school account)</span></span>|<span data-ttu-id="de537-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de537-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="de537-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="de537-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de537-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="de537-114">Not supported.</span></span>|
|<span data-ttu-id="de537-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="de537-115">Application</span></span>|<span data-ttu-id="de537-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="de537-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de537-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="de537-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="de537-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="de537-118">Request headers</span></span>
|<span data-ttu-id="de537-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="de537-119">Header</span></span>|<span data-ttu-id="de537-120">Wert</span><span class="sxs-lookup"><span data-stu-id="de537-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de537-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="de537-121">Authorization</span></span>|<span data-ttu-id="de537-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="de537-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de537-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="de537-123">Accept</span></span>|<span data-ttu-id="de537-124">application/json</span><span class="sxs-lookup"><span data-stu-id="de537-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de537-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="de537-125">Request body</span></span>
<span data-ttu-id="de537-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekt des Typs [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) an.</span><span class="sxs-lookup"><span data-stu-id="de537-126">In the request body, supply a JSON representation for the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="de537-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="de537-127">The following table shows the properties that are required when you create the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

|<span data-ttu-id="de537-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="de537-128">Property</span></span>|<span data-ttu-id="de537-129">Typ</span><span class="sxs-lookup"><span data-stu-id="de537-129">Type</span></span>|<span data-ttu-id="de537-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="de537-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de537-131">id</span><span class="sxs-lookup"><span data-stu-id="de537-131">id</span></span>|<span data-ttu-id="de537-132">String</span><span class="sxs-lookup"><span data-stu-id="de537-132">String</span></span>|<span data-ttu-id="de537-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="de537-133">Key of the entity.</span></span>|
|<span data-ttu-id="de537-134">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="de537-134">gracePeriodHours</span></span>|<span data-ttu-id="de537-135">Int32</span><span class="sxs-lookup"><span data-stu-id="de537-135">Int32</span></span>|<span data-ttu-id="de537-136">Die Anzahl der Stunden, bis die Aktion erzwungen wird.</span><span class="sxs-lookup"><span data-stu-id="de537-136">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="de537-137">Gültige Werte: 0 bis 8760</span><span class="sxs-lookup"><span data-stu-id="de537-137">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="de537-138">actionType</span><span class="sxs-lookup"><span data-stu-id="de537-138">actionType</span></span>|[<span data-ttu-id="de537-139">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="de537-139">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="de537-140">Welche Aktion ergriffen werden soll.</span><span class="sxs-lookup"><span data-stu-id="de537-140">What action to take.</span></span> <span data-ttu-id="de537-141">Mögliche Werte: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span><span class="sxs-lookup"><span data-stu-id="de537-141">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span></span>|
|<span data-ttu-id="de537-142">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="de537-142">notificationTemplateId</span></span>|<span data-ttu-id="de537-143">String</span><span class="sxs-lookup"><span data-stu-id="de537-143">String</span></span>|<span data-ttu-id="de537-144">Auswahl der verwendeten Benachrichtigungsvorlage</span><span class="sxs-lookup"><span data-stu-id="de537-144">What notification Message template to use</span></span>|
|<span data-ttu-id="de537-145">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="de537-145">notificationMessageCCList</span></span>|<span data-ttu-id="de537-146">String collection</span><span class="sxs-lookup"><span data-stu-id="de537-146">String collection</span></span>|<span data-ttu-id="de537-147">Liste der Gruppen-IDs, die festlegt, wer in der Benachrichtigungs-E-Mail in CC gesetzt wird</span><span class="sxs-lookup"><span data-stu-id="de537-147">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="de537-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="de537-148">Response</span></span>
<span data-ttu-id="de537-149">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="de537-149">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de537-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="de537-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="de537-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="de537-151">Request</span></span>
<span data-ttu-id="de537-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="de537-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="de537-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="de537-153">Response</span></span>
<span data-ttu-id="de537-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="de537-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



