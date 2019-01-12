---
title: deviceManagementExchangeConnector aktualisieren
description: Aktualisieren der Eigenschaften eines deviceManagementExchangeConnector-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 877493e0ef2234942abf2b1b90d4493b73afb615
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946112"
---
# <a name="update-devicemanagementexchangeconnector"></a><span data-ttu-id="d29bd-103">deviceManagementExchangeConnector aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d29bd-103">Update deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="d29bd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d29bd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d29bd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d29bd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d29bd-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d29bd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d29bd-107">Aktualisieren der Eigenschaften eines [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d29bd-107">Update the properties of a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d29bd-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d29bd-108">Prerequisites</span></span>
<span data-ttu-id="d29bd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d29bd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d29bd-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d29bd-111">Permission type</span></span>|<span data-ttu-id="d29bd-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d29bd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d29bd-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d29bd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d29bd-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d29bd-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d29bd-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d29bd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d29bd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d29bd-116">Not supported.</span></span>|
|<span data-ttu-id="d29bd-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d29bd-117">Application</span></span>|<span data-ttu-id="d29bd-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d29bd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d29bd-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d29bd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="d29bd-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d29bd-120">Request headers</span></span>
|<span data-ttu-id="d29bd-121">Header</span><span class="sxs-lookup"><span data-stu-id="d29bd-121">Header</span></span>|<span data-ttu-id="d29bd-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d29bd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d29bd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d29bd-123">Authorization</span></span>|<span data-ttu-id="d29bd-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d29bd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d29bd-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d29bd-125">Accept</span></span>|<span data-ttu-id="d29bd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d29bd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d29bd-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d29bd-127">Request body</span></span>
<span data-ttu-id="d29bd-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) an.</span><span class="sxs-lookup"><span data-stu-id="d29bd-128">In the request body, supply a JSON representation for the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

<span data-ttu-id="d29bd-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="d29bd-129">The following table shows the properties that are required when you create the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span></span>

|<span data-ttu-id="d29bd-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d29bd-130">Property</span></span>|<span data-ttu-id="d29bd-131">Typ</span><span class="sxs-lookup"><span data-stu-id="d29bd-131">Type</span></span>|<span data-ttu-id="d29bd-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d29bd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d29bd-133">id</span><span class="sxs-lookup"><span data-stu-id="d29bd-133">id</span></span>|<span data-ttu-id="d29bd-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d29bd-134">String</span></span>|<span data-ttu-id="d29bd-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="d29bd-135">Not yet documented</span></span>|
|<span data-ttu-id="d29bd-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d29bd-136">lastSyncDateTime</span></span>|<span data-ttu-id="d29bd-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d29bd-137">DateTimeOffset</span></span>|<span data-ttu-id="d29bd-138">Zeit der letzten Synchronisierung für Exchange Connector</span><span class="sxs-lookup"><span data-stu-id="d29bd-138">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="d29bd-139">status</span><span class="sxs-lookup"><span data-stu-id="d29bd-139">status</span></span>|[<span data-ttu-id="d29bd-140">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="d29bd-140">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="d29bd-141">Exchange Connectorstatus.</span><span class="sxs-lookup"><span data-stu-id="d29bd-141">Exchange Connector Status.</span></span> <span data-ttu-id="d29bd-142">Mögliche Werte: sind `none`, `connectionPending`, `connected` und `disconnected`.</span><span class="sxs-lookup"><span data-stu-id="d29bd-142">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="d29bd-143">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="d29bd-143">primarySmtpAddress</span></span>|<span data-ttu-id="d29bd-144">String</span><span class="sxs-lookup"><span data-stu-id="d29bd-144">String</span></span>|<span data-ttu-id="d29bd-145">E-Mail-Adresse, die zum Konfigurieren von Exchange Connector zwischen Diensten verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="d29bd-145">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="d29bd-146">serverName</span><span class="sxs-lookup"><span data-stu-id="d29bd-146">serverName</span></span>|<span data-ttu-id="d29bd-147">String</span><span class="sxs-lookup"><span data-stu-id="d29bd-147">String</span></span>|<span data-ttu-id="d29bd-148">Der Name des Exchange-Servers.</span><span class="sxs-lookup"><span data-stu-id="d29bd-148">The name of the Exchange server.</span></span>|
|<span data-ttu-id="d29bd-149">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="d29bd-149">connectorServerName</span></span>|<span data-ttu-id="d29bd-150">String</span><span class="sxs-lookup"><span data-stu-id="d29bd-150">String</span></span>|<span data-ttu-id="d29bd-151">Der Name des Servers, der Exchange Connector hostet.</span><span class="sxs-lookup"><span data-stu-id="d29bd-151">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="d29bd-152">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="d29bd-152">exchangeConnectorType</span></span>|[<span data-ttu-id="d29bd-153">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="d29bd-153">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="d29bd-154">Der konfigurierte Typ von Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="d29bd-154">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="d29bd-155">Mögliche Werte: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span><span class="sxs-lookup"><span data-stu-id="d29bd-155">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="d29bd-156">Version</span><span class="sxs-lookup"><span data-stu-id="d29bd-156">version</span></span>|<span data-ttu-id="d29bd-157">String</span><span class="sxs-lookup"><span data-stu-id="d29bd-157">String</span></span>|<span data-ttu-id="d29bd-158">Die Version des ExchangeConnectorAgent</span><span class="sxs-lookup"><span data-stu-id="d29bd-158">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="d29bd-159">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="d29bd-159">exchangeAlias</span></span>|<span data-ttu-id="d29bd-160">String</span><span class="sxs-lookup"><span data-stu-id="d29bd-160">String</span></span>|<span data-ttu-id="d29bd-161">Ein dem Exchange-Server zugewiesener Alias</span><span class="sxs-lookup"><span data-stu-id="d29bd-161">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="d29bd-162">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="d29bd-162">exchangeOrganization</span></span>|<span data-ttu-id="d29bd-163">String</span><span class="sxs-lookup"><span data-stu-id="d29bd-163">String</span></span>|<span data-ttu-id="d29bd-164">Exchange-Organisation für den Exchange-Server</span><span class="sxs-lookup"><span data-stu-id="d29bd-164">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="d29bd-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="d29bd-165">Response</span></span>
<span data-ttu-id="d29bd-166">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d29bd-166">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d29bd-167">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d29bd-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="d29bd-168">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d29bd-168">Request</span></span>
<span data-ttu-id="d29bd-169">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d29bd-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
Content-type: application/json
Content-length: 418

{
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "status": "connectionPending",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "connectorServerName": "Connector Server Name value",
  "exchangeConnectorType": "hosted",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```

### <a name="response"></a><span data-ttu-id="d29bd-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="d29bd-170">Response</span></span>
<span data-ttu-id="d29bd-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d29bd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 539

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "id": "e11c1de8-1de8-e11c-e81d-1ce1e81d1ce1",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "status": "connectionPending",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "connectorServerName": "Connector Server Name value",
  "exchangeConnectorType": "hosted",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```





