---
title: NetworkIPv6ConfigurationManagementCondition aktualisieren
description: Aktualisieren Sie die Eigenschaften eines networkIPv6ConfigurationManagementCondition-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b4309110d0f7075a5a841521980b73dba9cd3906
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424308"
---
# <a name="update-networkipv6configurationmanagementcondition"></a><span data-ttu-id="5c97c-103">NetworkIPv6ConfigurationManagementCondition aktualisieren</span><span class="sxs-lookup"><span data-stu-id="5c97c-103">Update networkIPv6ConfigurationManagementCondition</span></span>

> <span data-ttu-id="5c97c-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="5c97c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5c97c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5c97c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5c97c-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5c97c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c97c-107">Aktualisieren Sie die Eigenschaften eines [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="5c97c-107">Update the properties of a [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c97c-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5c97c-108">Prerequisites</span></span>
<span data-ttu-id="5c97c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5c97c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5c97c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5c97c-111">Permission type</span></span>|<span data-ttu-id="5c97c-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5c97c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c97c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5c97c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5c97c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c97c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5c97c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5c97c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c97c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5c97c-116">Not supported.</span></span>|
|<span data-ttu-id="5c97c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5c97c-117">Application</span></span>|<span data-ttu-id="5c97c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5c97c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c97c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5c97c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a><span data-ttu-id="5c97c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5c97c-120">Request headers</span></span>
|<span data-ttu-id="5c97c-121">Header</span><span class="sxs-lookup"><span data-stu-id="5c97c-121">Header</span></span>|<span data-ttu-id="5c97c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="5c97c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c97c-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="5c97c-123">Authorization</span></span>|<span data-ttu-id="5c97c-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5c97c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c97c-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5c97c-125">Accept</span></span>|<span data-ttu-id="5c97c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5c97c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c97c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5c97c-127">Request body</span></span>
<span data-ttu-id="5c97c-128">Geben Sie im Textkörper Anforderung für das Objekt [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="5c97c-128">In the request body, supply a JSON representation for the [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object.</span></span>

<span data-ttu-id="5c97c-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="5c97c-129">The following table shows the properties that are required when you create the [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md).</span></span>

|<span data-ttu-id="5c97c-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5c97c-130">Property</span></span>|<span data-ttu-id="5c97c-131">Typ</span><span class="sxs-lookup"><span data-stu-id="5c97c-131">Type</span></span>|<span data-ttu-id="5c97c-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5c97c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c97c-133">id</span><span class="sxs-lookup"><span data-stu-id="5c97c-133">id</span></span>|<span data-ttu-id="5c97c-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c97c-134">String</span></span>|<span data-ttu-id="5c97c-135">Eindeutiger Bezeichner für die Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="5c97c-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="5c97c-136">System generierten Wert, die beim Erstellen zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="5c97c-136">System generated value assigned when created.</span></span> <span data-ttu-id="5c97c-137">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="5c97c-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="5c97c-138">uniqueName</span><span class="sxs-lookup"><span data-stu-id="5c97c-138">uniqueName</span></span>|<span data-ttu-id="5c97c-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c97c-139">String</span></span>|<span data-ttu-id="5c97c-140">Eindeutiger Name für die Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="5c97c-140">Unique name for the management condition.</span></span> <span data-ttu-id="5c97c-141">In Management Bedingung Ausdrücken verwendet.</span><span class="sxs-lookup"><span data-stu-id="5c97c-141">Used in management condition expressions.</span></span> <span data-ttu-id="5c97c-142">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="5c97c-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="5c97c-143">displayName</span><span class="sxs-lookup"><span data-stu-id="5c97c-143">displayName</span></span>|<span data-ttu-id="5c97c-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c97c-144">String</span></span>|<span data-ttu-id="5c97c-145">Der Administrator definierter Name der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="5c97c-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="5c97c-146">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="5c97c-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="5c97c-147">description</span><span class="sxs-lookup"><span data-stu-id="5c97c-147">description</span></span>|<span data-ttu-id="5c97c-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c97c-148">String</span></span>|<span data-ttu-id="5c97c-149">Der Administrator definiert die Beschreibung der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="5c97c-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="5c97c-150">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="5c97c-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="5c97c-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5c97c-151">createdDateTime</span></span>|<span data-ttu-id="5c97c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c97c-152">DateTimeOffset</span></span>|<span data-ttu-id="5c97c-153">Der Zeitpunkt, an die Bedingung Management erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="5c97c-153">The time the management condition was created.</span></span> <span data-ttu-id="5c97c-154">Generierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="5c97c-154">Generated service side.</span></span> <span data-ttu-id="5c97c-155">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="5c97c-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="5c97c-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5c97c-156">modifiedDateTime</span></span>|<span data-ttu-id="5c97c-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c97c-157">DateTimeOffset</span></span>|<span data-ttu-id="5c97c-158">Die Zeit, die die Bedingung Management zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="5c97c-158">The time the management condition was last modified.</span></span> <span data-ttu-id="5c97c-159">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="5c97c-159">Updated service side.</span></span> <span data-ttu-id="5c97c-160">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="5c97c-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="5c97c-161">eTag</span><span class="sxs-lookup"><span data-stu-id="5c97c-161">eTag</span></span>|<span data-ttu-id="5c97c-162">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c97c-162">String</span></span>|<span data-ttu-id="5c97c-163">ETag der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="5c97c-163">ETag of the management condition.</span></span> <span data-ttu-id="5c97c-164">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="5c97c-164">Updated service side.</span></span> <span data-ttu-id="5c97c-165">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="5c97c-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="5c97c-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="5c97c-166">applicablePlatforms</span></span>|<span data-ttu-id="5c97c-167">[DevicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="5c97c-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="5c97c-168">Die entsprechenden Plattformen für diese Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="5c97c-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="5c97c-169">Geerbt von [ManagementCondition](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="5c97c-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="5c97c-170">Mögliche Werte sind: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater` und `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="5c97c-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="5c97c-171">ipV6Prefix</span><span class="sxs-lookup"><span data-stu-id="5c97c-171">ipV6Prefix</span></span>|<span data-ttu-id="5c97c-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c97c-172">String</span></span>|<span data-ttu-id="5c97c-173">Die IPv6-Subnetz mit verbunden sein.</span><span class="sxs-lookup"><span data-stu-id="5c97c-173">The IPv6 subnet to be connected to.</span></span> <span data-ttu-id="5c97c-174">Diese Vorgaben unter 2001:db8:: / 32</span><span class="sxs-lookup"><span data-stu-id="5c97c-174">e.g. 2001:db8::/32</span></span>|
|<span data-ttu-id="5c97c-175">ipV6Gateway</span><span class="sxs-lookup"><span data-stu-id="5c97c-175">ipV6Gateway</span></span>|<span data-ttu-id="5c97c-176">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c97c-176">String</span></span>|<span data-ttu-id="5c97c-177">Die IPv6-Gateway-Adresse zu.</span><span class="sxs-lookup"><span data-stu-id="5c97c-177">The IPv6 gateway address to.</span></span> <span data-ttu-id="5c97c-178">z. B. 2001:db8::1</span><span class="sxs-lookup"><span data-stu-id="5c97c-178">e.g 2001:db8::1</span></span>|
|<span data-ttu-id="5c97c-179">ipV6DNSServerList</span><span class="sxs-lookup"><span data-stu-id="5c97c-179">ipV6DNSServerList</span></span>|<span data-ttu-id="5c97c-180">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="5c97c-180">String collection</span></span>|<span data-ttu-id="5c97c-181">Eine IPv6-DNS-Server für den Adapter konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="5c97c-181">An IPv6 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="5c97c-182">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="5c97c-182">dnsSuffixList</span></span>|<span data-ttu-id="5c97c-183">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="5c97c-183">String collection</span></span>|<span data-ttu-id="5c97c-184">Gültige DNS-Suffixe für das aktuelle Netzwerk.</span><span class="sxs-lookup"><span data-stu-id="5c97c-184">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="5c97c-185">Diese Vorgaben unter seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="5c97c-185">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="5c97c-186">Antwort</span><span class="sxs-lookup"><span data-stu-id="5c97c-186">Response</span></span>
<span data-ttu-id="5c97c-187">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="5c97c-187">If successful, this method returns a `200 OK` response code and an updated [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c97c-188">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5c97c-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c97c-189">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5c97c-189">Request</span></span>
<span data-ttu-id="5c97c-190">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5c97c-190">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
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

### <a name="response"></a><span data-ttu-id="5c97c-191">Antwort</span><span class="sxs-lookup"><span data-stu-id="5c97c-191">Response</span></span>
<span data-ttu-id="5c97c-p114">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5c97c-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




