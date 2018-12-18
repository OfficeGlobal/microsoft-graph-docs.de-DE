---
title: Erstellen von networkIPv6ConfigurationManagementCondition
description: Erstellen eines neuen networkIPv6ConfigurationManagementCondition-Objekts.
author: tfitzmac
ms.openlocfilehash: b59a194ac7d7853ff958435406ff7e7af01a21b1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356434"
---
# <a name="create-networkipv6configurationmanagementcondition"></a><span data-ttu-id="7144f-103">Erstellen von networkIPv6ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="7144f-103">Create networkIPv6ConfigurationManagementCondition</span></span>

> <span data-ttu-id="7144f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7144f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7144f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7144f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7144f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7144f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7144f-107">Erstellen eines neuen [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="7144f-107">Create a new [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7144f-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7144f-108">Prerequisites</span></span>
<span data-ttu-id="7144f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7144f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7144f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7144f-111">Permission type</span></span>|<span data-ttu-id="7144f-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7144f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7144f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7144f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7144f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7144f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7144f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7144f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7144f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7144f-116">Not supported.</span></span>|
|<span data-ttu-id="7144f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7144f-117">Application</span></span>|<span data-ttu-id="7144f-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7144f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7144f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7144f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="7144f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7144f-120">Request headers</span></span>
|<span data-ttu-id="7144f-121">Header</span><span class="sxs-lookup"><span data-stu-id="7144f-121">Header</span></span>|<span data-ttu-id="7144f-122">Wert</span><span class="sxs-lookup"><span data-stu-id="7144f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7144f-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="7144f-123">Authorization</span></span>|<span data-ttu-id="7144f-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7144f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7144f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7144f-125">Accept</span></span>|<span data-ttu-id="7144f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7144f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7144f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7144f-127">Request body</span></span>
<span data-ttu-id="7144f-128">Geben Sie im Textkörper Anforderung für das Objekt networkIPv6ConfigurationManagementCondition eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="7144f-128">In the request body, supply a JSON representation for the networkIPv6ConfigurationManagementCondition object.</span></span>

<span data-ttu-id="7144f-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die networkIPv6ConfigurationManagementCondition erstellen.</span><span class="sxs-lookup"><span data-stu-id="7144f-129">The following table shows the properties that are required when you create the networkIPv6ConfigurationManagementCondition.</span></span>

|<span data-ttu-id="7144f-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7144f-130">Property</span></span>|<span data-ttu-id="7144f-131">Typ</span><span class="sxs-lookup"><span data-stu-id="7144f-131">Type</span></span>|<span data-ttu-id="7144f-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7144f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7144f-133">id</span><span class="sxs-lookup"><span data-stu-id="7144f-133">id</span></span>|<span data-ttu-id="7144f-134">String</span><span class="sxs-lookup"><span data-stu-id="7144f-134">String</span></span>|<span data-ttu-id="7144f-135">Eindeutiger Bezeichner für die Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="7144f-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="7144f-136">System generierten Wert, die beim Erstellen zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="7144f-136">System generated value assigned when created.</span></span> <span data-ttu-id="7144f-137">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="7144f-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="7144f-138">uniqueName</span><span class="sxs-lookup"><span data-stu-id="7144f-138">uniqueName</span></span>|<span data-ttu-id="7144f-139">String</span><span class="sxs-lookup"><span data-stu-id="7144f-139">String</span></span>|<span data-ttu-id="7144f-140">Eindeutiger Name für die Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="7144f-140">Unique name for the management condition.</span></span> <span data-ttu-id="7144f-141">In Management Bedingung Ausdrücken verwendet.</span><span class="sxs-lookup"><span data-stu-id="7144f-141">Used in management condition expressions.</span></span> <span data-ttu-id="7144f-142">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="7144f-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="7144f-143">displayName</span><span class="sxs-lookup"><span data-stu-id="7144f-143">displayName</span></span>|<span data-ttu-id="7144f-144">String</span><span class="sxs-lookup"><span data-stu-id="7144f-144">String</span></span>|<span data-ttu-id="7144f-145">Der Administrator definierter Name der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="7144f-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="7144f-146">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="7144f-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="7144f-147">description</span><span class="sxs-lookup"><span data-stu-id="7144f-147">description</span></span>|<span data-ttu-id="7144f-148">String</span><span class="sxs-lookup"><span data-stu-id="7144f-148">String</span></span>|<span data-ttu-id="7144f-149">Der Administrator definiert die Beschreibung der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="7144f-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="7144f-150">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="7144f-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="7144f-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7144f-151">createdDateTime</span></span>|<span data-ttu-id="7144f-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7144f-152">DateTimeOffset</span></span>|<span data-ttu-id="7144f-153">Der Zeitpunkt, an die Bedingung Management erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="7144f-153">The time the management condition was created.</span></span> <span data-ttu-id="7144f-154">Generierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="7144f-154">Generated service side.</span></span> <span data-ttu-id="7144f-155">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="7144f-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="7144f-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7144f-156">modifiedDateTime</span></span>|<span data-ttu-id="7144f-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7144f-157">DateTimeOffset</span></span>|<span data-ttu-id="7144f-158">Die Zeit, die die Bedingung Management zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="7144f-158">The time the management condition was last modified.</span></span> <span data-ttu-id="7144f-159">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="7144f-159">Updated service side.</span></span> <span data-ttu-id="7144f-160">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="7144f-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="7144f-161">eTag</span><span class="sxs-lookup"><span data-stu-id="7144f-161">eTag</span></span>|<span data-ttu-id="7144f-162">String</span><span class="sxs-lookup"><span data-stu-id="7144f-162">String</span></span>|<span data-ttu-id="7144f-163">ETag der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="7144f-163">ETag of the management condition.</span></span> <span data-ttu-id="7144f-164">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="7144f-164">Updated service side.</span></span> <span data-ttu-id="7144f-165">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="7144f-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="7144f-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="7144f-166">applicablePlatforms</span></span>|<span data-ttu-id="7144f-167">[DevicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="7144f-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="7144f-168">Die entsprechenden Plattformen für diese Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="7144f-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="7144f-169">Geerbt von [ManagementCondition](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="7144f-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="7144f-170">Mögliche Werte sind: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater` und `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="7144f-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="7144f-171">ipV6Prefix</span><span class="sxs-lookup"><span data-stu-id="7144f-171">ipV6Prefix</span></span>|<span data-ttu-id="7144f-172">String</span><span class="sxs-lookup"><span data-stu-id="7144f-172">String</span></span>|<span data-ttu-id="7144f-173">Die IPv6-Subnetz mit verbunden sein.</span><span class="sxs-lookup"><span data-stu-id="7144f-173">The IPv6 subnet to be connected to.</span></span> <span data-ttu-id="7144f-174">Diese Vorgaben unter 2001:db8:: / 32</span><span class="sxs-lookup"><span data-stu-id="7144f-174">e.g. 2001:db8::/32</span></span>|
|<span data-ttu-id="7144f-175">ipV6Gateway</span><span class="sxs-lookup"><span data-stu-id="7144f-175">ipV6Gateway</span></span>|<span data-ttu-id="7144f-176">String</span><span class="sxs-lookup"><span data-stu-id="7144f-176">String</span></span>|<span data-ttu-id="7144f-177">Die IPv6-Gateway-Adresse zu.</span><span class="sxs-lookup"><span data-stu-id="7144f-177">The IPv6 gateway address to.</span></span> <span data-ttu-id="7144f-178">z. B. 2001:db8::1</span><span class="sxs-lookup"><span data-stu-id="7144f-178">e.g 2001:db8::1</span></span>|
|<span data-ttu-id="7144f-179">ipV6DNSServerList</span><span class="sxs-lookup"><span data-stu-id="7144f-179">ipV6DNSServerList</span></span>|<span data-ttu-id="7144f-180">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="7144f-180">String collection</span></span>|<span data-ttu-id="7144f-181">Eine IPv6-DNS-Server für den Adapter konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="7144f-181">An IPv6 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="7144f-182">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="7144f-182">dnsSuffixList</span></span>|<span data-ttu-id="7144f-183">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="7144f-183">String collection</span></span>|<span data-ttu-id="7144f-184">Gültige DNS-Suffixe für das aktuelle Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="7144f-184">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="7144f-185">Diese Vorgaben unter seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="7144f-185">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="7144f-186">Antwort</span><span class="sxs-lookup"><span data-stu-id="7144f-186">Response</span></span>
<span data-ttu-id="7144f-187">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="7144f-187">If successful, this method returns a `201 Created` response code and a [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7144f-188">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7144f-188">Example</span></span>
### <a name="request"></a><span data-ttu-id="7144f-189">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7144f-189">Request</span></span>
<span data-ttu-id="7144f-190">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7144f-190">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7144f-191">Antwort</span><span class="sxs-lookup"><span data-stu-id="7144f-191">Response</span></span>
<span data-ttu-id="7144f-p114">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7144f-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





