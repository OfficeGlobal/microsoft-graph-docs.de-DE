---
title: Erstellen von „deviceComplianceActionItem“
description: Diese Methode erstellt ein neues Objekt des Typs deviceComplianceActionItem.
author: tfitzmac
ms.openlocfilehash: a4e0facb0a9d34d840b6ef737c09737c9a6626a4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317976"
---
# <a name="create-devicecomplianceactionitem"></a><span data-ttu-id="13f30-103">Erstellen von „deviceComplianceActionItem“</span><span class="sxs-lookup"><span data-stu-id="13f30-103">Create deviceComplianceActionItem</span></span>

> <span data-ttu-id="13f30-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="13f30-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="13f30-105">Diese Methode erstellt ein neues Objekt des Typs [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="13f30-105">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="13f30-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="13f30-106">Prerequisites</span></span>
<span data-ttu-id="13f30-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13f30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13f30-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="13f30-109">Permission type</span></span>|<span data-ttu-id="13f30-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="13f30-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13f30-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="13f30-111">Delegated (work or school account)</span></span>|<span data-ttu-id="13f30-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13f30-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="13f30-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="13f30-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13f30-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="13f30-114">Not supported.</span></span>|
|<span data-ttu-id="13f30-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="13f30-115">Application</span></span>|<span data-ttu-id="13f30-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="13f30-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13f30-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="13f30-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="13f30-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="13f30-118">Request headers</span></span>
|<span data-ttu-id="13f30-119">Header</span><span class="sxs-lookup"><span data-stu-id="13f30-119">Header</span></span>|<span data-ttu-id="13f30-120">Wert</span><span class="sxs-lookup"><span data-stu-id="13f30-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13f30-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="13f30-121">Authorization</span></span>|<span data-ttu-id="13f30-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="13f30-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13f30-123">Accept</span><span class="sxs-lookup"><span data-stu-id="13f30-123">Accept</span></span>|<span data-ttu-id="13f30-124">application/json</span><span class="sxs-lookup"><span data-stu-id="13f30-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13f30-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="13f30-125">Request body</span></span>
<span data-ttu-id="13f30-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekt des Typs „deviceComplianceActionItem“ an.</span><span class="sxs-lookup"><span data-stu-id="13f30-126">In the request body, supply a JSON representation for the deviceComplianceActionItem object.</span></span>

<span data-ttu-id="13f30-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceComplianceActionItem“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="13f30-127">The following table shows the properties that are required when you create the deviceComplianceActionItem.</span></span>

|<span data-ttu-id="13f30-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="13f30-128">Property</span></span>|<span data-ttu-id="13f30-129">Typ</span><span class="sxs-lookup"><span data-stu-id="13f30-129">Type</span></span>|<span data-ttu-id="13f30-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="13f30-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13f30-131">id</span><span class="sxs-lookup"><span data-stu-id="13f30-131">id</span></span>|<span data-ttu-id="13f30-132">String</span><span class="sxs-lookup"><span data-stu-id="13f30-132">String</span></span>|<span data-ttu-id="13f30-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="13f30-133">Key of the entity.</span></span>|
|<span data-ttu-id="13f30-134">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="13f30-134">gracePeriodHours</span></span>|<span data-ttu-id="13f30-135">Int32</span><span class="sxs-lookup"><span data-stu-id="13f30-135">Int32</span></span>|<span data-ttu-id="13f30-136">Anzahl Stunden, die gewartet wird, bis die Aktion erzwungen wird.</span><span class="sxs-lookup"><span data-stu-id="13f30-136">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="13f30-137">Gültige Werte: 0 bis 8760.</span><span class="sxs-lookup"><span data-stu-id="13f30-137">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="13f30-138">actionType</span><span class="sxs-lookup"><span data-stu-id="13f30-138">actionType</span></span>|[<span data-ttu-id="13f30-139">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="13f30-139">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="13f30-140">Welche Aktion erfolgen soll.</span><span class="sxs-lookup"><span data-stu-id="13f30-140">What action to take.</span></span> <span data-ttu-id="13f30-141">Mögliche Werte sind: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles` und `pushNotification`.</span><span class="sxs-lookup"><span data-stu-id="13f30-141">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span></span>|
|<span data-ttu-id="13f30-142">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="13f30-142">notificationTemplateId</span></span>|<span data-ttu-id="13f30-143">String</span><span class="sxs-lookup"><span data-stu-id="13f30-143">String</span></span>|<span data-ttu-id="13f30-144">Benachrichtigungs-E-Mail-Vorlage, die verwendet werden soll</span><span class="sxs-lookup"><span data-stu-id="13f30-144">What notification Message template to use</span></span>|
|<span data-ttu-id="13f30-145">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="13f30-145">notificationMessageCCList</span></span>|<span data-ttu-id="13f30-146">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="13f30-146">String collection</span></span>|<span data-ttu-id="13f30-147">Liste der Gruppen-IDs, die festlegt, wer in der Benachrichtigungs-E-Mail in CC gesetzt wird</span><span class="sxs-lookup"><span data-stu-id="13f30-147">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="13f30-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="13f30-148">Response</span></span>
<span data-ttu-id="13f30-149">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="13f30-149">If successful, this method returns a `201 Created` response code and a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13f30-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="13f30-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="13f30-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="13f30-151">Request</span></span>
<span data-ttu-id="13f30-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="13f30-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="13f30-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="13f30-153">Response</span></span>
<span data-ttu-id="13f30-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="13f30-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



