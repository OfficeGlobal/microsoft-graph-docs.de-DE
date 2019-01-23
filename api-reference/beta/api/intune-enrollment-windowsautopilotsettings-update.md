---
title: WindowsAutopilotSettings aktualisieren
description: Aktualisieren Sie die Eigenschaften eines WindowsAutopilotSettings-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a0c7f0fba63fa94bfdf2d5a6f9eebd344aa12b93
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394250"
---
# <a name="update-windowsautopilotsettings"></a><span data-ttu-id="178a0-103">WindowsAutopilotSettings aktualisieren</span><span class="sxs-lookup"><span data-stu-id="178a0-103">Update windowsAutopilotSettings</span></span>

> <span data-ttu-id="178a0-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="178a0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="178a0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="178a0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="178a0-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="178a0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="178a0-107">Aktualisieren Sie die Eigenschaften eines [WindowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="178a0-107">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="178a0-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="178a0-108">Prerequisites</span></span>
<span data-ttu-id="178a0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="178a0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="178a0-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="178a0-111">Permission type</span></span>|<span data-ttu-id="178a0-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="178a0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="178a0-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="178a0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="178a0-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="178a0-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="178a0-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="178a0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="178a0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="178a0-116">Not supported.</span></span>|
|<span data-ttu-id="178a0-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="178a0-117">Application</span></span>|<span data-ttu-id="178a0-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="178a0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="178a0-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="178a0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotSettings
```

## <a name="request-headers"></a><span data-ttu-id="178a0-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="178a0-120">Request headers</span></span>
|<span data-ttu-id="178a0-121">Header</span><span class="sxs-lookup"><span data-stu-id="178a0-121">Header</span></span>|<span data-ttu-id="178a0-122">Wert</span><span class="sxs-lookup"><span data-stu-id="178a0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="178a0-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="178a0-123">Authorization</span></span>|<span data-ttu-id="178a0-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="178a0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="178a0-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="178a0-125">Accept</span></span>|<span data-ttu-id="178a0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="178a0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="178a0-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="178a0-127">Request body</span></span>
<span data-ttu-id="178a0-128">Geben Sie im Textkörper Anforderung für das Objekt [WindowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="178a0-128">In the request body, supply a JSON representation for the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>

<span data-ttu-id="178a0-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [WindowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="178a0-129">The following table shows the properties that are required when you create the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md).</span></span>

|<span data-ttu-id="178a0-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="178a0-130">Property</span></span>|<span data-ttu-id="178a0-131">Typ</span><span class="sxs-lookup"><span data-stu-id="178a0-131">Type</span></span>|<span data-ttu-id="178a0-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="178a0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="178a0-133">id</span><span class="sxs-lookup"><span data-stu-id="178a0-133">id</span></span>|<span data-ttu-id="178a0-134">String</span><span class="sxs-lookup"><span data-stu-id="178a0-134">String</span></span>|<span data-ttu-id="178a0-135">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="178a0-135">The GUID for the object</span></span>|
|<span data-ttu-id="178a0-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="178a0-136">lastSyncDateTime</span></span>|<span data-ttu-id="178a0-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="178a0-137">DateTimeOffset</span></span>|<span data-ttu-id="178a0-138">Zuletzt Daten synchronisieren Datum-Uhrzeit mit DDS-Dienst.</span><span class="sxs-lookup"><span data-stu-id="178a0-138">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="178a0-139">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="178a0-139">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="178a0-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="178a0-140">DateTimeOffset</span></span>|<span data-ttu-id="178a0-141">Zuletzt Daten synchronisieren Datum-Uhrzeit mit DDS-Dienst.</span><span class="sxs-lookup"><span data-stu-id="178a0-141">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="178a0-142">syncStatus</span><span class="sxs-lookup"><span data-stu-id="178a0-142">syncStatus</span></span>|[<span data-ttu-id="178a0-143">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="178a0-143">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="178a0-144">Gibt den Status der Synchronisierung mit Gerät Daten Synchronisierungsdiensts (DDS).</span><span class="sxs-lookup"><span data-stu-id="178a0-144">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="178a0-145">Mögliche Werte sind: `unknown`, `inProgress`, `completed` und `failed`.</span><span class="sxs-lookup"><span data-stu-id="178a0-145">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|



## <a name="response"></a><span data-ttu-id="178a0-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="178a0-146">Response</span></span>
<span data-ttu-id="178a0-147">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [WindowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="178a0-147">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="178a0-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="178a0-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="178a0-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="178a0-149">Request</span></span>
<span data-ttu-id="178a0-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="178a0-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotSettings
Content-type: application/json
Content-length: 230

{
  "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "lastManualSyncTriggerDateTime": "2016-12-31T23:57:54.7364636-08:00",
  "syncStatus": "inProgress"
}
```

### <a name="response"></a><span data-ttu-id="178a0-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="178a0-151">Response</span></span>
<span data-ttu-id="178a0-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="178a0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 279

{
  "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
  "id": "08c16770-6770-08c1-7067-c1087067c108",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "lastManualSyncTriggerDateTime": "2016-12-31T23:57:54.7364636-08:00",
  "syncStatus": "inProgress"
}
```




