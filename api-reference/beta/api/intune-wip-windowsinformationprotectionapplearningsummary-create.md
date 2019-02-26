---
title: windowsInformationProtectionAppLearningSummary erstellen
description: Erstellen eines neuen windowsInformationProtectionAppLearningSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 165664c3977ede205c406da712d5a331ff9de7c7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174657"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="4ecec-103">windowsInformationProtectionAppLearningSummary erstellen</span><span class="sxs-lookup"><span data-stu-id="4ecec-103">Create windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="4ecec-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4ecec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ecec-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4ecec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ecec-106">Erstellen eines neuen [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="4ecec-106">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ecec-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4ecec-107">Prerequisites</span></span>
<span data-ttu-id="4ecec-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4ecec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4ecec-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4ecec-110">Permission type</span></span>|<span data-ttu-id="4ecec-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4ecec-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ecec-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4ecec-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4ecec-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ecec-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4ecec-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4ecec-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ecec-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4ecec-115">Not supported.</span></span>|
|<span data-ttu-id="4ecec-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4ecec-116">Application</span></span>|<span data-ttu-id="4ecec-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4ecec-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ecec-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4ecec-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="4ecec-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4ecec-119">Request headers</span></span>
|<span data-ttu-id="4ecec-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4ecec-120">Header</span></span>|<span data-ttu-id="4ecec-121">Wert</span><span class="sxs-lookup"><span data-stu-id="4ecec-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ecec-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ecec-122">Authorization</span></span>|<span data-ttu-id="4ecec-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4ecec-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ecec-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4ecec-124">Accept</span></span>|<span data-ttu-id="4ecec-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4ecec-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ecec-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4ecec-126">Request body</span></span>
<span data-ttu-id="4ecec-127">Geben Sie im Anforderungstext eine JSON-Darstellung des windowsInformationProtectionAppLearningSummary-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="4ecec-127">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="4ecec-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsInformationProtectionAppLearningSummary erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="4ecec-128">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="4ecec-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4ecec-129">Property</span></span>|<span data-ttu-id="4ecec-130">Typ</span><span class="sxs-lookup"><span data-stu-id="4ecec-130">Type</span></span>|<span data-ttu-id="4ecec-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4ecec-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ecec-132">id</span><span class="sxs-lookup"><span data-stu-id="4ecec-132">id</span></span>|<span data-ttu-id="4ecec-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4ecec-133">String</span></span>|<span data-ttu-id="4ecec-134">Eindeutiger Bezeichner für die WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="4ecec-134">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="4ecec-135">applicationName</span><span class="sxs-lookup"><span data-stu-id="4ecec-135">applicationName</span></span>|<span data-ttu-id="4ecec-136">String</span><span class="sxs-lookup"><span data-stu-id="4ecec-136">String</span></span>|<span data-ttu-id="4ecec-137">Name der Anwendung</span><span class="sxs-lookup"><span data-stu-id="4ecec-137">Application Name</span></span>|
|<span data-ttu-id="4ecec-138">applicationType</span><span class="sxs-lookup"><span data-stu-id="4ecec-138">applicationType</span></span>|[<span data-ttu-id="4ecec-139">applicationType</span><span class="sxs-lookup"><span data-stu-id="4ecec-139">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="4ecec-140">Anwendungstyp.</span><span class="sxs-lookup"><span data-stu-id="4ecec-140">Application Type.</span></span> <span data-ttu-id="4ecec-141">Mögliche Werte sind: `universal` und `desktop`.</span><span class="sxs-lookup"><span data-stu-id="4ecec-141">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="4ecec-142">deviceCount</span><span class="sxs-lookup"><span data-stu-id="4ecec-142">deviceCount</span></span>|<span data-ttu-id="4ecec-143">Int32</span><span class="sxs-lookup"><span data-stu-id="4ecec-143">Int32</span></span>|<span data-ttu-id="4ecec-144">Geräteanzahl</span><span class="sxs-lookup"><span data-stu-id="4ecec-144">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="4ecec-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="4ecec-145">Response</span></span>
<span data-ttu-id="4ecec-146">Wenn erfolgreich, gibt diese Methode den `201 Created`-Antwortcode und das [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4ecec-146">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ecec-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4ecec-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ecec-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4ecec-148">Request</span></span>
<span data-ttu-id="4ecec-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4ecec-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionAppLearningSummaries
Content-type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="4ecec-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="4ecec-150">Response</span></span>
<span data-ttu-id="4ecec-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4ecec-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




