---
title: windowsInformationProtectionAppLearningSummary erstellen
description: Erstellen eines neuen windowsInformationProtectionAppLearningSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 66658cdd601ec7ea1af60a29a9302ca100debfaf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940582"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="eb3f9-103">windowsInformationProtectionAppLearningSummary erstellen</span><span class="sxs-lookup"><span data-stu-id="eb3f9-103">Create windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="eb3f9-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="eb3f9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eb3f9-105">Erstellen eines neuen [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="eb3f9-105">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eb3f9-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="eb3f9-106">Prerequisites</span></span>
<span data-ttu-id="eb3f9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb3f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb3f9-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eb3f9-109">Permission type</span></span>|<span data-ttu-id="eb3f9-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="eb3f9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb3f9-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eb3f9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eb3f9-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb3f9-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="eb3f9-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eb3f9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb3f9-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eb3f9-114">Not supported.</span></span>|
|<span data-ttu-id="eb3f9-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eb3f9-115">Application</span></span>|<span data-ttu-id="eb3f9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eb3f9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb3f9-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb3f9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="eb3f9-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eb3f9-118">Request headers</span></span>
|<span data-ttu-id="eb3f9-119">Header</span><span class="sxs-lookup"><span data-stu-id="eb3f9-119">Header</span></span>|<span data-ttu-id="eb3f9-120">Wert</span><span class="sxs-lookup"><span data-stu-id="eb3f9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb3f9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb3f9-121">Authorization</span></span>|<span data-ttu-id="eb3f9-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="eb3f9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb3f9-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="eb3f9-123">Accept</span></span>|<span data-ttu-id="eb3f9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="eb3f9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb3f9-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="eb3f9-125">Request body</span></span>
<span data-ttu-id="eb3f9-126">Geben Sie im Anforderungstext eine JSON-Darstellung des windowsInformationProtectionAppLearningSummary-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="eb3f9-126">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="eb3f9-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsInformationProtectionAppLearningSummary erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="eb3f9-127">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="eb3f9-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="eb3f9-128">Property</span></span>|<span data-ttu-id="eb3f9-129">Typ</span><span class="sxs-lookup"><span data-stu-id="eb3f9-129">Type</span></span>|<span data-ttu-id="eb3f9-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eb3f9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb3f9-131">id</span><span class="sxs-lookup"><span data-stu-id="eb3f9-131">id</span></span>|<span data-ttu-id="eb3f9-132">String</span><span class="sxs-lookup"><span data-stu-id="eb3f9-132">String</span></span>|<span data-ttu-id="eb3f9-133">Eindeutiger Bezeichner für die WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="eb3f9-133">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="eb3f9-134">applicationName</span><span class="sxs-lookup"><span data-stu-id="eb3f9-134">applicationName</span></span>|<span data-ttu-id="eb3f9-135">String</span><span class="sxs-lookup"><span data-stu-id="eb3f9-135">String</span></span>|<span data-ttu-id="eb3f9-136">Name der Anwendung</span><span class="sxs-lookup"><span data-stu-id="eb3f9-136">Application Name</span></span>|
|<span data-ttu-id="eb3f9-137">applicationType</span><span class="sxs-lookup"><span data-stu-id="eb3f9-137">applicationType</span></span>|[<span data-ttu-id="eb3f9-138">applicationType</span><span class="sxs-lookup"><span data-stu-id="eb3f9-138">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="eb3f9-139">Anwendungstyp.</span><span class="sxs-lookup"><span data-stu-id="eb3f9-139">Application Type.</span></span> <span data-ttu-id="eb3f9-140">Mögliche Werte sind: `universal` und `desktop`.</span><span class="sxs-lookup"><span data-stu-id="eb3f9-140">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="eb3f9-141">deviceCount</span><span class="sxs-lookup"><span data-stu-id="eb3f9-141">deviceCount</span></span>|<span data-ttu-id="eb3f9-142">Int32</span><span class="sxs-lookup"><span data-stu-id="eb3f9-142">Int32</span></span>|<span data-ttu-id="eb3f9-143">Geräteanzahl</span><span class="sxs-lookup"><span data-stu-id="eb3f9-143">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="eb3f9-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb3f9-144">Response</span></span>
<span data-ttu-id="eb3f9-145">Wenn erfolgreich, gibt diese Methode den `201 Created`-Antwortcode und das [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="eb3f9-145">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb3f9-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eb3f9-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="eb3f9-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb3f9-147">Request</span></span>
<span data-ttu-id="eb3f9-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="eb3f9-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionAppLearningSummaries
Content-type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="eb3f9-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb3f9-149">Response</span></span>
<span data-ttu-id="eb3f9-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eb3f9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 240

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "id": "063baf50-af50-063b-50af-3b0650af3b06",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```



