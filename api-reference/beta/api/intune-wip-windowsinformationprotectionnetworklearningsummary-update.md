---
title: windowsInformationProtectionNetworkLearningSummary aktualisieren
description: Aktualisieren der Eigenschaften eines windowsInformationProtectionNetworkLearningSummary-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 05c59d3bc28f5a0c29a33f1a0046b18331f46570
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409223"
---
# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="5f5f7-103">windowsInformationProtectionNetworkLearningSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="5f5f7-103">Update windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="5f5f7-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="5f5f7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5f5f7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f5f7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5f5f7-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5f5f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f5f7-107">Aktualisieren der Eigenschaften eines [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="5f5f7-107">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5f5f7-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5f5f7-108">Prerequisites</span></span>
<span data-ttu-id="5f5f7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5f5f7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5f5f7-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5f5f7-111">Permission type</span></span>|<span data-ttu-id="5f5f7-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5f5f7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f5f7-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5f5f7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5f5f7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f5f7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5f5f7-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5f5f7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f5f7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5f5f7-116">Not supported.</span></span>|
|<span data-ttu-id="5f5f7-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5f5f7-117">Application</span></span>|<span data-ttu-id="5f5f7-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5f5f7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f5f7-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5f5f7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="5f5f7-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5f5f7-120">Request headers</span></span>
|<span data-ttu-id="5f5f7-121">Header</span><span class="sxs-lookup"><span data-stu-id="5f5f7-121">Header</span></span>|<span data-ttu-id="5f5f7-122">Wert</span><span class="sxs-lookup"><span data-stu-id="5f5f7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f5f7-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="5f5f7-123">Authorization</span></span>|<span data-ttu-id="5f5f7-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5f5f7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f5f7-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5f5f7-125">Accept</span></span>|<span data-ttu-id="5f5f7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5f5f7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f5f7-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5f5f7-127">Request body</span></span>
<span data-ttu-id="5f5f7-128">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)-Objekt ein.</span><span class="sxs-lookup"><span data-stu-id="5f5f7-128">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="5f5f7-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="5f5f7-129">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="5f5f7-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5f5f7-130">Property</span></span>|<span data-ttu-id="5f5f7-131">Typ</span><span class="sxs-lookup"><span data-stu-id="5f5f7-131">Type</span></span>|<span data-ttu-id="5f5f7-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5f5f7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f5f7-133">id</span><span class="sxs-lookup"><span data-stu-id="5f5f7-133">id</span></span>|<span data-ttu-id="5f5f7-134">String</span><span class="sxs-lookup"><span data-stu-id="5f5f7-134">String</span></span>|<span data-ttu-id="5f5f7-135">Eindeutiger Bezeichner für die WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="5f5f7-135">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="5f5f7-136">url</span><span class="sxs-lookup"><span data-stu-id="5f5f7-136">url</span></span>|<span data-ttu-id="5f5f7-137">String</span><span class="sxs-lookup"><span data-stu-id="5f5f7-137">String</span></span>|<span data-ttu-id="5f5f7-138">Website-URL</span><span class="sxs-lookup"><span data-stu-id="5f5f7-138">Website url</span></span>|
|<span data-ttu-id="5f5f7-139">deviceCount</span><span class="sxs-lookup"><span data-stu-id="5f5f7-139">deviceCount</span></span>|<span data-ttu-id="5f5f7-140">Int32</span><span class="sxs-lookup"><span data-stu-id="5f5f7-140">Int32</span></span>|<span data-ttu-id="5f5f7-141">Geräteanzahl</span><span class="sxs-lookup"><span data-stu-id="5f5f7-141">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="5f5f7-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="5f5f7-142">Response</span></span>
<span data-ttu-id="5f5f7-143">Wenn erfolgreich, gibt diese Methode den `200 OK`-Antwortcode und das aktualisierte [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5f5f7-143">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f5f7-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5f5f7-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f5f7-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5f5f7-145">Request</span></span>
<span data-ttu-id="5f5f7-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5f5f7-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5f5f7-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="5f5f7-147">Response</span></span>
<span data-ttu-id="5f5f7-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5f5f7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




