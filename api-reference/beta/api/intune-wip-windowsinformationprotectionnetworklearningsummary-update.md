---
title: windowsInformationProtectionNetworkLearningSummary aktualisieren
description: Aktualisieren der Eigenschaften eines windowsInformationProtectionNetworkLearningSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 68c2bf244ac650c682b303633e28d5d5b8bbca1e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30972144"
---
# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="859d1-103">windowsInformationProtectionNetworkLearningSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="859d1-103">Update windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="859d1-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="859d1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="859d1-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="859d1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="859d1-106">Aktualisieren der Eigenschaften eines [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="859d1-106">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="859d1-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="859d1-107">Prerequisites</span></span>
<span data-ttu-id="859d1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="859d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="859d1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="859d1-110">Permission type</span></span>|<span data-ttu-id="859d1-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="859d1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="859d1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="859d1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="859d1-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="859d1-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="859d1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="859d1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="859d1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="859d1-115">Not supported.</span></span>|
|<span data-ttu-id="859d1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="859d1-116">Application</span></span>|<span data-ttu-id="859d1-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="859d1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="859d1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="859d1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="859d1-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="859d1-119">Request headers</span></span>
|<span data-ttu-id="859d1-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="859d1-120">Header</span></span>|<span data-ttu-id="859d1-121">Wert</span><span class="sxs-lookup"><span data-stu-id="859d1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="859d1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="859d1-122">Authorization</span></span>|<span data-ttu-id="859d1-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="859d1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="859d1-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="859d1-124">Accept</span></span>|<span data-ttu-id="859d1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="859d1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="859d1-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="859d1-126">Request body</span></span>
<span data-ttu-id="859d1-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)-Objekt ein.</span><span class="sxs-lookup"><span data-stu-id="859d1-127">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="859d1-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="859d1-128">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="859d1-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="859d1-129">Property</span></span>|<span data-ttu-id="859d1-130">Typ</span><span class="sxs-lookup"><span data-stu-id="859d1-130">Type</span></span>|<span data-ttu-id="859d1-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="859d1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="859d1-132">id</span><span class="sxs-lookup"><span data-stu-id="859d1-132">id</span></span>|<span data-ttu-id="859d1-133">String</span><span class="sxs-lookup"><span data-stu-id="859d1-133">String</span></span>|<span data-ttu-id="859d1-134">Eindeutiger Bezeichner für die WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="859d1-134">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="859d1-135">url</span><span class="sxs-lookup"><span data-stu-id="859d1-135">url</span></span>|<span data-ttu-id="859d1-136">String</span><span class="sxs-lookup"><span data-stu-id="859d1-136">String</span></span>|<span data-ttu-id="859d1-137">Website-URL</span><span class="sxs-lookup"><span data-stu-id="859d1-137">Website url</span></span>|
|<span data-ttu-id="859d1-138">deviceCount</span><span class="sxs-lookup"><span data-stu-id="859d1-138">deviceCount</span></span>|<span data-ttu-id="859d1-139">Int32</span><span class="sxs-lookup"><span data-stu-id="859d1-139">Int32</span></span>|<span data-ttu-id="859d1-140">Geräteanzahl</span><span class="sxs-lookup"><span data-stu-id="859d1-140">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="859d1-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="859d1-141">Response</span></span>
<span data-ttu-id="859d1-142">Wenn erfolgreich, gibt diese Methode den `200 OK`-Antwortcode und das aktualisierte [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="859d1-142">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="859d1-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="859d1-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="859d1-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="859d1-144">Request</span></span>
<span data-ttu-id="859d1-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="859d1-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="859d1-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="859d1-146">Response</span></span>
<span data-ttu-id="859d1-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="859d1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 186

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "242108f7-08f7-2421-f708-2124f7082124",
  "url": "Url value",
  "deviceCount": 11
}
```




