---
title: Remote Action Audit-Ressourcentyp
description: Bericht über die Remote Aktionen, die auf den Geräten eingeleitet wurden, die zu einem bestimmten Mandanten gehören.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c06f7472addff7c475eeeb8ac3f1a26cc7ea78bc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165877"
---
# <a name="remoteactionaudit-resource-type"></a><span data-ttu-id="19a7c-103">Remote Action Audit-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="19a7c-103">remoteActionAudit resource type</span></span>

> <span data-ttu-id="19a7c-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19a7c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19a7c-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="19a7c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19a7c-106">Bericht über die Remote Aktionen, die auf den Geräten eingeleitet wurden, die zu einem bestimmten Mandanten gehören.</span><span class="sxs-lookup"><span data-stu-id="19a7c-106">Report of remote actions initiated on the devices belonging to a certain tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="19a7c-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="19a7c-107">Methods</span></span>
|<span data-ttu-id="19a7c-108">Methode</span><span class="sxs-lookup"><span data-stu-id="19a7c-108">Method</span></span>|<span data-ttu-id="19a7c-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="19a7c-109">Return Type</span></span>|<span data-ttu-id="19a7c-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="19a7c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="19a7c-111">RemoteActionAudits aufListen</span><span class="sxs-lookup"><span data-stu-id="19a7c-111">List remoteActionAudits</span></span>](../api/intune-devices-remoteactionaudit-list.md)|<span data-ttu-id="19a7c-112">[Remote Action Audit](../resources/intune-devices-remoteactionaudit.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="19a7c-112">[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) collection</span></span>|<span data-ttu-id="19a7c-113">AufListen von Eigenschaften und Beziehungen der [Remote Action Audit](../resources/intune-devices-remoteactionaudit.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="19a7c-113">List properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) objects.</span></span>|
|[<span data-ttu-id="19a7c-114">Remote Action Audit abrufen</span><span class="sxs-lookup"><span data-stu-id="19a7c-114">Get remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-get.md)|[<span data-ttu-id="19a7c-115">Remote Action Audit</span><span class="sxs-lookup"><span data-stu-id="19a7c-115">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="19a7c-116">Lesen von Eigenschaften und Beziehungen des [Remote Action Audit](../resources/intune-devices-remoteactionaudit.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="19a7c-116">Read properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="19a7c-117">Remote Action Audit erstellen</span><span class="sxs-lookup"><span data-stu-id="19a7c-117">Create remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-create.md)|[<span data-ttu-id="19a7c-118">Remote Action Audit</span><span class="sxs-lookup"><span data-stu-id="19a7c-118">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="19a7c-119">Erstellen eines neuen [Remote Action Audit](../resources/intune-devices-remoteactionaudit.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="19a7c-119">Create a new [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="19a7c-120">Remote Action Audit löschen</span><span class="sxs-lookup"><span data-stu-id="19a7c-120">Delete remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-delete.md)|<span data-ttu-id="19a7c-121">Keine</span><span class="sxs-lookup"><span data-stu-id="19a7c-121">None</span></span>|<span data-ttu-id="19a7c-122">Löscht eine [Remote Action Audit](../resources/intune-devices-remoteactionaudit.md).</span><span class="sxs-lookup"><span data-stu-id="19a7c-122">Deletes a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span></span>|
|[<span data-ttu-id="19a7c-123">Remote Action Audit aktualisieren</span><span class="sxs-lookup"><span data-stu-id="19a7c-123">Update remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-update.md)|[<span data-ttu-id="19a7c-124">Remote Action Audit</span><span class="sxs-lookup"><span data-stu-id="19a7c-124">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="19a7c-125">Aktualisieren der Eigenschaften eines [Remote Action Audit](../resources/intune-devices-remoteactionaudit.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="19a7c-125">Update the properties of a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="19a7c-126">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="19a7c-126">Properties</span></span>
|<span data-ttu-id="19a7c-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="19a7c-127">Property</span></span>|<span data-ttu-id="19a7c-128">Typ</span><span class="sxs-lookup"><span data-stu-id="19a7c-128">Type</span></span>|<span data-ttu-id="19a7c-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="19a7c-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19a7c-130">id</span><span class="sxs-lookup"><span data-stu-id="19a7c-130">id</span></span>|<span data-ttu-id="19a7c-131">String</span><span class="sxs-lookup"><span data-stu-id="19a7c-131">String</span></span>|<span data-ttu-id="19a7c-132">Berichts-ID.</span><span class="sxs-lookup"><span data-stu-id="19a7c-132">Report Id.</span></span>|
|<span data-ttu-id="19a7c-133">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="19a7c-133">deviceDisplayName</span></span>|<span data-ttu-id="19a7c-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="19a7c-134">String</span></span>|<span data-ttu-id="19a7c-135">InTune-Gerätename.</span><span class="sxs-lookup"><span data-stu-id="19a7c-135">Intune device name.</span></span>|
|<span data-ttu-id="19a7c-136">userName</span><span class="sxs-lookup"><span data-stu-id="19a7c-136">userName</span></span>|<span data-ttu-id="19a7c-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="19a7c-137">String</span></span>|<span data-ttu-id="19a7c-138">\[veraltet verwenden\] Sie stattdessen Eigenschaften initiatedbyuserprincipalname.</span><span class="sxs-lookup"><span data-stu-id="19a7c-138">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="19a7c-139">Eigenschaften initiatedbyuserprincipalname</span><span class="sxs-lookup"><span data-stu-id="19a7c-139">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="19a7c-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="19a7c-140">String</span></span>|<span data-ttu-id="19a7c-141">Benutzer, der die Geräte Aktion initiiert hat, Format ist UPN.</span><span class="sxs-lookup"><span data-stu-id="19a7c-141">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="19a7c-142">Aktion</span><span class="sxs-lookup"><span data-stu-id="19a7c-142">action</span></span>|[<span data-ttu-id="19a7c-143">Remote-Steuerung</span><span class="sxs-lookup"><span data-stu-id="19a7c-143">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="19a7c-144">Der Name der Aktion.</span><span class="sxs-lookup"><span data-stu-id="19a7c-144">The action name.</span></span> <span data-ttu-id="19a7c-145">Mögliche Werte sind: `unknown`, `factoryReset`, `removeCompanyData` `resetPasscode` `remoteLock` `enableLostMode` `disableLostMode` `rebootNow` `recoverPasscode` `cleanWindowsDevice` `logoutSharedAppleDeviceActiveUser` `quickScan` `fullScan` `windowsDefenderUpdateSignatures`,,,,,,,, `factoryResetKeepEnrollmentData`,, `shutDown` ,,,,,, `updateDeviceAccount` `automaticRedeployment` `locateDevice` .</span><span class="sxs-lookup"><span data-stu-id="19a7c-145">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`.</span></span>|
|<span data-ttu-id="19a7c-146">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="19a7c-146">requestDateTime</span></span>|<span data-ttu-id="19a7c-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19a7c-147">DateTimeOffset</span></span>|<span data-ttu-id="19a7c-148">Zeitpunkt der Ausgabe der Aktion in UTC.</span><span class="sxs-lookup"><span data-stu-id="19a7c-148">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="19a7c-149">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="19a7c-149">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="19a7c-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="19a7c-150">String</span></span>|<span data-ttu-id="19a7c-151">UPN des Geräte Besitzers.</span><span class="sxs-lookup"><span data-stu-id="19a7c-151">Upn of the device owner.</span></span>|
|<span data-ttu-id="19a7c-152">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="19a7c-152">deviceIMEI</span></span>|<span data-ttu-id="19a7c-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="19a7c-153">String</span></span>|<span data-ttu-id="19a7c-154">IMEI des Geräts.</span><span class="sxs-lookup"><span data-stu-id="19a7c-154">IMEI of the device.</span></span>|
|<span data-ttu-id="19a7c-155">actionState</span><span class="sxs-lookup"><span data-stu-id="19a7c-155">actionState</span></span>|[<span data-ttu-id="19a7c-156">actionState</span><span class="sxs-lookup"><span data-stu-id="19a7c-156">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="19a7c-157">Aktionsstatus.</span><span class="sxs-lookup"><span data-stu-id="19a7c-157">Action state.</span></span> <span data-ttu-id="19a7c-158">Mögliche Werte: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="19a7c-158">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="19a7c-159">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="19a7c-159">Relationships</span></span>
<span data-ttu-id="19a7c-160">Keine</span><span class="sxs-lookup"><span data-stu-id="19a7c-160">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="19a7c-161">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="19a7c-161">JSON Representation</span></span>
<span data-ttu-id="19a7c-162">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="19a7c-162">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteActionAudit"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "id": "String (identifier)",
  "deviceDisplayName": "String",
  "userName": "String",
  "initiatedByUserPrincipalName": "String",
  "action": "String",
  "requestDateTime": "String (timestamp)",
  "deviceOwnerUserPrincipalName": "String",
  "deviceIMEI": "String",
  "actionState": "String"
}
```




