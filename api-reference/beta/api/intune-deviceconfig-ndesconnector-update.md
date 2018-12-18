---
title: NdesConnector aktualisieren
description: Aktualisieren Sie die Eigenschaften eines NdesConnector-Objekts.
author: tfitzmac
ms.openlocfilehash: 80a518a403ce2354ec2f0a633520baf98ae2c7c3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358303"
---
# <a name="update-ndesconnector"></a><span data-ttu-id="65ca0-103">NdesConnector aktualisieren</span><span class="sxs-lookup"><span data-stu-id="65ca0-103">Update ndesConnector</span></span>

> <span data-ttu-id="65ca0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="65ca0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65ca0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="65ca0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="65ca0-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="65ca0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="65ca0-107">Aktualisieren Sie die Eigenschaften eines [NdesConnector](../resources/intune-deviceconfig-ndesconnector.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="65ca0-107">Update the properties of a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="65ca0-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="65ca0-108">Prerequisites</span></span>
<span data-ttu-id="65ca0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65ca0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65ca0-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="65ca0-111">Permission type</span></span>|<span data-ttu-id="65ca0-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="65ca0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65ca0-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="65ca0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="65ca0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65ca0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="65ca0-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="65ca0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65ca0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="65ca0-116">Not supported.</span></span>|
|<span data-ttu-id="65ca0-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="65ca0-117">Application</span></span>|<span data-ttu-id="65ca0-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="65ca0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65ca0-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="65ca0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/ndesConnectors/{ndesConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="65ca0-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="65ca0-120">Request headers</span></span>
|<span data-ttu-id="65ca0-121">Header</span><span class="sxs-lookup"><span data-stu-id="65ca0-121">Header</span></span>|<span data-ttu-id="65ca0-122">Wert</span><span class="sxs-lookup"><span data-stu-id="65ca0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65ca0-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="65ca0-123">Authorization</span></span>|<span data-ttu-id="65ca0-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="65ca0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65ca0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="65ca0-125">Accept</span></span>|<span data-ttu-id="65ca0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="65ca0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65ca0-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="65ca0-127">Request body</span></span>
<span data-ttu-id="65ca0-128">Geben Sie im Textkörper Anforderung für das Objekt [NdesConnector](../resources/intune-deviceconfig-ndesconnector.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="65ca0-128">In the request body, supply a JSON representation for the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

<span data-ttu-id="65ca0-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [NdesConnector](../resources/intune-deviceconfig-ndesconnector.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="65ca0-129">The following table shows the properties that are required when you create the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).</span></span>

|<span data-ttu-id="65ca0-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="65ca0-130">Property</span></span>|<span data-ttu-id="65ca0-131">Typ</span><span class="sxs-lookup"><span data-stu-id="65ca0-131">Type</span></span>|<span data-ttu-id="65ca0-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="65ca0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65ca0-133">id</span><span class="sxs-lookup"><span data-stu-id="65ca0-133">id</span></span>|<span data-ttu-id="65ca0-134">String</span><span class="sxs-lookup"><span data-stu-id="65ca0-134">String</span></span>|<span data-ttu-id="65ca0-135">Der Schlüssel des NDES Connectors.</span><span class="sxs-lookup"><span data-stu-id="65ca0-135">The key of the NDES Connector.</span></span>|
|<span data-ttu-id="65ca0-136">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="65ca0-136">lastConnectionDateTime</span></span>|<span data-ttu-id="65ca0-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65ca0-137">DateTimeOffset</span></span>|<span data-ttu-id="65ca0-138">Letzte Verbindungszeit für den Ndes Connector</span><span class="sxs-lookup"><span data-stu-id="65ca0-138">Last connection time for the Ndes Connector</span></span>|
|<span data-ttu-id="65ca0-139">state</span><span class="sxs-lookup"><span data-stu-id="65ca0-139">state</span></span>|[<span data-ttu-id="65ca0-140">ndesConnectorState</span><span class="sxs-lookup"><span data-stu-id="65ca0-140">ndesConnectorState</span></span>](../resources/intune-deviceconfig-ndesconnectorstate.md)|<span data-ttu-id="65ca0-141">NDES Connector Status.</span><span class="sxs-lookup"><span data-stu-id="65ca0-141">Ndes Connector Status.</span></span> <span data-ttu-id="65ca0-142">Mögliche Werte sind: `none`, `active` und `inactive`.</span><span class="sxs-lookup"><span data-stu-id="65ca0-142">Possible values are: `none`, `active`, `inactive`.</span></span>|
|<span data-ttu-id="65ca0-143">displayName</span><span class="sxs-lookup"><span data-stu-id="65ca0-143">displayName</span></span>|<span data-ttu-id="65ca0-144">String</span><span class="sxs-lookup"><span data-stu-id="65ca0-144">String</span></span>|<span data-ttu-id="65ca0-145">Der Anzeigename der Verbindung Ndes.</span><span class="sxs-lookup"><span data-stu-id="65ca0-145">The friendly name of the Ndes Connector.</span></span>|



## <a name="response"></a><span data-ttu-id="65ca0-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="65ca0-146">Response</span></span>
<span data-ttu-id="65ca0-147">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [NdesConnector](../resources/intune-deviceconfig-ndesconnector.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="65ca0-147">If successful, this method returns a `200 OK` response code and an updated [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65ca0-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="65ca0-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="65ca0-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="65ca0-149">Request</span></span>
<span data-ttu-id="65ca0-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="65ca0-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/ndesConnectors/{ndesConnectorId}
Content-type: application/json
Content-length: 131

{
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "active",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="65ca0-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="65ca0-151">Response</span></span>
<span data-ttu-id="65ca0-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="65ca0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





