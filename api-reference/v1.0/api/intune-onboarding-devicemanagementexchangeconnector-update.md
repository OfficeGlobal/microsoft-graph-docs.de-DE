---
title: deviceManagementExchangeConnector aktualisieren
description: Aktualisieren der Eigenschaften eines deviceManagementExchangeConnector-Objekts.
author: tfitzmac
ms.openlocfilehash: 1bbc3f05dd3cee4f2bc92cc279adda705f6a324e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359367"
---
# <a name="update-devicemanagementexchangeconnector"></a><span data-ttu-id="1686f-103">deviceManagementExchangeConnector aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1686f-103">Update deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="1686f-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1686f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1686f-105">Aktualisieren der Eigenschaften eines [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1686f-105">Update the properties of a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1686f-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1686f-106">Prerequisites</span></span>
<span data-ttu-id="1686f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1686f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1686f-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1686f-109">Permission type</span></span>|<span data-ttu-id="1686f-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1686f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1686f-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1686f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1686f-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1686f-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1686f-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1686f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1686f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1686f-114">Not supported.</span></span>|
|<span data-ttu-id="1686f-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1686f-115">Application</span></span>|<span data-ttu-id="1686f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1686f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1686f-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1686f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="1686f-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1686f-118">Request headers</span></span>
|<span data-ttu-id="1686f-119">Header</span><span class="sxs-lookup"><span data-stu-id="1686f-119">Header</span></span>|<span data-ttu-id="1686f-120">Wert</span><span class="sxs-lookup"><span data-stu-id="1686f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1686f-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1686f-121">Authorization</span></span>|<span data-ttu-id="1686f-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1686f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1686f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1686f-123">Accept</span></span>|<span data-ttu-id="1686f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1686f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1686f-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1686f-125">Request body</span></span>
<span data-ttu-id="1686f-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) an.</span><span class="sxs-lookup"><span data-stu-id="1686f-126">In the request body, supply a JSON representation for the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

<span data-ttu-id="1686f-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="1686f-127">The following table shows the properties that are required when you create the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span></span>

|<span data-ttu-id="1686f-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1686f-128">Property</span></span>|<span data-ttu-id="1686f-129">Typ</span><span class="sxs-lookup"><span data-stu-id="1686f-129">Type</span></span>|<span data-ttu-id="1686f-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1686f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1686f-131">id</span><span class="sxs-lookup"><span data-stu-id="1686f-131">id</span></span>|<span data-ttu-id="1686f-132">String</span><span class="sxs-lookup"><span data-stu-id="1686f-132">String</span></span>|<span data-ttu-id="1686f-133">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="1686f-133">Not yet documented</span></span>|
|<span data-ttu-id="1686f-134">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="1686f-134">lastSyncDateTime</span></span>|<span data-ttu-id="1686f-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1686f-135">DateTimeOffset</span></span>|<span data-ttu-id="1686f-136">Zeit der letzten Synchronisierung für Exchange Connector</span><span class="sxs-lookup"><span data-stu-id="1686f-136">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="1686f-137">status</span><span class="sxs-lookup"><span data-stu-id="1686f-137">status</span></span>|[<span data-ttu-id="1686f-138">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="1686f-138">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="1686f-139">Exchange Connectorstatus.</span><span class="sxs-lookup"><span data-stu-id="1686f-139">Exchange Connector Status.</span></span> <span data-ttu-id="1686f-140">Mögliche Werte: sind `none`, `connectionPending`, `connected` und `disconnected`.</span><span class="sxs-lookup"><span data-stu-id="1686f-140">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="1686f-141">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="1686f-141">primarySmtpAddress</span></span>|<span data-ttu-id="1686f-142">String</span><span class="sxs-lookup"><span data-stu-id="1686f-142">String</span></span>|<span data-ttu-id="1686f-143">E-Mail-Adresse, die zum Konfigurieren von Exchange Connector zwischen Diensten verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="1686f-143">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="1686f-144">serverName</span><span class="sxs-lookup"><span data-stu-id="1686f-144">serverName</span></span>|<span data-ttu-id="1686f-145">String</span><span class="sxs-lookup"><span data-stu-id="1686f-145">String</span></span>|<span data-ttu-id="1686f-146">Der Name des Exchange-Servers.</span><span class="sxs-lookup"><span data-stu-id="1686f-146">The name of the Exchange server.</span></span>|
|<span data-ttu-id="1686f-147">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="1686f-147">connectorServerName</span></span>|<span data-ttu-id="1686f-148">String</span><span class="sxs-lookup"><span data-stu-id="1686f-148">String</span></span>|<span data-ttu-id="1686f-149">Der Name des Servers, der Exchange Connector hostet.</span><span class="sxs-lookup"><span data-stu-id="1686f-149">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="1686f-150">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="1686f-150">exchangeConnectorType</span></span>|[<span data-ttu-id="1686f-151">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="1686f-151">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="1686f-152">Der konfigurierte Typ von Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="1686f-152">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="1686f-153">Mögliche Werte: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span><span class="sxs-lookup"><span data-stu-id="1686f-153">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="1686f-154">Version</span><span class="sxs-lookup"><span data-stu-id="1686f-154">version</span></span>|<span data-ttu-id="1686f-155">String</span><span class="sxs-lookup"><span data-stu-id="1686f-155">String</span></span>|<span data-ttu-id="1686f-156">Die Version des ExchangeConnectorAgent</span><span class="sxs-lookup"><span data-stu-id="1686f-156">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="1686f-157">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="1686f-157">exchangeAlias</span></span>|<span data-ttu-id="1686f-158">String</span><span class="sxs-lookup"><span data-stu-id="1686f-158">String</span></span>|<span data-ttu-id="1686f-159">Ein dem Exchange-Server zugewiesener Alias</span><span class="sxs-lookup"><span data-stu-id="1686f-159">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="1686f-160">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="1686f-160">exchangeOrganization</span></span>|<span data-ttu-id="1686f-161">String</span><span class="sxs-lookup"><span data-stu-id="1686f-161">String</span></span>|<span data-ttu-id="1686f-162">Exchange-Organisation für den Exchange-Server</span><span class="sxs-lookup"><span data-stu-id="1686f-162">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="1686f-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="1686f-163">Response</span></span>
<span data-ttu-id="1686f-164">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1686f-164">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1686f-165">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1686f-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="1686f-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1686f-166">Request</span></span>
<span data-ttu-id="1686f-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1686f-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
Content-type: application/json
Content-length: 490

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
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

### <a name="response"></a><span data-ttu-id="1686f-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="1686f-168">Response</span></span>
<span data-ttu-id="1686f-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1686f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



