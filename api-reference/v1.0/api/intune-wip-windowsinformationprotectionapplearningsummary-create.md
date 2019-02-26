---
title: windowsInformationProtectionAppLearningSummary erstellen
description: Erstellen eines neuen windowsInformationProtectionAppLearningSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 30cfe88f6e0a8a72e1a373b0f867357c63138f42
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260256"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="411fa-103">windowsInformationProtectionAppLearningSummary erstellen</span><span class="sxs-lookup"><span data-stu-id="411fa-103">Create windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="411fa-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="411fa-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="411fa-105">Erstellen eines neuen [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="411fa-105">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="411fa-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="411fa-106">Prerequisites</span></span>
<span data-ttu-id="411fa-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="411fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="411fa-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="411fa-109">Permission type</span></span>|<span data-ttu-id="411fa-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="411fa-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="411fa-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="411fa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="411fa-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="411fa-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="411fa-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="411fa-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="411fa-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="411fa-114">Not supported.</span></span>|
|<span data-ttu-id="411fa-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="411fa-115">Application</span></span>|<span data-ttu-id="411fa-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="411fa-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="411fa-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="411fa-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="411fa-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="411fa-118">Request headers</span></span>
|<span data-ttu-id="411fa-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="411fa-119">Header</span></span>|<span data-ttu-id="411fa-120">Wert</span><span class="sxs-lookup"><span data-stu-id="411fa-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="411fa-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="411fa-121">Authorization</span></span>|<span data-ttu-id="411fa-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="411fa-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="411fa-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="411fa-123">Accept</span></span>|<span data-ttu-id="411fa-124">application/json</span><span class="sxs-lookup"><span data-stu-id="411fa-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="411fa-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="411fa-125">Request body</span></span>
<span data-ttu-id="411fa-126">Geben Sie im Anforderungstext eine JSON-Darstellung des windowsInformationProtectionAppLearningSummary-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="411fa-126">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="411fa-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsInformationProtectionAppLearningSummary erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="411fa-127">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="411fa-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="411fa-128">Property</span></span>|<span data-ttu-id="411fa-129">Typ</span><span class="sxs-lookup"><span data-stu-id="411fa-129">Type</span></span>|<span data-ttu-id="411fa-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="411fa-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="411fa-131">id</span><span class="sxs-lookup"><span data-stu-id="411fa-131">id</span></span>|<span data-ttu-id="411fa-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="411fa-132">String</span></span>|<span data-ttu-id="411fa-133">Eindeutiger Bezeichner für die WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="411fa-133">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="411fa-134">applicationName</span><span class="sxs-lookup"><span data-stu-id="411fa-134">applicationName</span></span>|<span data-ttu-id="411fa-135">String</span><span class="sxs-lookup"><span data-stu-id="411fa-135">String</span></span>|<span data-ttu-id="411fa-136">Name der Anwendung</span><span class="sxs-lookup"><span data-stu-id="411fa-136">Application Name</span></span>|
|<span data-ttu-id="411fa-137">applicationType</span><span class="sxs-lookup"><span data-stu-id="411fa-137">applicationType</span></span>|[<span data-ttu-id="411fa-138">applicationType</span><span class="sxs-lookup"><span data-stu-id="411fa-138">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="411fa-139">Anwendungstyp.</span><span class="sxs-lookup"><span data-stu-id="411fa-139">Application Type.</span></span> <span data-ttu-id="411fa-140">Mögliche Werte sind: `universal` und `desktop`.</span><span class="sxs-lookup"><span data-stu-id="411fa-140">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="411fa-141">deviceCount</span><span class="sxs-lookup"><span data-stu-id="411fa-141">deviceCount</span></span>|<span data-ttu-id="411fa-142">Int32</span><span class="sxs-lookup"><span data-stu-id="411fa-142">Int32</span></span>|<span data-ttu-id="411fa-143">Geräteanzahl</span><span class="sxs-lookup"><span data-stu-id="411fa-143">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="411fa-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="411fa-144">Response</span></span>
<span data-ttu-id="411fa-145">Wenn erfolgreich, gibt diese Methode den `201 Created`-Antwortcode und das [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="411fa-145">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="411fa-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="411fa-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="411fa-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="411fa-147">Request</span></span>
<span data-ttu-id="411fa-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="411fa-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="411fa-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="411fa-149">Response</span></span>
<span data-ttu-id="411fa-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="411fa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



