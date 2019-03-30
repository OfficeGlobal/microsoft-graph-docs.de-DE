---
title: DeviceConfigurationConflictSummary aktualisieren
description: Aktualisieren der Eigenschaften eines deviceConfigurationConflictSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cfe4b4d9925b64e35a5e79fad5f1f124350a1ee4
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30989239"
---
# <a name="update-deviceconfigurationconflictsummary"></a><span data-ttu-id="f76d1-103">DeviceConfigurationConflictSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f76d1-103">Update deviceConfigurationConflictSummary</span></span>

> <span data-ttu-id="f76d1-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f76d1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f76d1-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f76d1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f76d1-106">Aktualisieren der Eigenschaften eines [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f76d1-106">Update the properties of a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f76d1-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f76d1-107">Prerequisites</span></span>
<span data-ttu-id="f76d1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f76d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f76d1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f76d1-110">Permission type</span></span>|<span data-ttu-id="f76d1-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f76d1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f76d1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f76d1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f76d1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f76d1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f76d1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f76d1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f76d1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f76d1-115">Not supported.</span></span>|
|<span data-ttu-id="f76d1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f76d1-116">Application</span></span>|<span data-ttu-id="f76d1-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f76d1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f76d1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f76d1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="f76d1-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f76d1-119">Request headers</span></span>
|<span data-ttu-id="f76d1-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f76d1-120">Header</span></span>|<span data-ttu-id="f76d1-121">Wert</span><span class="sxs-lookup"><span data-stu-id="f76d1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f76d1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f76d1-122">Authorization</span></span>|<span data-ttu-id="f76d1-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f76d1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f76d1-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f76d1-124">Accept</span></span>|<span data-ttu-id="f76d1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f76d1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f76d1-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f76d1-126">Request body</span></span>
<span data-ttu-id="f76d1-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="f76d1-127">In the request body, supply a JSON representation for the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

<span data-ttu-id="f76d1-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="f76d1-128">The following table shows the properties that are required when you create the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span></span>

|<span data-ttu-id="f76d1-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f76d1-129">Property</span></span>|<span data-ttu-id="f76d1-130">Typ</span><span class="sxs-lookup"><span data-stu-id="f76d1-130">Type</span></span>|<span data-ttu-id="f76d1-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f76d1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f76d1-132">conflictingDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="f76d1-132">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="f76d1-133">[settingSource](../resources/intune-deviceconfig-settingsource.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="f76d1-133">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="f76d1-134">Die Gruppe von Richtlinien, die mit der angegebenen Einstellung in Konflikt stehen</span><span class="sxs-lookup"><span data-stu-id="f76d1-134">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="f76d1-135">id</span><span class="sxs-lookup"><span data-stu-id="f76d1-135">id</span></span>|<span data-ttu-id="f76d1-136">String</span><span class="sxs-lookup"><span data-stu-id="f76d1-136">String</span></span>|<span data-ttu-id="f76d1-137">Die ID für diesen Satz von Konflikt verursachenden Richtlinien.</span><span class="sxs-lookup"><span data-stu-id="f76d1-137">The id for this set of conflicting policies.</span></span> <span data-ttu-id="f76d1-138">Diese ID ist die IDs aller Richtlinien in ConflictingDeviceConfigurations in lexikografische Reihenfolge durch Unterstriche getrennt.</span><span class="sxs-lookup"><span data-stu-id="f76d1-138">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="f76d1-139">contributingSettings</span><span class="sxs-lookup"><span data-stu-id="f76d1-139">contributingSettings</span></span>|<span data-ttu-id="f76d1-140">String collection</span><span class="sxs-lookup"><span data-stu-id="f76d1-140">String collection</span></span>|<span data-ttu-id="f76d1-141">Die Gruppe von Einstellungen, die mit den angegebenen Richtlinien in Konflikt stehen</span><span class="sxs-lookup"><span data-stu-id="f76d1-141">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="f76d1-142">deviceCheckinsImpacted</span><span class="sxs-lookup"><span data-stu-id="f76d1-142">deviceCheckinsImpacted</span></span>|<span data-ttu-id="f76d1-143">Int32</span><span class="sxs-lookup"><span data-stu-id="f76d1-143">Int32</span></span>|<span data-ttu-id="f76d1-144">Die Anzahl der checkins, die von den widersprüchlichen Richtlinien und Einstellungen beeinflusst wurden</span><span class="sxs-lookup"><span data-stu-id="f76d1-144">The count of checkins impacted by the conflicting policies and settings</span></span>|



## <a name="response"></a><span data-ttu-id="f76d1-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="f76d1-145">Response</span></span>
<span data-ttu-id="f76d1-146">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f76d1-146">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f76d1-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f76d1-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="f76d1-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f76d1-148">Request</span></span>
<span data-ttu-id="f76d1-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f76d1-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
Content-type: application/json
Content-length: 361

{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "Id value",
      "displayName": "Display Name value"
    }
  ],
  "contributingSettings": [
    "Contributing Settings value"
  ],
  "deviceCheckinsImpacted": 6
}
```

### <a name="response"></a><span data-ttu-id="f76d1-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="f76d1-150">Response</span></span>
<span data-ttu-id="f76d1-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f76d1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 410

{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "Id value",
      "displayName": "Display Name value"
    }
  ],
  "id": "d5f22c23-2c23-d5f2-232c-f2d5232cf2d5",
  "contributingSettings": [
    "Contributing Settings value"
  ],
  "deviceCheckinsImpacted": 6
}
```




