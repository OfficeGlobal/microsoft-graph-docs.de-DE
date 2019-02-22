---
title: NdesConnector aktualisieren
description: Aktualisieren der Eigenschaften eines ndesConnector-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a4d51f22c71ef43784ec45e521f0e1900abdb9c0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140278"
---
# <a name="update-ndesconnector"></a><span data-ttu-id="c918d-103">NdesConnector aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c918d-103">Update ndesConnector</span></span>

> <span data-ttu-id="c918d-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c918d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c918d-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c918d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c918d-106">Aktualisieren der Eigenschaften eines [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c918d-106">Update the properties of a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c918d-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c918d-107">Prerequisites</span></span>
<span data-ttu-id="c918d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c918d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c918d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c918d-110">Permission type</span></span>|<span data-ttu-id="c918d-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c918d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c918d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c918d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c918d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c918d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c918d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c918d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c918d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c918d-115">Not supported.</span></span>|
|<span data-ttu-id="c918d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c918d-116">Application</span></span>|<span data-ttu-id="c918d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c918d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c918d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c918d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/ndesConnectors/{ndesConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="c918d-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c918d-119">Request headers</span></span>
|<span data-ttu-id="c918d-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c918d-120">Header</span></span>|<span data-ttu-id="c918d-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c918d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c918d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c918d-122">Authorization</span></span>|<span data-ttu-id="c918d-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c918d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c918d-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c918d-124">Accept</span></span>|<span data-ttu-id="c918d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c918d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c918d-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c918d-126">Request body</span></span>
<span data-ttu-id="c918d-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="c918d-127">In the request body, supply a JSON representation for the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

<span data-ttu-id="c918d-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c918d-128">The following table shows the properties that are required when you create the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).</span></span>

|<span data-ttu-id="c918d-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c918d-129">Property</span></span>|<span data-ttu-id="c918d-130">Typ</span><span class="sxs-lookup"><span data-stu-id="c918d-130">Type</span></span>|<span data-ttu-id="c918d-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c918d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c918d-132">id</span><span class="sxs-lookup"><span data-stu-id="c918d-132">id</span></span>|<span data-ttu-id="c918d-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c918d-133">String</span></span>|<span data-ttu-id="c918d-134">Der Schlüssel des NDES-Konnektors.</span><span class="sxs-lookup"><span data-stu-id="c918d-134">The key of the NDES Connector.</span></span>|
|<span data-ttu-id="c918d-135">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="c918d-135">lastConnectionDateTime</span></span>|<span data-ttu-id="c918d-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c918d-136">DateTimeOffset</span></span>|<span data-ttu-id="c918d-137">Letzter Verbindungszeitpunkt für den NDES-Connector</span><span class="sxs-lookup"><span data-stu-id="c918d-137">Last connection time for the Ndes Connector</span></span>|
|<span data-ttu-id="c918d-138">state</span><span class="sxs-lookup"><span data-stu-id="c918d-138">state</span></span>|[<span data-ttu-id="c918d-139">ndesConnectorState</span><span class="sxs-lookup"><span data-stu-id="c918d-139">ndesConnectorState</span></span>](../resources/intune-deviceconfig-ndesconnectorstate.md)|<span data-ttu-id="c918d-140">NDES-Connectorstatus.</span><span class="sxs-lookup"><span data-stu-id="c918d-140">Ndes Connector Status.</span></span> <span data-ttu-id="c918d-141">Mögliche Werte sind: `none`, `active` und `inactive`.</span><span class="sxs-lookup"><span data-stu-id="c918d-141">Possible values are: `none`, `active`, `inactive`.</span></span>|
|<span data-ttu-id="c918d-142">displayName</span><span class="sxs-lookup"><span data-stu-id="c918d-142">displayName</span></span>|<span data-ttu-id="c918d-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c918d-143">String</span></span>|<span data-ttu-id="c918d-144">Der Anzeigename des NDES-Konnektors.</span><span class="sxs-lookup"><span data-stu-id="c918d-144">The friendly name of the Ndes Connector.</span></span>|



## <a name="response"></a><span data-ttu-id="c918d-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="c918d-145">Response</span></span>
<span data-ttu-id="c918d-146">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c918d-146">If successful, this method returns a `200 OK` response code and an updated [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c918d-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c918d-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="c918d-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c918d-148">Request</span></span>
<span data-ttu-id="c918d-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c918d-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/ndesConnectors/{ndesConnectorId}
Content-type: application/json
Content-length: 183

{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "active",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="c918d-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="c918d-150">Response</span></span>
<span data-ttu-id="c918d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c918d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 232

{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "id": "e71fa706-a706-e71f-06a7-1fe706a71fe7",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "active",
  "displayName": "Display Name value"
}
```




