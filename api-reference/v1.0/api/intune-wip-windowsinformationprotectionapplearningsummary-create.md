---
title: windowsInformationProtectionAppLearningSummary erstellen
description: Erstellen eines neuen windowsInformationProtectionAppLearningSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 498b6da245cbf805ef4c106447f73e56837a43e9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810556"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="7c927-103">windowsInformationProtectionAppLearningSummary erstellen</span><span class="sxs-lookup"><span data-stu-id="7c927-103">Create windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="7c927-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7c927-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7c927-105">Erstellen eines neuen [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="7c927-105">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7c927-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7c927-106">Prerequisites</span></span>
<span data-ttu-id="7c927-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c927-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c927-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7c927-109">Permission type</span></span>|<span data-ttu-id="7c927-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7c927-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c927-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7c927-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7c927-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c927-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7c927-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7c927-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c927-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c927-114">Not supported.</span></span>|
|<span data-ttu-id="7c927-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7c927-115">Application</span></span>|<span data-ttu-id="7c927-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c927-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c927-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c927-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="7c927-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7c927-118">Request headers</span></span>
|<span data-ttu-id="7c927-119">Header</span><span class="sxs-lookup"><span data-stu-id="7c927-119">Header</span></span>|<span data-ttu-id="7c927-120">Wert</span><span class="sxs-lookup"><span data-stu-id="7c927-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c927-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c927-121">Authorization</span></span>|<span data-ttu-id="7c927-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7c927-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c927-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7c927-123">Accept</span></span>|<span data-ttu-id="7c927-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7c927-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c927-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7c927-125">Request body</span></span>
<span data-ttu-id="7c927-126">Geben Sie im Anforderungstext eine JSON-Darstellung des windowsInformationProtectionAppLearningSummary-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="7c927-126">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="7c927-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsInformationProtectionAppLearningSummary erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="7c927-127">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="7c927-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7c927-128">Property</span></span>|<span data-ttu-id="7c927-129">Typ</span><span class="sxs-lookup"><span data-stu-id="7c927-129">Type</span></span>|<span data-ttu-id="7c927-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7c927-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c927-131">id</span><span class="sxs-lookup"><span data-stu-id="7c927-131">id</span></span>|<span data-ttu-id="7c927-132">String</span><span class="sxs-lookup"><span data-stu-id="7c927-132">String</span></span>|<span data-ttu-id="7c927-133">Eindeutiger Bezeichner für die WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="7c927-133">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="7c927-134">applicationName</span><span class="sxs-lookup"><span data-stu-id="7c927-134">applicationName</span></span>|<span data-ttu-id="7c927-135">String</span><span class="sxs-lookup"><span data-stu-id="7c927-135">String</span></span>|<span data-ttu-id="7c927-136">Name der Anwendung</span><span class="sxs-lookup"><span data-stu-id="7c927-136">Application Name</span></span>|
|<span data-ttu-id="7c927-137">applicationType</span><span class="sxs-lookup"><span data-stu-id="7c927-137">applicationType</span></span>|[<span data-ttu-id="7c927-138">applicationType</span><span class="sxs-lookup"><span data-stu-id="7c927-138">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="7c927-139">Anwendungstyp.</span><span class="sxs-lookup"><span data-stu-id="7c927-139">Application Type.</span></span> <span data-ttu-id="7c927-140">Mögliche Werte sind: `universal` und `desktop`.</span><span class="sxs-lookup"><span data-stu-id="7c927-140">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="7c927-141">deviceCount</span><span class="sxs-lookup"><span data-stu-id="7c927-141">deviceCount</span></span>|<span data-ttu-id="7c927-142">Int32</span><span class="sxs-lookup"><span data-stu-id="7c927-142">Int32</span></span>|<span data-ttu-id="7c927-143">Geräteanzahl</span><span class="sxs-lookup"><span data-stu-id="7c927-143">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="7c927-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c927-144">Response</span></span>
<span data-ttu-id="7c927-145">Wenn erfolgreich, gibt diese Methode den `201 Created`-Antwortcode und das [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7c927-145">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c927-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7c927-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="7c927-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c927-147">Request</span></span>
<span data-ttu-id="7c927-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7c927-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7c927-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c927-149">Response</span></span>
<span data-ttu-id="7c927-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7c927-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



