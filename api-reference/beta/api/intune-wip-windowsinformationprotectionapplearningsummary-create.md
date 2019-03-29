---
title: windowsInformationProtectionAppLearningSummary erstellen
description: Erstellen eines neuen windowsInformationProtectionAppLearningSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5721e88ac59dfcfa4e7c0bd6faa5393feea0b464
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30976400"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="afe6c-103">windowsInformationProtectionAppLearningSummary erstellen</span><span class="sxs-lookup"><span data-stu-id="afe6c-103">Create windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="afe6c-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="afe6c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="afe6c-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="afe6c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="afe6c-106">Erstellen eines neuen [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="afe6c-106">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="afe6c-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="afe6c-107">Prerequisites</span></span>
<span data-ttu-id="afe6c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afe6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afe6c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="afe6c-110">Permission type</span></span>|<span data-ttu-id="afe6c-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="afe6c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="afe6c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="afe6c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="afe6c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afe6c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="afe6c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="afe6c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="afe6c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="afe6c-115">Not supported.</span></span>|
|<span data-ttu-id="afe6c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="afe6c-116">Application</span></span>|<span data-ttu-id="afe6c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="afe6c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="afe6c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="afe6c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="afe6c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="afe6c-119">Request headers</span></span>
|<span data-ttu-id="afe6c-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="afe6c-120">Header</span></span>|<span data-ttu-id="afe6c-121">Wert</span><span class="sxs-lookup"><span data-stu-id="afe6c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="afe6c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="afe6c-122">Authorization</span></span>|<span data-ttu-id="afe6c-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="afe6c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="afe6c-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="afe6c-124">Accept</span></span>|<span data-ttu-id="afe6c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="afe6c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="afe6c-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="afe6c-126">Request body</span></span>
<span data-ttu-id="afe6c-127">Geben Sie im Anforderungstext eine JSON-Darstellung des windowsInformationProtectionAppLearningSummary-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="afe6c-127">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="afe6c-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsInformationProtectionAppLearningSummary erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="afe6c-128">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="afe6c-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="afe6c-129">Property</span></span>|<span data-ttu-id="afe6c-130">Typ</span><span class="sxs-lookup"><span data-stu-id="afe6c-130">Type</span></span>|<span data-ttu-id="afe6c-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="afe6c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afe6c-132">id</span><span class="sxs-lookup"><span data-stu-id="afe6c-132">id</span></span>|<span data-ttu-id="afe6c-133">String</span><span class="sxs-lookup"><span data-stu-id="afe6c-133">String</span></span>|<span data-ttu-id="afe6c-134">Eindeutiger Bezeichner für die WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="afe6c-134">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="afe6c-135">applicationName</span><span class="sxs-lookup"><span data-stu-id="afe6c-135">applicationName</span></span>|<span data-ttu-id="afe6c-136">String</span><span class="sxs-lookup"><span data-stu-id="afe6c-136">String</span></span>|<span data-ttu-id="afe6c-137">Name der Anwendung</span><span class="sxs-lookup"><span data-stu-id="afe6c-137">Application Name</span></span>|
|<span data-ttu-id="afe6c-138">applicationType</span><span class="sxs-lookup"><span data-stu-id="afe6c-138">applicationType</span></span>|[<span data-ttu-id="afe6c-139">applicationtype</span><span class="sxs-lookup"><span data-stu-id="afe6c-139">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="afe6c-140">Anwendungstyp.</span><span class="sxs-lookup"><span data-stu-id="afe6c-140">Application Type.</span></span> <span data-ttu-id="afe6c-141">Mögliche Werte sind: `universal` und `desktop`.</span><span class="sxs-lookup"><span data-stu-id="afe6c-141">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="afe6c-142">deviceCount</span><span class="sxs-lookup"><span data-stu-id="afe6c-142">deviceCount</span></span>|<span data-ttu-id="afe6c-143">Int32</span><span class="sxs-lookup"><span data-stu-id="afe6c-143">Int32</span></span>|<span data-ttu-id="afe6c-144">Geräteanzahl</span><span class="sxs-lookup"><span data-stu-id="afe6c-144">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="afe6c-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="afe6c-145">Response</span></span>
<span data-ttu-id="afe6c-146">Wenn erfolgreich, gibt diese Methode den `201 Created`-Antwortcode und das [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="afe6c-146">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afe6c-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="afe6c-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="afe6c-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="afe6c-148">Request</span></span>
<span data-ttu-id="afe6c-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="afe6c-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="afe6c-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="afe6c-150">Response</span></span>
<span data-ttu-id="afe6c-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="afe6c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




