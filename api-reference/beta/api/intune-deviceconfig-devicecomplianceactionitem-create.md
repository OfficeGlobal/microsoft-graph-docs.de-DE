---
title: Erstellen von „deviceComplianceActionItem“
description: Diese Methode erstellt ein neues Objekt des Typs deviceComplianceActionItem.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5e538bd064c2d590eeb743e2c2dea05abc869900
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421579"
---
# <a name="create-devicecomplianceactionitem"></a><span data-ttu-id="15759-103">Erstellen von „deviceComplianceActionItem“</span><span class="sxs-lookup"><span data-stu-id="15759-103">Create deviceComplianceActionItem</span></span>

> <span data-ttu-id="15759-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="15759-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="15759-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="15759-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15759-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="15759-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15759-107">Diese Methode erstellt ein neues Objekt des Typs [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="15759-107">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15759-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="15759-108">Prerequisites</span></span>
<span data-ttu-id="15759-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="15759-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="15759-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="15759-111">Permission type</span></span>|<span data-ttu-id="15759-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="15759-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15759-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="15759-113">Delegated (work or school account)</span></span>|<span data-ttu-id="15759-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15759-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="15759-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="15759-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15759-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="15759-116">Not supported.</span></span>|
|<span data-ttu-id="15759-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="15759-117">Application</span></span>|<span data-ttu-id="15759-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="15759-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15759-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="15759-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="15759-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="15759-120">Request headers</span></span>
|<span data-ttu-id="15759-121">Header</span><span class="sxs-lookup"><span data-stu-id="15759-121">Header</span></span>|<span data-ttu-id="15759-122">Wert</span><span class="sxs-lookup"><span data-stu-id="15759-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15759-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="15759-123">Authorization</span></span>|<span data-ttu-id="15759-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="15759-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15759-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="15759-125">Accept</span></span>|<span data-ttu-id="15759-126">application/json</span><span class="sxs-lookup"><span data-stu-id="15759-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15759-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="15759-127">Request body</span></span>
<span data-ttu-id="15759-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekt des Typs „deviceComplianceActionItem“ an.</span><span class="sxs-lookup"><span data-stu-id="15759-128">In the request body, supply a JSON representation for the deviceComplianceActionItem object.</span></span>

<span data-ttu-id="15759-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceComplianceActionItem“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="15759-129">The following table shows the properties that are required when you create the deviceComplianceActionItem.</span></span>

|<span data-ttu-id="15759-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="15759-130">Property</span></span>|<span data-ttu-id="15759-131">Typ</span><span class="sxs-lookup"><span data-stu-id="15759-131">Type</span></span>|<span data-ttu-id="15759-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="15759-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15759-133">id</span><span class="sxs-lookup"><span data-stu-id="15759-133">id</span></span>|<span data-ttu-id="15759-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15759-134">String</span></span>|<span data-ttu-id="15759-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="15759-135">Key of the entity.</span></span>|
|<span data-ttu-id="15759-136">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="15759-136">gracePeriodHours</span></span>|<span data-ttu-id="15759-137">Int32</span><span class="sxs-lookup"><span data-stu-id="15759-137">Int32</span></span>|<span data-ttu-id="15759-138">Anzahl Stunden, die gewartet wird, bis die Aktion erzwungen wird.</span><span class="sxs-lookup"><span data-stu-id="15759-138">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="15759-139">Gültige Werte: 0 bis 8760.</span><span class="sxs-lookup"><span data-stu-id="15759-139">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="15759-140">actionType</span><span class="sxs-lookup"><span data-stu-id="15759-140">actionType</span></span>|[<span data-ttu-id="15759-141">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="15759-141">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="15759-142">Welche Aktion erfolgen soll.</span><span class="sxs-lookup"><span data-stu-id="15759-142">What action to take.</span></span> <span data-ttu-id="15759-143">Mögliche Werte sind: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification` und `remoteLock`.</span><span class="sxs-lookup"><span data-stu-id="15759-143">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="15759-144">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="15759-144">notificationTemplateId</span></span>|<span data-ttu-id="15759-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15759-145">String</span></span>|<span data-ttu-id="15759-146">Benachrichtigungs-E-Mail-Vorlage, die verwendet werden soll</span><span class="sxs-lookup"><span data-stu-id="15759-146">What notification Message template to use</span></span>|
|<span data-ttu-id="15759-147">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="15759-147">notificationMessageCCList</span></span>|<span data-ttu-id="15759-148">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="15759-148">String collection</span></span>|<span data-ttu-id="15759-149">Liste der Gruppen-IDs, die festlegt, wer in der Benachrichtigungs-E-Mail in CC gesetzt wird</span><span class="sxs-lookup"><span data-stu-id="15759-149">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="15759-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="15759-150">Response</span></span>
<span data-ttu-id="15759-151">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="15759-151">If successful, this method returns a `201 Created` response code and a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15759-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="15759-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="15759-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="15759-153">Request</span></span>
<span data-ttu-id="15759-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="15759-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="15759-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="15759-155">Response</span></span>
<span data-ttu-id="15759-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="15759-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




