---
title: deviceComplianceActionItem aktualisieren
description: Aktualisieren der Eigenschaften eines deviceComplianceActionItem-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 77f1292e240d8d8887adff98aa9326685659bb77
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404974"
---
# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="41977-103">deviceComplianceActionItem aktualisieren</span><span class="sxs-lookup"><span data-stu-id="41977-103">Update deviceComplianceActionItem</span></span>

> <span data-ttu-id="41977-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="41977-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="41977-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="41977-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="41977-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="41977-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41977-107">Aktualisieren der Eigenschaften eines [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="41977-107">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41977-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="41977-108">Prerequisites</span></span>
<span data-ttu-id="41977-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="41977-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="41977-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="41977-111">Permission type</span></span>|<span data-ttu-id="41977-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="41977-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41977-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="41977-113">Delegated (work or school account)</span></span>|<span data-ttu-id="41977-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41977-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="41977-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="41977-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41977-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="41977-116">Not supported.</span></span>|
|<span data-ttu-id="41977-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="41977-117">Application</span></span>|<span data-ttu-id="41977-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="41977-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41977-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="41977-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="41977-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="41977-120">Request headers</span></span>
|<span data-ttu-id="41977-121">Header</span><span class="sxs-lookup"><span data-stu-id="41977-121">Header</span></span>|<span data-ttu-id="41977-122">Wert</span><span class="sxs-lookup"><span data-stu-id="41977-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41977-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="41977-123">Authorization</span></span>|<span data-ttu-id="41977-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="41977-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41977-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="41977-125">Accept</span></span>|<span data-ttu-id="41977-126">application/json</span><span class="sxs-lookup"><span data-stu-id="41977-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41977-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="41977-127">Request body</span></span>
<span data-ttu-id="41977-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekt des Typs [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) an.</span><span class="sxs-lookup"><span data-stu-id="41977-128">In the request body, supply a JSON representation for the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="41977-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="41977-129">The following table shows the properties that are required when you create the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

|<span data-ttu-id="41977-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="41977-130">Property</span></span>|<span data-ttu-id="41977-131">Typ</span><span class="sxs-lookup"><span data-stu-id="41977-131">Type</span></span>|<span data-ttu-id="41977-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="41977-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41977-133">id</span><span class="sxs-lookup"><span data-stu-id="41977-133">id</span></span>|<span data-ttu-id="41977-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="41977-134">String</span></span>|<span data-ttu-id="41977-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="41977-135">Key of the entity.</span></span>|
|<span data-ttu-id="41977-136">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="41977-136">gracePeriodHours</span></span>|<span data-ttu-id="41977-137">Int32</span><span class="sxs-lookup"><span data-stu-id="41977-137">Int32</span></span>|<span data-ttu-id="41977-138">Anzahl Stunden, die gewartet wird, bis die Aktion erzwungen wird.</span><span class="sxs-lookup"><span data-stu-id="41977-138">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="41977-139">Gültige Werte: 0 bis 8760.</span><span class="sxs-lookup"><span data-stu-id="41977-139">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="41977-140">actionType</span><span class="sxs-lookup"><span data-stu-id="41977-140">actionType</span></span>|[<span data-ttu-id="41977-141">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="41977-141">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="41977-142">Welche Aktion erfolgen soll.</span><span class="sxs-lookup"><span data-stu-id="41977-142">What action to take.</span></span> <span data-ttu-id="41977-143">Mögliche Werte sind: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification` und `remoteLock`.</span><span class="sxs-lookup"><span data-stu-id="41977-143">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="41977-144">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="41977-144">notificationTemplateId</span></span>|<span data-ttu-id="41977-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="41977-145">String</span></span>|<span data-ttu-id="41977-146">Benachrichtigungs-E-Mail-Vorlage, die verwendet werden soll</span><span class="sxs-lookup"><span data-stu-id="41977-146">What notification Message template to use</span></span>|
|<span data-ttu-id="41977-147">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="41977-147">notificationMessageCCList</span></span>|<span data-ttu-id="41977-148">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="41977-148">String collection</span></span>|<span data-ttu-id="41977-149">Liste der Gruppen-IDs, die festlegt, wer in der Benachrichtigungs-E-Mail in CC gesetzt wird</span><span class="sxs-lookup"><span data-stu-id="41977-149">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="41977-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="41977-150">Response</span></span>
<span data-ttu-id="41977-151">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="41977-151">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41977-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="41977-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="41977-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="41977-153">Request</span></span>
<span data-ttu-id="41977-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="41977-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="41977-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="41977-155">Response</span></span>
<span data-ttu-id="41977-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="41977-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




