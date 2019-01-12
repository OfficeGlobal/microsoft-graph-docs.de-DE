---
title: Erstellen von deviceConfigurationConflictSummary
description: Erstellen eines neuen DeviceConfigurationConflictSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ea5aa43cf4df325afbffddcc1323f98bf89a3166
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968400"
---
# <a name="create-deviceconfigurationconflictsummary"></a><span data-ttu-id="c7490-103">Erstellen von deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="c7490-103">Create deviceConfigurationConflictSummary</span></span>

> <span data-ttu-id="c7490-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c7490-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c7490-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c7490-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c7490-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c7490-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c7490-107">Erstellen eines neuen [DeviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c7490-107">Create a new [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c7490-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c7490-108">Prerequisites</span></span>
<span data-ttu-id="c7490-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7490-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7490-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c7490-111">Permission type</span></span>|<span data-ttu-id="c7490-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c7490-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7490-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c7490-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c7490-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7490-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c7490-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c7490-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7490-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c7490-116">Not supported.</span></span>|
|<span data-ttu-id="c7490-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c7490-117">Application</span></span>|<span data-ttu-id="c7490-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c7490-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7490-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c7490-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationConflictSummary
```

## <a name="request-headers"></a><span data-ttu-id="c7490-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c7490-120">Request headers</span></span>
|<span data-ttu-id="c7490-121">Header</span><span class="sxs-lookup"><span data-stu-id="c7490-121">Header</span></span>|<span data-ttu-id="c7490-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c7490-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7490-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7490-123">Authorization</span></span>|<span data-ttu-id="c7490-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c7490-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7490-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c7490-125">Accept</span></span>|<span data-ttu-id="c7490-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c7490-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7490-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c7490-127">Request body</span></span>
<span data-ttu-id="c7490-128">Geben Sie im Textkörper Anforderung für das Objekt DeviceConfigurationConflictSummary eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="c7490-128">In the request body, supply a JSON representation for the deviceConfigurationConflictSummary object.</span></span>

<span data-ttu-id="c7490-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die DeviceConfigurationConflictSummary erstellen.</span><span class="sxs-lookup"><span data-stu-id="c7490-129">The following table shows the properties that are required when you create the deviceConfigurationConflictSummary.</span></span>

|<span data-ttu-id="c7490-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c7490-130">Property</span></span>|<span data-ttu-id="c7490-131">Typ</span><span class="sxs-lookup"><span data-stu-id="c7490-131">Type</span></span>|<span data-ttu-id="c7490-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c7490-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7490-133">conflictingDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="c7490-133">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="c7490-134">[settingSource](../resources/intune-deviceconfig-settingsource.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="c7490-134">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="c7490-135">Der Satz von Richtlinien mit der angegebenen Einstellung in Konflikt</span><span class="sxs-lookup"><span data-stu-id="c7490-135">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="c7490-136">id</span><span class="sxs-lookup"><span data-stu-id="c7490-136">id</span></span>|<span data-ttu-id="c7490-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c7490-137">String</span></span>|<span data-ttu-id="c7490-138">Die Id für diesen Satz von miteinander in Konflikt stehende Richtlinien.</span><span class="sxs-lookup"><span data-stu-id="c7490-138">The id for this set of conflicting policies.</span></span> <span data-ttu-id="c7490-139">Diese Id ist die Ids aller Richtlinien in ConflictingDeviceConfigurations in lexikografischer Reihenfolge durch Unterstriche getrennt sind.</span><span class="sxs-lookup"><span data-stu-id="c7490-139">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="c7490-140">contributingSettings</span><span class="sxs-lookup"><span data-stu-id="c7490-140">contributingSettings</span></span>|<span data-ttu-id="c7490-141">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="c7490-141">String collection</span></span>|<span data-ttu-id="c7490-142">Die Gruppe von Einstellungen in Konflikt mit der angegebenen Richtlinien</span><span class="sxs-lookup"><span data-stu-id="c7490-142">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="c7490-143">deviceCheckinsImpacted</span><span class="sxs-lookup"><span data-stu-id="c7490-143">deviceCheckinsImpacted</span></span>|<span data-ttu-id="c7490-144">Int32</span><span class="sxs-lookup"><span data-stu-id="c7490-144">Int32</span></span>|<span data-ttu-id="c7490-145">Die Anzahl der durch die miteinander in Konflikt stehende Richtlinien und Einstellungen beeinträchtigt Eincheckvorgänge</span><span class="sxs-lookup"><span data-stu-id="c7490-145">The count of checkins impacted by the conflicting policies and settings</span></span>|



## <a name="response"></a><span data-ttu-id="c7490-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="c7490-146">Response</span></span>
<span data-ttu-id="c7490-147">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [DeviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="c7490-147">If successful, this method returns a `201 Created` response code and a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7490-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c7490-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="c7490-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c7490-149">Request</span></span>
<span data-ttu-id="c7490-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c7490-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c7490-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="c7490-151">Response</span></span>
<span data-ttu-id="c7490-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c7490-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





