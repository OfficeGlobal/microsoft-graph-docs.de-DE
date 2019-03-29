---
title: NetworkIPv4ConfigurationManagementCondition erstellen
description: Erstellen eines neuen networkIPv4ConfigurationManagementCondition-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e045c50df3e2ce74ed3bc4d4420c506ef5e7a651
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30966173"
---
# <a name="create-networkipv4configurationmanagementcondition"></a><span data-ttu-id="75b89-103">NetworkIPv4ConfigurationManagementCondition erstellen</span><span class="sxs-lookup"><span data-stu-id="75b89-103">Create networkIPv4ConfigurationManagementCondition</span></span>

> <span data-ttu-id="75b89-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="75b89-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75b89-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="75b89-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75b89-106">Erstellen eines neuen [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="75b89-106">Create a new [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75b89-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="75b89-107">Prerequisites</span></span>
<span data-ttu-id="75b89-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75b89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75b89-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="75b89-110">Permission type</span></span>|<span data-ttu-id="75b89-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="75b89-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75b89-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="75b89-112">Delegated (work or school account)</span></span>|<span data-ttu-id="75b89-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75b89-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="75b89-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="75b89-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75b89-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="75b89-115">Not supported.</span></span>|
|<span data-ttu-id="75b89-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="75b89-116">Application</span></span>|<span data-ttu-id="75b89-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="75b89-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="75b89-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="75b89-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="75b89-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="75b89-119">Request headers</span></span>
|<span data-ttu-id="75b89-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="75b89-120">Header</span></span>|<span data-ttu-id="75b89-121">Wert</span><span class="sxs-lookup"><span data-stu-id="75b89-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75b89-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="75b89-122">Authorization</span></span>|<span data-ttu-id="75b89-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="75b89-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75b89-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="75b89-124">Accept</span></span>|<span data-ttu-id="75b89-125">application/json</span><span class="sxs-lookup"><span data-stu-id="75b89-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75b89-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="75b89-126">Request body</span></span>
<span data-ttu-id="75b89-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das networkIPv4ConfigurationManagementCondition-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="75b89-127">In the request body, supply a JSON representation for the networkIPv4ConfigurationManagementCondition object.</span></span>

<span data-ttu-id="75b89-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der networkIPv4ConfigurationManagementCondition erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="75b89-128">The following table shows the properties that are required when you create the networkIPv4ConfigurationManagementCondition.</span></span>

|<span data-ttu-id="75b89-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="75b89-129">Property</span></span>|<span data-ttu-id="75b89-130">Typ</span><span class="sxs-lookup"><span data-stu-id="75b89-130">Type</span></span>|<span data-ttu-id="75b89-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="75b89-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75b89-132">id</span><span class="sxs-lookup"><span data-stu-id="75b89-132">id</span></span>|<span data-ttu-id="75b89-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="75b89-133">String</span></span>|<span data-ttu-id="75b89-134">Eindeutiger Bezeichner für die Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="75b89-134">Unique identifier for the management condition.</span></span> <span data-ttu-id="75b89-135">Vom System generierter Wert, der bei der Erstellung zugewiesen wird.</span><span class="sxs-lookup"><span data-stu-id="75b89-135">System generated value assigned when created.</span></span> <span data-ttu-id="75b89-136">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="75b89-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="75b89-137">uniqueName</span><span class="sxs-lookup"><span data-stu-id="75b89-137">uniqueName</span></span>|<span data-ttu-id="75b89-138">String</span><span class="sxs-lookup"><span data-stu-id="75b89-138">String</span></span>|<span data-ttu-id="75b89-139">Eindeutiger Name für die Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="75b89-139">Unique name for the management condition.</span></span> <span data-ttu-id="75b89-140">Wird in Verwaltungs Bedingungsausdrücken verwendet.</span><span class="sxs-lookup"><span data-stu-id="75b89-140">Used in management condition expressions.</span></span> <span data-ttu-id="75b89-141">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="75b89-141">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="75b89-142">displayName</span><span class="sxs-lookup"><span data-stu-id="75b89-142">displayName</span></span>|<span data-ttu-id="75b89-143">String</span><span class="sxs-lookup"><span data-stu-id="75b89-143">String</span></span>|<span data-ttu-id="75b89-144">Der Administrator definierte Name der Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="75b89-144">The admin defined name of the management condition.</span></span> <span data-ttu-id="75b89-145">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="75b89-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="75b89-146">description</span><span class="sxs-lookup"><span data-stu-id="75b89-146">description</span></span>|<span data-ttu-id="75b89-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="75b89-147">String</span></span>|<span data-ttu-id="75b89-148">Die vom Administrator definierte Beschreibung der Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="75b89-148">The admin defined description of the management condition.</span></span> <span data-ttu-id="75b89-149">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="75b89-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="75b89-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="75b89-150">createdDateTime</span></span>|<span data-ttu-id="75b89-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75b89-151">DateTimeOffset</span></span>|<span data-ttu-id="75b89-152">Der Zeitpunkt, zu dem die Verwaltungsbedingung erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="75b89-152">The time the management condition was created.</span></span> <span data-ttu-id="75b89-153">Generierte Dienstseite.</span><span class="sxs-lookup"><span data-stu-id="75b89-153">Generated service side.</span></span> <span data-ttu-id="75b89-154">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="75b89-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="75b89-155">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="75b89-155">modifiedDateTime</span></span>|<span data-ttu-id="75b89-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75b89-156">DateTimeOffset</span></span>|<span data-ttu-id="75b89-157">Der Zeitpunkt, zu dem die Verwaltungsbedingung zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="75b89-157">The time the management condition was last modified.</span></span> <span data-ttu-id="75b89-158">Aktualisierte Dienstseite.</span><span class="sxs-lookup"><span data-stu-id="75b89-158">Updated service side.</span></span> <span data-ttu-id="75b89-159">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="75b89-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="75b89-160">eTag</span><span class="sxs-lookup"><span data-stu-id="75b89-160">eTag</span></span>|<span data-ttu-id="75b89-161">String</span><span class="sxs-lookup"><span data-stu-id="75b89-161">String</span></span>|<span data-ttu-id="75b89-162">ETag der Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="75b89-162">ETag of the management condition.</span></span> <span data-ttu-id="75b89-163">Aktualisierte Dienstseite.</span><span class="sxs-lookup"><span data-stu-id="75b89-163">Updated service side.</span></span> <span data-ttu-id="75b89-164">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="75b89-164">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="75b89-165">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="75b89-165">applicablePlatforms</span></span>|<span data-ttu-id="75b89-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="75b89-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="75b89-167">Die entsprechenden Plattformen für diese Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="75b89-167">The applicable platforms for this management condition.</span></span> <span data-ttu-id="75b89-168">Von [ManagementCondition](../resources/intune-fencing-managementcondition.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="75b89-168">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="75b89-169">Mögliche Werte: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="75b89-169">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="75b89-170">ipV4Prefix</span><span class="sxs-lookup"><span data-stu-id="75b89-170">ipV4Prefix</span></span>|<span data-ttu-id="75b89-171">String</span><span class="sxs-lookup"><span data-stu-id="75b89-171">String</span></span>|<span data-ttu-id="75b89-172">Das IPv4-Subnetz, mit dem eine Verbindung hergestellt werden soll.</span><span class="sxs-lookup"><span data-stu-id="75b89-172">The IPv4 subnet to be connected to.</span></span> <span data-ttu-id="75b89-173">z.b. 10.0.0.0/8</span><span class="sxs-lookup"><span data-stu-id="75b89-173">e.g. 10.0.0.0/8</span></span>|
|<span data-ttu-id="75b89-174">ipV4Gateway</span><span class="sxs-lookup"><span data-stu-id="75b89-174">ipV4Gateway</span></span>|<span data-ttu-id="75b89-175">String</span><span class="sxs-lookup"><span data-stu-id="75b89-175">String</span></span>|<span data-ttu-id="75b89-176">Die Adresse des IPv4-Gateways.</span><span class="sxs-lookup"><span data-stu-id="75b89-176">The IPv4 gateway address.</span></span> <span data-ttu-id="75b89-177">beispielsweise 10.0.0.0</span><span class="sxs-lookup"><span data-stu-id="75b89-177">e.g. 10.0.0.0</span></span>|
|<span data-ttu-id="75b89-178">ipV4DHCPServer</span><span class="sxs-lookup"><span data-stu-id="75b89-178">ipV4DHCPServer</span></span>|<span data-ttu-id="75b89-179">String</span><span class="sxs-lookup"><span data-stu-id="75b89-179">String</span></span>|<span data-ttu-id="75b89-180">Die IPv4-Adresse des DHCP-Servers für den Adapter.</span><span class="sxs-lookup"><span data-stu-id="75b89-180">The IPv4 address of the DHCP server for the adapter.</span></span>|
|<span data-ttu-id="75b89-181">ipV4DNSServerList</span><span class="sxs-lookup"><span data-stu-id="75b89-181">ipV4DNSServerList</span></span>|<span data-ttu-id="75b89-182">String collection</span><span class="sxs-lookup"><span data-stu-id="75b89-182">String collection</span></span>|<span data-ttu-id="75b89-183">Die für den Adapter konfigurierten IPv4-DNS-Server.</span><span class="sxs-lookup"><span data-stu-id="75b89-183">The IPv4 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="75b89-184">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="75b89-184">dnsSuffixList</span></span>|<span data-ttu-id="75b89-185">String collection</span><span class="sxs-lookup"><span data-stu-id="75b89-185">String collection</span></span>|<span data-ttu-id="75b89-186">Gültige DNS-Suffixe für das aktuelle Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="75b89-186">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="75b89-187">beispielsweise Seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="75b89-187">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="75b89-188">Antwort</span><span class="sxs-lookup"><span data-stu-id="75b89-188">Response</span></span>
<span data-ttu-id="75b89-189">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="75b89-189">If successful, this method returns a `201 Created` response code and a [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75b89-190">Beispiel</span><span class="sxs-lookup"><span data-stu-id="75b89-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="75b89-191">Anforderung</span><span class="sxs-lookup"><span data-stu-id="75b89-191">Request</span></span>
<span data-ttu-id="75b89-192">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="75b89-192">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditions
Content-type: application/json
Content-length: 529

{
  "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV4Prefix": "Ip V4Prefix value",
  "ipV4Gateway": "Ip V4Gateway value",
  "ipV4DHCPServer": "Ip V4DHCPServer value",
  "ipV4DNSServerList": [
    "Ip V4DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="75b89-193">Antwort</span><span class="sxs-lookup"><span data-stu-id="75b89-193">Response</span></span>
<span data-ttu-id="75b89-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="75b89-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 697

{
  "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
  "id": "5e4a8284-8284-5e4a-8482-4a5e84824a5e",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV4Prefix": "Ip V4Prefix value",
  "ipV4Gateway": "Ip V4Gateway value",
  "ipV4DHCPServer": "Ip V4DHCPServer value",
  "ipV4DNSServerList": [
    "Ip V4DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```




