---
title: WindowsAutopilotSettings aktualisieren
description: Aktualisieren Sie die Eigenschaften eines WindowsAutopilotSettings-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8087ce2a3d7fd02eb6cc118d75082382bcddd58d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877651"
---
# <a name="update-windowsautopilotsettings"></a><span data-ttu-id="1e5b3-103">WindowsAutopilotSettings aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1e5b3-103">Update windowsAutopilotSettings</span></span>

> <span data-ttu-id="1e5b3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1e5b3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e5b3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1e5b3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1e5b3-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1e5b3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e5b3-107">Aktualisieren Sie die Eigenschaften eines [WindowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="1e5b3-107">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1e5b3-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1e5b3-108">Prerequisites</span></span>
<span data-ttu-id="1e5b3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e5b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e5b3-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1e5b3-111">Permission type</span></span>|<span data-ttu-id="1e5b3-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1e5b3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e5b3-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1e5b3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1e5b3-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e5b3-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1e5b3-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1e5b3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e5b3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1e5b3-116">Not supported.</span></span>|
|<span data-ttu-id="1e5b3-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1e5b3-117">Application</span></span>|<span data-ttu-id="1e5b3-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1e5b3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e5b3-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1e5b3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotSettings
```

## <a name="request-headers"></a><span data-ttu-id="1e5b3-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1e5b3-120">Request headers</span></span>
|<span data-ttu-id="1e5b3-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1e5b3-121">Header</span></span>|<span data-ttu-id="1e5b3-122">Wert</span><span class="sxs-lookup"><span data-stu-id="1e5b3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e5b3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e5b3-123">Authorization</span></span>|<span data-ttu-id="1e5b3-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1e5b3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e5b3-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1e5b3-125">Accept</span></span>|<span data-ttu-id="1e5b3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1e5b3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e5b3-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1e5b3-127">Request body</span></span>
<span data-ttu-id="1e5b3-128">Geben Sie im Textkörper Anforderung für das Objekt [WindowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="1e5b3-128">In the request body, supply a JSON representation for the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>

<span data-ttu-id="1e5b3-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [WindowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="1e5b3-129">The following table shows the properties that are required when you create the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md).</span></span>

|<span data-ttu-id="1e5b3-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1e5b3-130">Property</span></span>|<span data-ttu-id="1e5b3-131">Typ</span><span class="sxs-lookup"><span data-stu-id="1e5b3-131">Type</span></span>|<span data-ttu-id="1e5b3-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1e5b3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e5b3-133">id</span><span class="sxs-lookup"><span data-stu-id="1e5b3-133">id</span></span>|<span data-ttu-id="1e5b3-134">String</span><span class="sxs-lookup"><span data-stu-id="1e5b3-134">String</span></span>|<span data-ttu-id="1e5b3-135">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="1e5b3-135">The GUID for the object</span></span>|
|<span data-ttu-id="1e5b3-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="1e5b3-136">lastSyncDateTime</span></span>|<span data-ttu-id="1e5b3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e5b3-137">DateTimeOffset</span></span>|<span data-ttu-id="1e5b3-138">Zuletzt Daten synchronisieren Datum-Uhrzeit mit DDS-Dienst.</span><span class="sxs-lookup"><span data-stu-id="1e5b3-138">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="1e5b3-139">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="1e5b3-139">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="1e5b3-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e5b3-140">DateTimeOffset</span></span>|<span data-ttu-id="1e5b3-141">Zuletzt Daten synchronisieren Datum-Uhrzeit mit DDS-Dienst.</span><span class="sxs-lookup"><span data-stu-id="1e5b3-141">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="1e5b3-142">syncStatus</span><span class="sxs-lookup"><span data-stu-id="1e5b3-142">syncStatus</span></span>|[<span data-ttu-id="1e5b3-143">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="1e5b3-143">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="1e5b3-144">Gibt den Status der Synchronisierung mit Gerät Daten Synchronisierungsdiensts (DDS).</span><span class="sxs-lookup"><span data-stu-id="1e5b3-144">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="1e5b3-145">Mögliche Werte sind: `unknown`, `inProgress`, `completed` und `failed`.</span><span class="sxs-lookup"><span data-stu-id="1e5b3-145">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|



## <a name="response"></a><span data-ttu-id="1e5b3-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="1e5b3-146">Response</span></span>
<span data-ttu-id="1e5b3-147">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [WindowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="1e5b3-147">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e5b3-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1e5b3-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="1e5b3-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1e5b3-149">Request</span></span>
<span data-ttu-id="1e5b3-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1e5b3-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotSettings
Content-type: application/json
Content-length: 167

{
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "lastManualSyncTriggerDateTime": "2016-12-31T23:57:54.7364636-08:00",
  "syncStatus": "inProgress"
}
```

### <a name="response"></a><span data-ttu-id="1e5b3-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="1e5b3-151">Response</span></span>
<span data-ttu-id="1e5b3-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1e5b3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





