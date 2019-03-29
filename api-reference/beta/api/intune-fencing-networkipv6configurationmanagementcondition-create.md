---
title: NetworkIPv6ConfigurationManagementCondition erstellen
description: Erstellen eines neuen networkIPv6ConfigurationManagementCondition-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5dee9ff40118cb52d51c53204332b859e0bb0bba
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30966145"
---
# <a name="create-networkipv6configurationmanagementcondition"></a><span data-ttu-id="664c8-103">NetworkIPv6ConfigurationManagementCondition erstellen</span><span class="sxs-lookup"><span data-stu-id="664c8-103">Create networkIPv6ConfigurationManagementCondition</span></span>

> <span data-ttu-id="664c8-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="664c8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="664c8-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="664c8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="664c8-106">Erstellen eines neuen [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="664c8-106">Create a new [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="664c8-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="664c8-107">Prerequisites</span></span>
<span data-ttu-id="664c8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="664c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="664c8-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="664c8-110">Permission type</span></span>|<span data-ttu-id="664c8-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="664c8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="664c8-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="664c8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="664c8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="664c8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="664c8-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="664c8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="664c8-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="664c8-115">Not supported.</span></span>|
|<span data-ttu-id="664c8-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="664c8-116">Application</span></span>|<span data-ttu-id="664c8-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="664c8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="664c8-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="664c8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="664c8-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="664c8-119">Request headers</span></span>
|<span data-ttu-id="664c8-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="664c8-120">Header</span></span>|<span data-ttu-id="664c8-121">Wert</span><span class="sxs-lookup"><span data-stu-id="664c8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="664c8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="664c8-122">Authorization</span></span>|<span data-ttu-id="664c8-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="664c8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="664c8-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="664c8-124">Accept</span></span>|<span data-ttu-id="664c8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="664c8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="664c8-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="664c8-126">Request body</span></span>
<span data-ttu-id="664c8-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das networkIPv6ConfigurationManagementCondition-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="664c8-127">In the request body, supply a JSON representation for the networkIPv6ConfigurationManagementCondition object.</span></span>

<span data-ttu-id="664c8-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der networkIPv6ConfigurationManagementCondition erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="664c8-128">The following table shows the properties that are required when you create the networkIPv6ConfigurationManagementCondition.</span></span>

|<span data-ttu-id="664c8-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="664c8-129">Property</span></span>|<span data-ttu-id="664c8-130">Typ</span><span class="sxs-lookup"><span data-stu-id="664c8-130">Type</span></span>|<span data-ttu-id="664c8-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="664c8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="664c8-132">id</span><span class="sxs-lookup"><span data-stu-id="664c8-132">id</span></span>|<span data-ttu-id="664c8-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="664c8-133">String</span></span>|<span data-ttu-id="664c8-134">Eindeutiger Bezeichner für die Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="664c8-134">Unique identifier for the management condition.</span></span> <span data-ttu-id="664c8-135">Vom System generierter Wert, der bei der Erstellung zugewiesen wird.</span><span class="sxs-lookup"><span data-stu-id="664c8-135">System generated value assigned when created.</span></span> <span data-ttu-id="664c8-136">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="664c8-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="664c8-137">uniqueName</span><span class="sxs-lookup"><span data-stu-id="664c8-137">uniqueName</span></span>|<span data-ttu-id="664c8-138">String</span><span class="sxs-lookup"><span data-stu-id="664c8-138">String</span></span>|<span data-ttu-id="664c8-139">Eindeutiger Name für die Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="664c8-139">Unique name for the management condition.</span></span> <span data-ttu-id="664c8-140">Wird in Verwaltungs Bedingungsausdrücken verwendet.</span><span class="sxs-lookup"><span data-stu-id="664c8-140">Used in management condition expressions.</span></span> <span data-ttu-id="664c8-141">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="664c8-141">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="664c8-142">displayName</span><span class="sxs-lookup"><span data-stu-id="664c8-142">displayName</span></span>|<span data-ttu-id="664c8-143">String</span><span class="sxs-lookup"><span data-stu-id="664c8-143">String</span></span>|<span data-ttu-id="664c8-144">Der Administrator definierte Name der Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="664c8-144">The admin defined name of the management condition.</span></span> <span data-ttu-id="664c8-145">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="664c8-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="664c8-146">description</span><span class="sxs-lookup"><span data-stu-id="664c8-146">description</span></span>|<span data-ttu-id="664c8-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="664c8-147">String</span></span>|<span data-ttu-id="664c8-148">Die vom Administrator definierte Beschreibung der Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="664c8-148">The admin defined description of the management condition.</span></span> <span data-ttu-id="664c8-149">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="664c8-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="664c8-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="664c8-150">createdDateTime</span></span>|<span data-ttu-id="664c8-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="664c8-151">DateTimeOffset</span></span>|<span data-ttu-id="664c8-152">Der Zeitpunkt, zu dem die Verwaltungsbedingung erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="664c8-152">The time the management condition was created.</span></span> <span data-ttu-id="664c8-153">Generierte Dienstseite.</span><span class="sxs-lookup"><span data-stu-id="664c8-153">Generated service side.</span></span> <span data-ttu-id="664c8-154">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="664c8-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="664c8-155">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="664c8-155">modifiedDateTime</span></span>|<span data-ttu-id="664c8-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="664c8-156">DateTimeOffset</span></span>|<span data-ttu-id="664c8-157">Der Zeitpunkt, zu dem die Verwaltungsbedingung zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="664c8-157">The time the management condition was last modified.</span></span> <span data-ttu-id="664c8-158">Aktualisierte Dienstseite.</span><span class="sxs-lookup"><span data-stu-id="664c8-158">Updated service side.</span></span> <span data-ttu-id="664c8-159">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="664c8-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="664c8-160">eTag</span><span class="sxs-lookup"><span data-stu-id="664c8-160">eTag</span></span>|<span data-ttu-id="664c8-161">String</span><span class="sxs-lookup"><span data-stu-id="664c8-161">String</span></span>|<span data-ttu-id="664c8-162">ETag der Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="664c8-162">ETag of the management condition.</span></span> <span data-ttu-id="664c8-163">Aktualisierte Dienstseite.</span><span class="sxs-lookup"><span data-stu-id="664c8-163">Updated service side.</span></span> <span data-ttu-id="664c8-164">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="664c8-164">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="664c8-165">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="664c8-165">applicablePlatforms</span></span>|<span data-ttu-id="664c8-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="664c8-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="664c8-167">Die entsprechenden Plattformen für diese Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="664c8-167">The applicable platforms for this management condition.</span></span> <span data-ttu-id="664c8-168">Von [ManagementCondition](../resources/intune-fencing-managementcondition.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="664c8-168">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="664c8-169">Mögliche Werte: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="664c8-169">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="664c8-170">ipV6Prefix</span><span class="sxs-lookup"><span data-stu-id="664c8-170">ipV6Prefix</span></span>|<span data-ttu-id="664c8-171">String</span><span class="sxs-lookup"><span data-stu-id="664c8-171">String</span></span>|<span data-ttu-id="664c8-172">Das IPv6-Subnetz, mit dem eine Verbindung hergestellt werden soll.</span><span class="sxs-lookup"><span data-stu-id="664c8-172">The IPv6 subnet to be connected to.</span></span> <span data-ttu-id="664c8-173">z. b. 2001: db8::/32</span><span class="sxs-lookup"><span data-stu-id="664c8-173">e.g. 2001:db8::/32</span></span>|
|<span data-ttu-id="664c8-174">ipV6Gateway</span><span class="sxs-lookup"><span data-stu-id="664c8-174">ipV6Gateway</span></span>|<span data-ttu-id="664c8-175">String</span><span class="sxs-lookup"><span data-stu-id="664c8-175">String</span></span>|<span data-ttu-id="664c8-176">Die IPv6-Gateway-Adresse für.</span><span class="sxs-lookup"><span data-stu-id="664c8-176">The IPv6 gateway address to.</span></span> <span data-ttu-id="664c8-177">z. b. 2001: db8:: 1</span><span class="sxs-lookup"><span data-stu-id="664c8-177">e.g 2001:db8::1</span></span>|
|<span data-ttu-id="664c8-178">ipV6DNSServerList</span><span class="sxs-lookup"><span data-stu-id="664c8-178">ipV6DNSServerList</span></span>|<span data-ttu-id="664c8-179">String collection</span><span class="sxs-lookup"><span data-stu-id="664c8-179">String collection</span></span>|<span data-ttu-id="664c8-180">Ein für den Adapter konfigurierter IPv6-DNS-Server.</span><span class="sxs-lookup"><span data-stu-id="664c8-180">An IPv6 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="664c8-181">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="664c8-181">dnsSuffixList</span></span>|<span data-ttu-id="664c8-182">String collection</span><span class="sxs-lookup"><span data-stu-id="664c8-182">String collection</span></span>|<span data-ttu-id="664c8-183">Gültige DNS-Suffixe für das aktuelle Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="664c8-183">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="664c8-184">beispielsweise Seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="664c8-184">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="664c8-185">Antwort</span><span class="sxs-lookup"><span data-stu-id="664c8-185">Response</span></span>
<span data-ttu-id="664c8-186">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="664c8-186">If successful, this method returns a `201 Created` response code and a [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="664c8-187">Beispiel</span><span class="sxs-lookup"><span data-stu-id="664c8-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="664c8-188">Anforderung</span><span class="sxs-lookup"><span data-stu-id="664c8-188">Request</span></span>
<span data-ttu-id="664c8-189">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="664c8-189">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditions
Content-type: application/json
Content-length: 483

{
  "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV6Prefix": "Ip V6Prefix value",
  "ipV6Gateway": "Ip V6Gateway value",
  "ipV6DNSServerList": [
    "Ip V6DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="664c8-190">Antwort</span><span class="sxs-lookup"><span data-stu-id="664c8-190">Response</span></span>
<span data-ttu-id="664c8-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="664c8-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 651

{
  "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
  "id": "25811206-1206-2581-0612-812506128125",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV6Prefix": "Ip V6Prefix value",
  "ipV6Gateway": "Ip V6Gateway value",
  "ipV6DNSServerList": [
    "Ip V6DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```




