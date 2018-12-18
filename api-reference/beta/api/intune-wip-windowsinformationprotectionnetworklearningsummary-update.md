---
title: windowsInformationProtectionNetworkLearningSummary aktualisieren
description: Aktualisieren der Eigenschaften eines windowsInformationProtectionNetworkLearningSummary-Objekts.
author: tfitzmac
ms.openlocfilehash: 335fee7e664000584fa4542985a3b014d827f0d9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344436"
---
# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="3dd42-103">windowsInformationProtectionNetworkLearningSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="3dd42-103">Update windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="3dd42-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3dd42-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3dd42-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3dd42-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3dd42-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3dd42-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3dd42-107">Aktualisieren der Eigenschaften eines [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="3dd42-107">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3dd42-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3dd42-108">Prerequisites</span></span>
<span data-ttu-id="3dd42-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3dd42-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3dd42-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3dd42-111">Permission type</span></span>|<span data-ttu-id="3dd42-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3dd42-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3dd42-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3dd42-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3dd42-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3dd42-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3dd42-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3dd42-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3dd42-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3dd42-116">Not supported.</span></span>|
|<span data-ttu-id="3dd42-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3dd42-117">Application</span></span>|<span data-ttu-id="3dd42-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3dd42-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3dd42-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3dd42-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="3dd42-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3dd42-120">Request headers</span></span>
|<span data-ttu-id="3dd42-121">Header</span><span class="sxs-lookup"><span data-stu-id="3dd42-121">Header</span></span>|<span data-ttu-id="3dd42-122">Wert</span><span class="sxs-lookup"><span data-stu-id="3dd42-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3dd42-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="3dd42-123">Authorization</span></span>|<span data-ttu-id="3dd42-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3dd42-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3dd42-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3dd42-125">Accept</span></span>|<span data-ttu-id="3dd42-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3dd42-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3dd42-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3dd42-127">Request body</span></span>
<span data-ttu-id="3dd42-128">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)-Objekt ein.</span><span class="sxs-lookup"><span data-stu-id="3dd42-128">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="3dd42-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="3dd42-129">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="3dd42-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3dd42-130">Property</span></span>|<span data-ttu-id="3dd42-131">Typ</span><span class="sxs-lookup"><span data-stu-id="3dd42-131">Type</span></span>|<span data-ttu-id="3dd42-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3dd42-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3dd42-133">id</span><span class="sxs-lookup"><span data-stu-id="3dd42-133">id</span></span>|<span data-ttu-id="3dd42-134">String</span><span class="sxs-lookup"><span data-stu-id="3dd42-134">String</span></span>|<span data-ttu-id="3dd42-135">Eindeutiger Bezeichner für die WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="3dd42-135">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="3dd42-136">url</span><span class="sxs-lookup"><span data-stu-id="3dd42-136">url</span></span>|<span data-ttu-id="3dd42-137">String</span><span class="sxs-lookup"><span data-stu-id="3dd42-137">String</span></span>|<span data-ttu-id="3dd42-138">Website-URL</span><span class="sxs-lookup"><span data-stu-id="3dd42-138">Website url</span></span>|
|<span data-ttu-id="3dd42-139">deviceCount</span><span class="sxs-lookup"><span data-stu-id="3dd42-139">deviceCount</span></span>|<span data-ttu-id="3dd42-140">Int32</span><span class="sxs-lookup"><span data-stu-id="3dd42-140">Int32</span></span>|<span data-ttu-id="3dd42-141">Geräteanzahl</span><span class="sxs-lookup"><span data-stu-id="3dd42-141">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="3dd42-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="3dd42-142">Response</span></span>
<span data-ttu-id="3dd42-143">Wenn erfolgreich, gibt diese Methode den `200 OK`-Antwortcode und das aktualisierte [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3dd42-143">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3dd42-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3dd42-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="3dd42-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3dd42-145">Request</span></span>
<span data-ttu-id="3dd42-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3dd42-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
Content-type: application/json
Content-length: 48

{
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="3dd42-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="3dd42-147">Response</span></span>
<span data-ttu-id="3dd42-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3dd42-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





