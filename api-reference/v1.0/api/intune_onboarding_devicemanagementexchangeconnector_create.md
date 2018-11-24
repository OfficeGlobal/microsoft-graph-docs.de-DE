# <a name="create-devicemanagementexchangeconnector"></a><span data-ttu-id="5d763-101">deviceManagementExchangeConnector erstellen</span><span class="sxs-lookup"><span data-stu-id="5d763-101">Create deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="5d763-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5d763-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5d763-103">Erstellen eines neuen [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="5d763-103">Create a new [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5d763-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5d763-104">Prerequisites</span></span>
<span data-ttu-id="5d763-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5d763-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5d763-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5d763-107">Permission type</span></span>|<span data-ttu-id="5d763-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5d763-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d763-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5d763-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5d763-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d763-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5d763-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5d763-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d763-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5d763-112">Not supported.</span></span>|
|<span data-ttu-id="5d763-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5d763-113">Application</span></span>|<span data-ttu-id="5d763-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5d763-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d763-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d763-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="5d763-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5d763-116">Request headers</span></span>
|<span data-ttu-id="5d763-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5d763-117">Header</span></span>|<span data-ttu-id="5d763-118">Wert</span><span class="sxs-lookup"><span data-stu-id="5d763-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d763-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d763-119">Authorization</span></span>|<span data-ttu-id="5d763-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5d763-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5d763-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5d763-121">Accept</span></span>|<span data-ttu-id="5d763-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5d763-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d763-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5d763-123">Request body</span></span>
<span data-ttu-id="5d763-124">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs deviceManagementExchangeConnector an.</span><span class="sxs-lookup"><span data-stu-id="5d763-124">In the request body, supply a JSON representation for the deviceManagementExchangeConnector object.</span></span>

<span data-ttu-id="5d763-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceManagementExchangeConnector erstellen.</span><span class="sxs-lookup"><span data-stu-id="5d763-125">The following table shows the properties that are required when you create the deviceManagementExchangeConnector.</span></span>

|<span data-ttu-id="5d763-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5d763-126">Property</span></span>|<span data-ttu-id="5d763-127">Typ</span><span class="sxs-lookup"><span data-stu-id="5d763-127">Type</span></span>|<span data-ttu-id="5d763-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5d763-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d763-129">id</span><span class="sxs-lookup"><span data-stu-id="5d763-129">id</span></span>|<span data-ttu-id="5d763-130">String</span><span class="sxs-lookup"><span data-stu-id="5d763-130">String</span></span>|<span data-ttu-id="5d763-131">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="5d763-131">Not yet documented</span></span>|
|<span data-ttu-id="5d763-132">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="5d763-132">lastSyncDateTime</span></span>|<span data-ttu-id="5d763-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d763-133">DateTimeOffset</span></span>|<span data-ttu-id="5d763-134">Zeit der letzten Synchronisierung für Exchange Connector</span><span class="sxs-lookup"><span data-stu-id="5d763-134">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="5d763-135">status</span><span class="sxs-lookup"><span data-stu-id="5d763-135">status</span></span>|[<span data-ttu-id="5d763-136">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="5d763-136">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune_onboarding_devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="5d763-137">Exchange Connectorstatus.</span><span class="sxs-lookup"><span data-stu-id="5d763-137">Exchange Connector Status.</span></span> <span data-ttu-id="5d763-138">Mögliche Werte: sind `none`, `connectionPending`, `connected` und `disconnected`.</span><span class="sxs-lookup"><span data-stu-id="5d763-138">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="5d763-139">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="5d763-139">primarySmtpAddress</span></span>|<span data-ttu-id="5d763-140">String</span><span class="sxs-lookup"><span data-stu-id="5d763-140">String</span></span>|<span data-ttu-id="5d763-141">E-Mail-Adresse, die zum Konfigurieren von Exchange Connector zwischen Diensten verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="5d763-141">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="5d763-142">serverName</span><span class="sxs-lookup"><span data-stu-id="5d763-142">serverName</span></span>|<span data-ttu-id="5d763-143">String</span><span class="sxs-lookup"><span data-stu-id="5d763-143">String</span></span>|<span data-ttu-id="5d763-144">Der Name des Exchange-Servers.</span><span class="sxs-lookup"><span data-stu-id="5d763-144">The name of the Exchange server.</span></span>|
|<span data-ttu-id="5d763-145">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="5d763-145">connectorServerName</span></span>|<span data-ttu-id="5d763-146">String</span><span class="sxs-lookup"><span data-stu-id="5d763-146">String</span></span>|<span data-ttu-id="5d763-147">Der Name des Servers, der Exchange Connector hostet.</span><span class="sxs-lookup"><span data-stu-id="5d763-147">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="5d763-148">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="5d763-148">exchangeConnectorType</span></span>|[<span data-ttu-id="5d763-149">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="5d763-149">deviceManagementExchangeConnectorType</span></span>](../resources/intune_onboarding_devicemanagementexchangeconnectortype.md)|<span data-ttu-id="5d763-150">Der konfigurierte Typ von Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="5d763-150">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="5d763-151">Mögliche Werte: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span><span class="sxs-lookup"><span data-stu-id="5d763-151">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="5d763-152">Version</span><span class="sxs-lookup"><span data-stu-id="5d763-152">version</span></span>|<span data-ttu-id="5d763-153">String</span><span class="sxs-lookup"><span data-stu-id="5d763-153">String</span></span>|<span data-ttu-id="5d763-154">Die Version des ExchangeConnectorAgent</span><span class="sxs-lookup"><span data-stu-id="5d763-154">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="5d763-155">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="5d763-155">exchangeAlias</span></span>|<span data-ttu-id="5d763-156">String</span><span class="sxs-lookup"><span data-stu-id="5d763-156">String</span></span>|<span data-ttu-id="5d763-157">Ein dem Exchange-Server zugewiesener Alias</span><span class="sxs-lookup"><span data-stu-id="5d763-157">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="5d763-158">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="5d763-158">exchangeOrganization</span></span>|<span data-ttu-id="5d763-159">String</span><span class="sxs-lookup"><span data-stu-id="5d763-159">String</span></span>|<span data-ttu-id="5d763-160">Exchange-Organisation für den Exchange-Server</span><span class="sxs-lookup"><span data-stu-id="5d763-160">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="5d763-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d763-161">Response</span></span>
<span data-ttu-id="5d763-162">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5d763-162">If successful, this method returns a `201 Created` response code and a [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d763-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5d763-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="5d763-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d763-164">Request</span></span>
<span data-ttu-id="5d763-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5d763-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5d763-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d763-166">Response</span></span>
<span data-ttu-id="5d763-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5d763-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



