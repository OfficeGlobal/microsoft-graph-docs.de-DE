---
title: windowsInformationProtectionNetworkLearningSummary erstellen
description: Erstellen eines neuen windowsInformationProtectionNetworkLearningSummary-Objekts.
ms.openlocfilehash: 14802b805a27de32611a32a1c27b7d428629b29e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065666"
---
# <a name="create-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="aef3e-103">windowsInformationProtectionNetworkLearningSummary erstellen</span><span class="sxs-lookup"><span data-stu-id="aef3e-103">Create windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="aef3e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="aef3e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aef3e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="aef3e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aef3e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="aef3e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aef3e-107">Erstellen eines neuen [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="aef3e-107">Create a new [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aef3e-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="aef3e-108">Prerequisites</span></span>
<span data-ttu-id="aef3e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aef3e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aef3e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="aef3e-111">Permission type</span></span>|<span data-ttu-id="aef3e-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="aef3e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aef3e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="aef3e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aef3e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aef3e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="aef3e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="aef3e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aef3e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aef3e-116">Not supported.</span></span>|
|<span data-ttu-id="aef3e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="aef3e-117">Application</span></span>|<span data-ttu-id="aef3e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aef3e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aef3e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aef3e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="aef3e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="aef3e-120">Request headers</span></span>
|<span data-ttu-id="aef3e-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="aef3e-121">Header</span></span>|<span data-ttu-id="aef3e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="aef3e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aef3e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aef3e-123">Authorization</span></span>|<span data-ttu-id="aef3e-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="aef3e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aef3e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aef3e-125">Accept</span></span>|<span data-ttu-id="aef3e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aef3e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aef3e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="aef3e-127">Request body</span></span>
<span data-ttu-id="aef3e-128">Geben Sie im Anforderungstext eine JSON-Darstellung für das windowsInformationProtectionNetworkLearningSummary-Objekt ein.</span><span class="sxs-lookup"><span data-stu-id="aef3e-128">In the request body, supply a JSON representation for the windowsInformationProtectionNetworkLearningSummary object.</span></span>

<span data-ttu-id="aef3e-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsInformationProtectionNetworkLearningSummary erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="aef3e-129">The following table shows the properties that are required when you create the windowsInformationProtectionNetworkLearningSummary.</span></span>

|<span data-ttu-id="aef3e-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="aef3e-130">Property</span></span>|<span data-ttu-id="aef3e-131">Typ</span><span class="sxs-lookup"><span data-stu-id="aef3e-131">Type</span></span>|<span data-ttu-id="aef3e-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aef3e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aef3e-133">id</span><span class="sxs-lookup"><span data-stu-id="aef3e-133">id</span></span>|<span data-ttu-id="aef3e-134">String</span><span class="sxs-lookup"><span data-stu-id="aef3e-134">String</span></span>|<span data-ttu-id="aef3e-135">Eindeutiger Bezeichner für die WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="aef3e-135">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="aef3e-136">url</span><span class="sxs-lookup"><span data-stu-id="aef3e-136">url</span></span>|<span data-ttu-id="aef3e-137">String</span><span class="sxs-lookup"><span data-stu-id="aef3e-137">String</span></span>|<span data-ttu-id="aef3e-138">Website-URL</span><span class="sxs-lookup"><span data-stu-id="aef3e-138">Website url</span></span>|
|<span data-ttu-id="aef3e-139">deviceCount</span><span class="sxs-lookup"><span data-stu-id="aef3e-139">deviceCount</span></span>|<span data-ttu-id="aef3e-140">Int32</span><span class="sxs-lookup"><span data-stu-id="aef3e-140">Int32</span></span>|<span data-ttu-id="aef3e-141">Geräteanzahl</span><span class="sxs-lookup"><span data-stu-id="aef3e-141">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="aef3e-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="aef3e-142">Response</span></span>
<span data-ttu-id="aef3e-143">Wenn erfolgreich, gibt diese Methode den `201 Created`-Antwortcode und das [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="aef3e-143">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aef3e-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="aef3e-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="aef3e-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aef3e-145">Request</span></span>
<span data-ttu-id="aef3e-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="aef3e-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionNetworkLearningSummaries
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="aef3e-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="aef3e-147">Response</span></span>
<span data-ttu-id="aef3e-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aef3e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 186

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "242108f7-08f7-2421-f708-2124f7082124",
  "url": "Url value",
  "deviceCount": 11
}
```





