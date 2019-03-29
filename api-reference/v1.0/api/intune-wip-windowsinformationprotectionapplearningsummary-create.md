---
title: windowsInformationProtectionAppLearningSummary erstellen
description: Erstellen eines neuen windowsInformationProtectionAppLearningSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 43f36e67ea0d1ec46708bcac1e5ecdf528f35c5b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30959474"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="46b47-103">windowsInformationProtectionAppLearningSummary erstellen</span><span class="sxs-lookup"><span data-stu-id="46b47-103">Create windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="46b47-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="46b47-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46b47-105">Erstellen eines neuen [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="46b47-105">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46b47-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="46b47-106">Prerequisites</span></span>
<span data-ttu-id="46b47-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46b47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46b47-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="46b47-109">Permission type</span></span>|<span data-ttu-id="46b47-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="46b47-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46b47-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="46b47-111">Delegated (work or school account)</span></span>|<span data-ttu-id="46b47-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46b47-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="46b47-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="46b47-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46b47-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="46b47-114">Not supported.</span></span>|
|<span data-ttu-id="46b47-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="46b47-115">Application</span></span>|<span data-ttu-id="46b47-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="46b47-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46b47-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="46b47-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="46b47-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="46b47-118">Request headers</span></span>
|<span data-ttu-id="46b47-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="46b47-119">Header</span></span>|<span data-ttu-id="46b47-120">Wert</span><span class="sxs-lookup"><span data-stu-id="46b47-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46b47-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="46b47-121">Authorization</span></span>|<span data-ttu-id="46b47-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="46b47-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46b47-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="46b47-123">Accept</span></span>|<span data-ttu-id="46b47-124">application/json</span><span class="sxs-lookup"><span data-stu-id="46b47-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46b47-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="46b47-125">Request body</span></span>
<span data-ttu-id="46b47-126">Geben Sie im Anforderungstext eine JSON-Darstellung des windowsInformationProtectionAppLearningSummary-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="46b47-126">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="46b47-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsInformationProtectionAppLearningSummary erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="46b47-127">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="46b47-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="46b47-128">Property</span></span>|<span data-ttu-id="46b47-129">Typ</span><span class="sxs-lookup"><span data-stu-id="46b47-129">Type</span></span>|<span data-ttu-id="46b47-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="46b47-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46b47-131">id</span><span class="sxs-lookup"><span data-stu-id="46b47-131">id</span></span>|<span data-ttu-id="46b47-132">String</span><span class="sxs-lookup"><span data-stu-id="46b47-132">String</span></span>|<span data-ttu-id="46b47-133">Eindeutiger Bezeichner für die WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="46b47-133">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="46b47-134">applicationName</span><span class="sxs-lookup"><span data-stu-id="46b47-134">applicationName</span></span>|<span data-ttu-id="46b47-135">String</span><span class="sxs-lookup"><span data-stu-id="46b47-135">String</span></span>|<span data-ttu-id="46b47-136">Name der Anwendung</span><span class="sxs-lookup"><span data-stu-id="46b47-136">Application Name</span></span>|
|<span data-ttu-id="46b47-137">applicationType</span><span class="sxs-lookup"><span data-stu-id="46b47-137">applicationType</span></span>|[<span data-ttu-id="46b47-138">applicationtype</span><span class="sxs-lookup"><span data-stu-id="46b47-138">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="46b47-139">Anwendungstyp.</span><span class="sxs-lookup"><span data-stu-id="46b47-139">Application Type.</span></span> <span data-ttu-id="46b47-140">Mögliche Werte sind: `universal` und `desktop`.</span><span class="sxs-lookup"><span data-stu-id="46b47-140">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="46b47-141">deviceCount</span><span class="sxs-lookup"><span data-stu-id="46b47-141">deviceCount</span></span>|<span data-ttu-id="46b47-142">Int32</span><span class="sxs-lookup"><span data-stu-id="46b47-142">Int32</span></span>|<span data-ttu-id="46b47-143">Geräteanzahl</span><span class="sxs-lookup"><span data-stu-id="46b47-143">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="46b47-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="46b47-144">Response</span></span>
<span data-ttu-id="46b47-145">Wenn erfolgreich, gibt diese Methode den `201 Created`-Antwortcode und das [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="46b47-145">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46b47-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="46b47-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="46b47-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="46b47-147">Request</span></span>
<span data-ttu-id="46b47-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="46b47-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="46b47-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="46b47-149">Response</span></span>
<span data-ttu-id="46b47-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="46b47-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



