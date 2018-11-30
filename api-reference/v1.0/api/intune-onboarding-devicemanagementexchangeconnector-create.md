---
title: deviceManagementExchangeConnector erstellen
description: Erstellen eines neuen deviceManagementExchangeConnector-Objekts.
ms.openlocfilehash: 710f2a1d43f95a8a3ca6f6f154a667b78e8c0795
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016606"
---
# <a name="create-devicemanagementexchangeconnector"></a><span data-ttu-id="9e6a2-103">deviceManagementExchangeConnector erstellen</span><span class="sxs-lookup"><span data-stu-id="9e6a2-103">Create deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="9e6a2-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9e6a2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9e6a2-105">Erstellen eines neuen [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9e6a2-105">Create a new [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9e6a2-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9e6a2-106">Prerequisites</span></span>
<span data-ttu-id="9e6a2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e6a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e6a2-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9e6a2-109">Permission type</span></span>|<span data-ttu-id="9e6a2-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9e6a2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e6a2-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9e6a2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9e6a2-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e6a2-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9e6a2-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9e6a2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e6a2-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9e6a2-114">Not supported.</span></span>|
|<span data-ttu-id="9e6a2-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9e6a2-115">Application</span></span>|<span data-ttu-id="9e6a2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9e6a2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e6a2-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9e6a2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="9e6a2-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9e6a2-118">Request headers</span></span>
|<span data-ttu-id="9e6a2-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9e6a2-119">Header</span></span>|<span data-ttu-id="9e6a2-120">Wert</span><span class="sxs-lookup"><span data-stu-id="9e6a2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e6a2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e6a2-121">Authorization</span></span>|<span data-ttu-id="9e6a2-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9e6a2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e6a2-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9e6a2-123">Accept</span></span>|<span data-ttu-id="9e6a2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9e6a2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e6a2-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9e6a2-125">Request body</span></span>
<span data-ttu-id="9e6a2-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs deviceManagementExchangeConnector an.</span><span class="sxs-lookup"><span data-stu-id="9e6a2-126">In the request body, supply a JSON representation for the deviceManagementExchangeConnector object.</span></span>

<span data-ttu-id="9e6a2-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceManagementExchangeConnector erstellen.</span><span class="sxs-lookup"><span data-stu-id="9e6a2-127">The following table shows the properties that are required when you create the deviceManagementExchangeConnector.</span></span>

|<span data-ttu-id="9e6a2-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9e6a2-128">Property</span></span>|<span data-ttu-id="9e6a2-129">Typ</span><span class="sxs-lookup"><span data-stu-id="9e6a2-129">Type</span></span>|<span data-ttu-id="9e6a2-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9e6a2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e6a2-131">id</span><span class="sxs-lookup"><span data-stu-id="9e6a2-131">id</span></span>|<span data-ttu-id="9e6a2-132">String</span><span class="sxs-lookup"><span data-stu-id="9e6a2-132">String</span></span>|<span data-ttu-id="9e6a2-133">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="9e6a2-133">Not yet documented</span></span>|
|<span data-ttu-id="9e6a2-134">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="9e6a2-134">lastSyncDateTime</span></span>|<span data-ttu-id="9e6a2-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e6a2-135">DateTimeOffset</span></span>|<span data-ttu-id="9e6a2-136">Zeit der letzten Synchronisierung für Exchange Connector</span><span class="sxs-lookup"><span data-stu-id="9e6a2-136">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="9e6a2-137">status</span><span class="sxs-lookup"><span data-stu-id="9e6a2-137">status</span></span>|[<span data-ttu-id="9e6a2-138">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="9e6a2-138">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="9e6a2-139">Exchange Connectorstatus.</span><span class="sxs-lookup"><span data-stu-id="9e6a2-139">Exchange Connector Status.</span></span> <span data-ttu-id="9e6a2-140">Mögliche Werte: sind `none`, `connectionPending`, `connected` und `disconnected`.</span><span class="sxs-lookup"><span data-stu-id="9e6a2-140">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="9e6a2-141">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="9e6a2-141">primarySmtpAddress</span></span>|<span data-ttu-id="9e6a2-142">String</span><span class="sxs-lookup"><span data-stu-id="9e6a2-142">String</span></span>|<span data-ttu-id="9e6a2-143">E-Mail-Adresse, die zum Konfigurieren von Exchange Connector zwischen Diensten verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="9e6a2-143">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="9e6a2-144">serverName</span><span class="sxs-lookup"><span data-stu-id="9e6a2-144">serverName</span></span>|<span data-ttu-id="9e6a2-145">String</span><span class="sxs-lookup"><span data-stu-id="9e6a2-145">String</span></span>|<span data-ttu-id="9e6a2-146">Der Name des Exchange-Servers.</span><span class="sxs-lookup"><span data-stu-id="9e6a2-146">The name of the Exchange server.</span></span>|
|<span data-ttu-id="9e6a2-147">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="9e6a2-147">connectorServerName</span></span>|<span data-ttu-id="9e6a2-148">String</span><span class="sxs-lookup"><span data-stu-id="9e6a2-148">String</span></span>|<span data-ttu-id="9e6a2-149">Der Name des Servers, der Exchange Connector hostet.</span><span class="sxs-lookup"><span data-stu-id="9e6a2-149">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="9e6a2-150">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="9e6a2-150">exchangeConnectorType</span></span>|[<span data-ttu-id="9e6a2-151">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="9e6a2-151">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="9e6a2-152">Der konfigurierte Typ von Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="9e6a2-152">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="9e6a2-153">Mögliche Werte: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span><span class="sxs-lookup"><span data-stu-id="9e6a2-153">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="9e6a2-154">Version</span><span class="sxs-lookup"><span data-stu-id="9e6a2-154">version</span></span>|<span data-ttu-id="9e6a2-155">String</span><span class="sxs-lookup"><span data-stu-id="9e6a2-155">String</span></span>|<span data-ttu-id="9e6a2-156">Die Version des ExchangeConnectorAgent</span><span class="sxs-lookup"><span data-stu-id="9e6a2-156">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="9e6a2-157">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="9e6a2-157">exchangeAlias</span></span>|<span data-ttu-id="9e6a2-158">String</span><span class="sxs-lookup"><span data-stu-id="9e6a2-158">String</span></span>|<span data-ttu-id="9e6a2-159">Ein dem Exchange-Server zugewiesener Alias</span><span class="sxs-lookup"><span data-stu-id="9e6a2-159">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="9e6a2-160">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="9e6a2-160">exchangeOrganization</span></span>|<span data-ttu-id="9e6a2-161">String</span><span class="sxs-lookup"><span data-stu-id="9e6a2-161">String</span></span>|<span data-ttu-id="9e6a2-162">Exchange-Organisation für den Exchange-Server</span><span class="sxs-lookup"><span data-stu-id="9e6a2-162">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="9e6a2-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="9e6a2-163">Response</span></span>
<span data-ttu-id="9e6a2-164">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9e6a2-164">If successful, this method returns a `201 Created` response code and a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e6a2-165">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9e6a2-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="9e6a2-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9e6a2-166">Request</span></span>
<span data-ttu-id="9e6a2-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9e6a2-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors
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

### <a name="response"></a><span data-ttu-id="9e6a2-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="9e6a2-168">Response</span></span>
<span data-ttu-id="9e6a2-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9e6a2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



