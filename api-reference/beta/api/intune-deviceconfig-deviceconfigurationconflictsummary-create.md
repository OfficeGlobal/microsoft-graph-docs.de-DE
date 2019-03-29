---
title: DeviceConfigurationConflictSummary erstellen
description: Erstellen eines neuen deviceConfigurationConflictSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2e59946ce8e252daedc13cae4800eece4fdd8bd4
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30960685"
---
# <a name="create-deviceconfigurationconflictsummary"></a><span data-ttu-id="b612c-103">DeviceConfigurationConflictSummary erstellen</span><span class="sxs-lookup"><span data-stu-id="b612c-103">Create deviceConfigurationConflictSummary</span></span>

> <span data-ttu-id="b612c-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b612c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b612c-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b612c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b612c-106">Erstellen eines neuen [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b612c-106">Create a new [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b612c-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b612c-107">Prerequisites</span></span>
<span data-ttu-id="b612c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b612c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b612c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b612c-110">Permission type</span></span>|<span data-ttu-id="b612c-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b612c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b612c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b612c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b612c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b612c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b612c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b612c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b612c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b612c-115">Not supported.</span></span>|
|<span data-ttu-id="b612c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b612c-116">Application</span></span>|<span data-ttu-id="b612c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b612c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b612c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b612c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationConflictSummary
```

## <a name="request-headers"></a><span data-ttu-id="b612c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b612c-119">Request headers</span></span>
|<span data-ttu-id="b612c-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b612c-120">Header</span></span>|<span data-ttu-id="b612c-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b612c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b612c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b612c-122">Authorization</span></span>|<span data-ttu-id="b612c-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b612c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b612c-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b612c-124">Accept</span></span>|<span data-ttu-id="b612c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b612c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b612c-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b612c-126">Request body</span></span>
<span data-ttu-id="b612c-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das deviceConfigurationConflictSummary-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="b612c-127">In the request body, supply a JSON representation for the deviceConfigurationConflictSummary object.</span></span>

<span data-ttu-id="b612c-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der deviceConfigurationConflictSummary erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b612c-128">The following table shows the properties that are required when you create the deviceConfigurationConflictSummary.</span></span>

|<span data-ttu-id="b612c-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b612c-129">Property</span></span>|<span data-ttu-id="b612c-130">Typ</span><span class="sxs-lookup"><span data-stu-id="b612c-130">Type</span></span>|<span data-ttu-id="b612c-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b612c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b612c-132">conflictingDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="b612c-132">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="b612c-133">[settingSource](../resources/intune-deviceconfig-settingsource.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b612c-133">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="b612c-134">Die Gruppe von Richtlinien, die mit der angegebenen Einstellung in Konflikt stehen</span><span class="sxs-lookup"><span data-stu-id="b612c-134">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="b612c-135">id</span><span class="sxs-lookup"><span data-stu-id="b612c-135">id</span></span>|<span data-ttu-id="b612c-136">String</span><span class="sxs-lookup"><span data-stu-id="b612c-136">String</span></span>|<span data-ttu-id="b612c-137">Die ID für diesen Satz von Konflikt verursachenden Richtlinien.</span><span class="sxs-lookup"><span data-stu-id="b612c-137">The id for this set of conflicting policies.</span></span> <span data-ttu-id="b612c-138">Diese ID ist die IDs aller Richtlinien in ConflictingDeviceConfigurations in lexikografische Reihenfolge durch Unterstriche getrennt.</span><span class="sxs-lookup"><span data-stu-id="b612c-138">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="b612c-139">contributingSettings</span><span class="sxs-lookup"><span data-stu-id="b612c-139">contributingSettings</span></span>|<span data-ttu-id="b612c-140">String collection</span><span class="sxs-lookup"><span data-stu-id="b612c-140">String collection</span></span>|<span data-ttu-id="b612c-141">Die Gruppe von Einstellungen, die mit den angegebenen Richtlinien in Konflikt stehen</span><span class="sxs-lookup"><span data-stu-id="b612c-141">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="b612c-142">deviceCheckinsImpacted</span><span class="sxs-lookup"><span data-stu-id="b612c-142">deviceCheckinsImpacted</span></span>|<span data-ttu-id="b612c-143">Int32</span><span class="sxs-lookup"><span data-stu-id="b612c-143">Int32</span></span>|<span data-ttu-id="b612c-144">Die Anzahl der checkins, die von den widersprüchlichen Richtlinien und Einstellungen beeinflusst wurden</span><span class="sxs-lookup"><span data-stu-id="b612c-144">The count of checkins impacted by the conflicting policies and settings</span></span>|



## <a name="response"></a><span data-ttu-id="b612c-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="b612c-145">Response</span></span>
<span data-ttu-id="b612c-146">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b612c-146">If successful, this method returns a `201 Created` response code and a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b612c-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b612c-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="b612c-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b612c-148">Request</span></span>
<span data-ttu-id="b612c-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b612c-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary
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

### <a name="response"></a><span data-ttu-id="b612c-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="b612c-150">Response</span></span>
<span data-ttu-id="b612c-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b612c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




