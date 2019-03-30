---
title: Erstellen von „deviceComplianceActionItem“
description: Diese Methode erstellt ein neues Objekt des Typs deviceComplianceActionItem.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dca5374dcb75e93667454389f0104861bb9f1d7c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988147"
---
# <a name="create-devicecomplianceactionitem"></a><span data-ttu-id="867da-103">Erstellen von „deviceComplianceActionItem“</span><span class="sxs-lookup"><span data-stu-id="867da-103">Create deviceComplianceActionItem</span></span>

> <span data-ttu-id="867da-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="867da-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="867da-105">Diese Methode erstellt ein neues Objekt des Typs [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="867da-105">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="867da-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="867da-106">Prerequisites</span></span>
<span data-ttu-id="867da-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="867da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="867da-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="867da-109">Permission type</span></span>|<span data-ttu-id="867da-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="867da-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="867da-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="867da-111">Delegated (work or school account)</span></span>|<span data-ttu-id="867da-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="867da-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="867da-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="867da-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="867da-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="867da-114">Not supported.</span></span>|
|<span data-ttu-id="867da-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="867da-115">Application</span></span>|<span data-ttu-id="867da-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="867da-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="867da-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="867da-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="867da-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="867da-118">Request headers</span></span>
|<span data-ttu-id="867da-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="867da-119">Header</span></span>|<span data-ttu-id="867da-120">Wert</span><span class="sxs-lookup"><span data-stu-id="867da-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="867da-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="867da-121">Authorization</span></span>|<span data-ttu-id="867da-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="867da-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="867da-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="867da-123">Accept</span></span>|<span data-ttu-id="867da-124">application/json</span><span class="sxs-lookup"><span data-stu-id="867da-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="867da-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="867da-125">Request body</span></span>
<span data-ttu-id="867da-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekt des Typs „deviceComplianceActionItem“ an.</span><span class="sxs-lookup"><span data-stu-id="867da-126">In the request body, supply a JSON representation for the deviceComplianceActionItem object.</span></span>

<span data-ttu-id="867da-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceComplianceActionItem“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="867da-127">The following table shows the properties that are required when you create the deviceComplianceActionItem.</span></span>

|<span data-ttu-id="867da-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="867da-128">Property</span></span>|<span data-ttu-id="867da-129">Typ</span><span class="sxs-lookup"><span data-stu-id="867da-129">Type</span></span>|<span data-ttu-id="867da-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="867da-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="867da-131">id</span><span class="sxs-lookup"><span data-stu-id="867da-131">id</span></span>|<span data-ttu-id="867da-132">String</span><span class="sxs-lookup"><span data-stu-id="867da-132">String</span></span>|<span data-ttu-id="867da-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="867da-133">Key of the entity.</span></span>|
|<span data-ttu-id="867da-134">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="867da-134">gracePeriodHours</span></span>|<span data-ttu-id="867da-135">Int32</span><span class="sxs-lookup"><span data-stu-id="867da-135">Int32</span></span>|<span data-ttu-id="867da-136">Die Anzahl der Stunden, bis die Aktion erzwungen wird.</span><span class="sxs-lookup"><span data-stu-id="867da-136">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="867da-137">Gültige Werte: 0 bis 8760</span><span class="sxs-lookup"><span data-stu-id="867da-137">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="867da-138">actionType</span><span class="sxs-lookup"><span data-stu-id="867da-138">actionType</span></span>|[<span data-ttu-id="867da-139">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="867da-139">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="867da-140">Welche Aktion ergriffen werden soll.</span><span class="sxs-lookup"><span data-stu-id="867da-140">What action to take.</span></span> <span data-ttu-id="867da-141">Mögliche Werte: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span><span class="sxs-lookup"><span data-stu-id="867da-141">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span></span>|
|<span data-ttu-id="867da-142">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="867da-142">notificationTemplateId</span></span>|<span data-ttu-id="867da-143">String</span><span class="sxs-lookup"><span data-stu-id="867da-143">String</span></span>|<span data-ttu-id="867da-144">Auswahl der verwendeten Benachrichtigungsvorlage</span><span class="sxs-lookup"><span data-stu-id="867da-144">What notification Message template to use</span></span>|
|<span data-ttu-id="867da-145">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="867da-145">notificationMessageCCList</span></span>|<span data-ttu-id="867da-146">String collection</span><span class="sxs-lookup"><span data-stu-id="867da-146">String collection</span></span>|<span data-ttu-id="867da-147">Liste der Gruppen-IDs, die festlegt, wer in der Benachrichtigungs-E-Mail in CC gesetzt wird</span><span class="sxs-lookup"><span data-stu-id="867da-147">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="867da-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="867da-148">Response</span></span>
<span data-ttu-id="867da-149">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="867da-149">If successful, this method returns a `201 Created` response code and a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="867da-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="867da-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="867da-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="867da-151">Request</span></span>
<span data-ttu-id="867da-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="867da-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="867da-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="867da-153">Response</span></span>
<span data-ttu-id="867da-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="867da-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



