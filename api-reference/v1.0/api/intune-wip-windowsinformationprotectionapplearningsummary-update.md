---
title: windowsInformationProtectionAppLearningSummary aktualisieren
description: Aktualisieren der Eigenschaften eines windowsInformationProtectionAppLearningSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 66f144c801c720289f52c5bfc8963e625065cb6f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940596"
---
# <a name="update-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="d44b1-103">windowsInformationProtectionAppLearningSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d44b1-103">Update windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="d44b1-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d44b1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d44b1-105">Aktualisieren der Eigenschaften eines [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d44b1-105">Update the properties of a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d44b1-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d44b1-106">Prerequisites</span></span>
<span data-ttu-id="d44b1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d44b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d44b1-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d44b1-109">Permission type</span></span>|<span data-ttu-id="d44b1-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d44b1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d44b1-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d44b1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d44b1-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d44b1-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d44b1-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d44b1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d44b1-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d44b1-114">Not supported.</span></span>|
|<span data-ttu-id="d44b1-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d44b1-115">Application</span></span>|<span data-ttu-id="d44b1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d44b1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d44b1-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d44b1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="d44b1-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d44b1-118">Request headers</span></span>
|<span data-ttu-id="d44b1-119">Header</span><span class="sxs-lookup"><span data-stu-id="d44b1-119">Header</span></span>|<span data-ttu-id="d44b1-120">Wert</span><span class="sxs-lookup"><span data-stu-id="d44b1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d44b1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d44b1-121">Authorization</span></span>|<span data-ttu-id="d44b1-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d44b1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d44b1-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d44b1-123">Accept</span></span>|<span data-ttu-id="d44b1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d44b1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d44b1-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d44b1-125">Request body</span></span>
<span data-ttu-id="d44b1-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="d44b1-126">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

<span data-ttu-id="d44b1-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="d44b1-127">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span></span>

|<span data-ttu-id="d44b1-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d44b1-128">Property</span></span>|<span data-ttu-id="d44b1-129">Typ</span><span class="sxs-lookup"><span data-stu-id="d44b1-129">Type</span></span>|<span data-ttu-id="d44b1-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d44b1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d44b1-131">id</span><span class="sxs-lookup"><span data-stu-id="d44b1-131">id</span></span>|<span data-ttu-id="d44b1-132">String</span><span class="sxs-lookup"><span data-stu-id="d44b1-132">String</span></span>|<span data-ttu-id="d44b1-133">Eindeutiger Bezeichner für die WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="d44b1-133">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="d44b1-134">applicationName</span><span class="sxs-lookup"><span data-stu-id="d44b1-134">applicationName</span></span>|<span data-ttu-id="d44b1-135">String</span><span class="sxs-lookup"><span data-stu-id="d44b1-135">String</span></span>|<span data-ttu-id="d44b1-136">Name der Anwendung</span><span class="sxs-lookup"><span data-stu-id="d44b1-136">Application Name</span></span>|
|<span data-ttu-id="d44b1-137">applicationType</span><span class="sxs-lookup"><span data-stu-id="d44b1-137">applicationType</span></span>|[<span data-ttu-id="d44b1-138">applicationType</span><span class="sxs-lookup"><span data-stu-id="d44b1-138">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="d44b1-139">Anwendungstyp.</span><span class="sxs-lookup"><span data-stu-id="d44b1-139">Application Type.</span></span> <span data-ttu-id="d44b1-140">Mögliche Werte sind: `universal` und `desktop`.</span><span class="sxs-lookup"><span data-stu-id="d44b1-140">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="d44b1-141">deviceCount</span><span class="sxs-lookup"><span data-stu-id="d44b1-141">deviceCount</span></span>|<span data-ttu-id="d44b1-142">Int32</span><span class="sxs-lookup"><span data-stu-id="d44b1-142">Int32</span></span>|<span data-ttu-id="d44b1-143">Geräteanzahl</span><span class="sxs-lookup"><span data-stu-id="d44b1-143">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="d44b1-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="d44b1-144">Response</span></span>
<span data-ttu-id="d44b1-145">Wenn erfolgreich, gibt diese Methode den `200 OK`-Antwortcode und das aktualisierte [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d44b1-145">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d44b1-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d44b1-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="d44b1-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d44b1-147">Request</span></span>
<span data-ttu-id="d44b1-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d44b1-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
Content-type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="d44b1-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="d44b1-149">Response</span></span>
<span data-ttu-id="d44b1-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d44b1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



