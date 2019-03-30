---
title: NdesConnector erstellen
description: Erstellen eines neuen ndesConnector-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 33d3d832df9e14692316b9b12132c531a2b610d3
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986180"
---
# <a name="create-ndesconnector"></a><span data-ttu-id="acec2-103">NdesConnector erstellen</span><span class="sxs-lookup"><span data-stu-id="acec2-103">Create ndesConnector</span></span>

> <span data-ttu-id="acec2-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="acec2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="acec2-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="acec2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="acec2-106">Erstellen eines neuen [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="acec2-106">Create a new [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="acec2-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="acec2-107">Prerequisites</span></span>
<span data-ttu-id="acec2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="acec2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acec2-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="acec2-110">Permission type</span></span>|<span data-ttu-id="acec2-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="acec2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="acec2-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="acec2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="acec2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acec2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="acec2-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="acec2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="acec2-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="acec2-115">Not supported.</span></span>|
|<span data-ttu-id="acec2-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="acec2-116">Application</span></span>|<span data-ttu-id="acec2-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="acec2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="acec2-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="acec2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/ndesConnectors
```

## <a name="request-headers"></a><span data-ttu-id="acec2-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="acec2-119">Request headers</span></span>
|<span data-ttu-id="acec2-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="acec2-120">Header</span></span>|<span data-ttu-id="acec2-121">Wert</span><span class="sxs-lookup"><span data-stu-id="acec2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="acec2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="acec2-122">Authorization</span></span>|<span data-ttu-id="acec2-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="acec2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="acec2-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="acec2-124">Accept</span></span>|<span data-ttu-id="acec2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="acec2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="acec2-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="acec2-126">Request body</span></span>
<span data-ttu-id="acec2-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das ndesConnector-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="acec2-127">In the request body, supply a JSON representation for the ndesConnector object.</span></span>

<span data-ttu-id="acec2-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der ndesConnector erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="acec2-128">The following table shows the properties that are required when you create the ndesConnector.</span></span>

|<span data-ttu-id="acec2-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="acec2-129">Property</span></span>|<span data-ttu-id="acec2-130">Typ</span><span class="sxs-lookup"><span data-stu-id="acec2-130">Type</span></span>|<span data-ttu-id="acec2-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="acec2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="acec2-132">id</span><span class="sxs-lookup"><span data-stu-id="acec2-132">id</span></span>|<span data-ttu-id="acec2-133">String</span><span class="sxs-lookup"><span data-stu-id="acec2-133">String</span></span>|<span data-ttu-id="acec2-134">Der Schlüssel des NDES-Konnektors.</span><span class="sxs-lookup"><span data-stu-id="acec2-134">The key of the NDES Connector.</span></span>|
|<span data-ttu-id="acec2-135">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="acec2-135">lastConnectionDateTime</span></span>|<span data-ttu-id="acec2-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="acec2-136">DateTimeOffset</span></span>|<span data-ttu-id="acec2-137">Letzter Verbindungszeitpunkt für den NDES-Connector</span><span class="sxs-lookup"><span data-stu-id="acec2-137">Last connection time for the Ndes Connector</span></span>|
|<span data-ttu-id="acec2-138">state</span><span class="sxs-lookup"><span data-stu-id="acec2-138">state</span></span>|[<span data-ttu-id="acec2-139">ndesConnectorState</span><span class="sxs-lookup"><span data-stu-id="acec2-139">ndesConnectorState</span></span>](../resources/intune-deviceconfig-ndesconnectorstate.md)|<span data-ttu-id="acec2-140">NDES-Connectorstatus.</span><span class="sxs-lookup"><span data-stu-id="acec2-140">Ndes Connector Status.</span></span> <span data-ttu-id="acec2-141">Mögliche Werte sind: `none`, `active` und `inactive`.</span><span class="sxs-lookup"><span data-stu-id="acec2-141">Possible values are: `none`, `active`, `inactive`.</span></span>|
|<span data-ttu-id="acec2-142">displayName</span><span class="sxs-lookup"><span data-stu-id="acec2-142">displayName</span></span>|<span data-ttu-id="acec2-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="acec2-143">String</span></span>|<span data-ttu-id="acec2-144">Der Anzeigename des NDES-Konnektors.</span><span class="sxs-lookup"><span data-stu-id="acec2-144">The friendly name of the Ndes Connector.</span></span>|



## <a name="response"></a><span data-ttu-id="acec2-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="acec2-145">Response</span></span>
<span data-ttu-id="acec2-146">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="acec2-146">If successful, this method returns a `201 Created` response code and a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="acec2-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="acec2-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="acec2-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="acec2-148">Request</span></span>
<span data-ttu-id="acec2-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="acec2-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/ndesConnectors
Content-type: application/json
Content-length: 183

{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "active",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="acec2-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="acec2-150">Response</span></span>
<span data-ttu-id="acec2-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="acec2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




