---
title: windowsInformationProtectionAppLearningSummary aktualisieren
description: Aktualisieren der Eigenschaften eines windowsInformationProtectionAppLearningSummary-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 05119960dd66ef28438bdcbe8bcaa5d9c64bebf2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407270"
---
# <a name="update-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="1410c-103">windowsInformationProtectionAppLearningSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1410c-103">Update windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="1410c-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="1410c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1410c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1410c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1410c-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1410c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1410c-107">Aktualisieren der Eigenschaften eines [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1410c-107">Update the properties of a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1410c-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1410c-108">Prerequisites</span></span>
<span data-ttu-id="1410c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1410c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1410c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1410c-111">Permission type</span></span>|<span data-ttu-id="1410c-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1410c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1410c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1410c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1410c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1410c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1410c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1410c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1410c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1410c-116">Not supported.</span></span>|
|<span data-ttu-id="1410c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1410c-117">Application</span></span>|<span data-ttu-id="1410c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1410c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1410c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1410c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="1410c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1410c-120">Request headers</span></span>
|<span data-ttu-id="1410c-121">Header</span><span class="sxs-lookup"><span data-stu-id="1410c-121">Header</span></span>|<span data-ttu-id="1410c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="1410c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1410c-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1410c-123">Authorization</span></span>|<span data-ttu-id="1410c-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1410c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1410c-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1410c-125">Accept</span></span>|<span data-ttu-id="1410c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1410c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1410c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1410c-127">Request body</span></span>
<span data-ttu-id="1410c-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="1410c-128">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

<span data-ttu-id="1410c-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="1410c-129">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span></span>

|<span data-ttu-id="1410c-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1410c-130">Property</span></span>|<span data-ttu-id="1410c-131">Typ</span><span class="sxs-lookup"><span data-stu-id="1410c-131">Type</span></span>|<span data-ttu-id="1410c-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1410c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1410c-133">id</span><span class="sxs-lookup"><span data-stu-id="1410c-133">id</span></span>|<span data-ttu-id="1410c-134">String</span><span class="sxs-lookup"><span data-stu-id="1410c-134">String</span></span>|<span data-ttu-id="1410c-135">Eindeutiger Bezeichner für die WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="1410c-135">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="1410c-136">applicationName</span><span class="sxs-lookup"><span data-stu-id="1410c-136">applicationName</span></span>|<span data-ttu-id="1410c-137">String</span><span class="sxs-lookup"><span data-stu-id="1410c-137">String</span></span>|<span data-ttu-id="1410c-138">Name der Anwendung</span><span class="sxs-lookup"><span data-stu-id="1410c-138">Application Name</span></span>|
|<span data-ttu-id="1410c-139">applicationType</span><span class="sxs-lookup"><span data-stu-id="1410c-139">applicationType</span></span>|[<span data-ttu-id="1410c-140">applicationType</span><span class="sxs-lookup"><span data-stu-id="1410c-140">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="1410c-141">Anwendungstyp.</span><span class="sxs-lookup"><span data-stu-id="1410c-141">Application Type.</span></span> <span data-ttu-id="1410c-142">Mögliche Werte sind: `universal` und `desktop`.</span><span class="sxs-lookup"><span data-stu-id="1410c-142">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="1410c-143">deviceCount</span><span class="sxs-lookup"><span data-stu-id="1410c-143">deviceCount</span></span>|<span data-ttu-id="1410c-144">Int32</span><span class="sxs-lookup"><span data-stu-id="1410c-144">Int32</span></span>|<span data-ttu-id="1410c-145">Geräteanzahl</span><span class="sxs-lookup"><span data-stu-id="1410c-145">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="1410c-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="1410c-146">Response</span></span>
<span data-ttu-id="1410c-147">Wenn erfolgreich, gibt diese Methode den `200 OK`-Antwortcode und das aktualisierte [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1410c-147">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1410c-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1410c-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="1410c-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1410c-149">Request</span></span>
<span data-ttu-id="1410c-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1410c-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
Content-type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="1410c-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="1410c-151">Response</span></span>
<span data-ttu-id="1410c-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1410c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




