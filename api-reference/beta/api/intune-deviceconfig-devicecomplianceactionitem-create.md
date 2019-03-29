---
title: Erstellen von „deviceComplianceActionItem“
description: Diese Methode erstellt ein neues Objekt des Typs deviceComplianceActionItem.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1b7bd39bb8def5404081dde1034e758de58340f0
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30976715"
---
# <a name="create-devicecomplianceactionitem"></a><span data-ttu-id="82c4b-103">Erstellen von „deviceComplianceActionItem“</span><span class="sxs-lookup"><span data-stu-id="82c4b-103">Create deviceComplianceActionItem</span></span>

> <span data-ttu-id="82c4b-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="82c4b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82c4b-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="82c4b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82c4b-106">Diese Methode erstellt ein neues Objekt des Typs [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="82c4b-106">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82c4b-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="82c4b-107">Prerequisites</span></span>
<span data-ttu-id="82c4b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82c4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82c4b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="82c4b-110">Permission type</span></span>|<span data-ttu-id="82c4b-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="82c4b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82c4b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="82c4b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="82c4b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82c4b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="82c4b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="82c4b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82c4b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="82c4b-115">Not supported.</span></span>|
|<span data-ttu-id="82c4b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="82c4b-116">Application</span></span>|<span data-ttu-id="82c4b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="82c4b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82c4b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="82c4b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="82c4b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="82c4b-119">Request headers</span></span>
|<span data-ttu-id="82c4b-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="82c4b-120">Header</span></span>|<span data-ttu-id="82c4b-121">Wert</span><span class="sxs-lookup"><span data-stu-id="82c4b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82c4b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="82c4b-122">Authorization</span></span>|<span data-ttu-id="82c4b-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="82c4b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82c4b-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="82c4b-124">Accept</span></span>|<span data-ttu-id="82c4b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="82c4b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82c4b-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="82c4b-126">Request body</span></span>
<span data-ttu-id="82c4b-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekt des Typs „deviceComplianceActionItem“ an.</span><span class="sxs-lookup"><span data-stu-id="82c4b-127">In the request body, supply a JSON representation for the deviceComplianceActionItem object.</span></span>

<span data-ttu-id="82c4b-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceComplianceActionItem“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="82c4b-128">The following table shows the properties that are required when you create the deviceComplianceActionItem.</span></span>

|<span data-ttu-id="82c4b-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="82c4b-129">Property</span></span>|<span data-ttu-id="82c4b-130">Typ</span><span class="sxs-lookup"><span data-stu-id="82c4b-130">Type</span></span>|<span data-ttu-id="82c4b-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="82c4b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82c4b-132">id</span><span class="sxs-lookup"><span data-stu-id="82c4b-132">id</span></span>|<span data-ttu-id="82c4b-133">String</span><span class="sxs-lookup"><span data-stu-id="82c4b-133">String</span></span>|<span data-ttu-id="82c4b-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="82c4b-134">Key of the entity.</span></span>|
|<span data-ttu-id="82c4b-135">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="82c4b-135">gracePeriodHours</span></span>|<span data-ttu-id="82c4b-136">Int32</span><span class="sxs-lookup"><span data-stu-id="82c4b-136">Int32</span></span>|<span data-ttu-id="82c4b-137">Die Anzahl der Stunden, bis die Aktion erzwungen wird.</span><span class="sxs-lookup"><span data-stu-id="82c4b-137">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="82c4b-138">Gültige Werte: 0 bis 8760</span><span class="sxs-lookup"><span data-stu-id="82c4b-138">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="82c4b-139">actionType</span><span class="sxs-lookup"><span data-stu-id="82c4b-139">actionType</span></span>|[<span data-ttu-id="82c4b-140">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="82c4b-140">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="82c4b-141">Welche Aktion ergriffen werden soll.</span><span class="sxs-lookup"><span data-stu-id="82c4b-141">What action to take.</span></span> <span data-ttu-id="82c4b-142">Mögliche Werte: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span><span class="sxs-lookup"><span data-stu-id="82c4b-142">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="82c4b-143">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="82c4b-143">notificationTemplateId</span></span>|<span data-ttu-id="82c4b-144">String</span><span class="sxs-lookup"><span data-stu-id="82c4b-144">String</span></span>|<span data-ttu-id="82c4b-145">Auswahl der verwendeten Benachrichtigungsvorlage</span><span class="sxs-lookup"><span data-stu-id="82c4b-145">What notification Message template to use</span></span>|
|<span data-ttu-id="82c4b-146">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="82c4b-146">notificationMessageCCList</span></span>|<span data-ttu-id="82c4b-147">String collection</span><span class="sxs-lookup"><span data-stu-id="82c4b-147">String collection</span></span>|<span data-ttu-id="82c4b-148">Liste der Gruppen-IDs, die festlegt, wer in der Benachrichtigungs-E-Mail in CC gesetzt wird</span><span class="sxs-lookup"><span data-stu-id="82c4b-148">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="82c4b-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="82c4b-149">Response</span></span>
<span data-ttu-id="82c4b-150">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="82c4b-150">If successful, this method returns a `201 Created` response code and a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82c4b-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="82c4b-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="82c4b-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="82c4b-152">Request</span></span>
<span data-ttu-id="82c4b-153">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="82c4b-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="82c4b-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="82c4b-154">Response</span></span>
<span data-ttu-id="82c4b-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="82c4b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




