---
title: WindowsDomainJoinConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines WindowsDomainJoinConfiguration-Objekts.
ms.openlocfilehash: 78e082aa7baba3e1e1483800d6971a2c376e2234
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062959"
---
# <a name="update-windowsdomainjoinconfiguration"></a><span data-ttu-id="32857-103">WindowsDomainJoinConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="32857-103">Update windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="32857-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="32857-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="32857-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="32857-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="32857-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="32857-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="32857-107">Aktualisieren Sie die Eigenschaften eines [WindowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="32857-107">Update the properties of a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="32857-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="32857-108">Prerequisites</span></span>
<span data-ttu-id="32857-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32857-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32857-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="32857-111">Permission type</span></span>|<span data-ttu-id="32857-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="32857-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32857-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="32857-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="32857-114">&nbsp;&nbsp; **Gerätekonfiguration**</span><span class="sxs-lookup"><span data-stu-id="32857-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="32857-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32857-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="32857-116">&nbsp; &nbsp; **Registrierung**</span><span class="sxs-lookup"><span data-stu-id="32857-116">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="32857-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32857-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="32857-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="32857-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32857-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="32857-119">Not supported.</span></span>|
|<span data-ttu-id="32857-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="32857-120">Application</span></span>|<span data-ttu-id="32857-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="32857-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32857-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="32857-122">HTTP Request</span></span>

<span data-ttu-id="32857-123">**deviceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="32857-123">**Device configuration**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="32857-124">**Registrierung**</span><span class="sxs-lookup"><span data-stu-id="32857-124">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="32857-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="32857-125">Request headers</span></span>
|<span data-ttu-id="32857-126">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="32857-126">Header</span></span>|<span data-ttu-id="32857-127">Wert</span><span class="sxs-lookup"><span data-stu-id="32857-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32857-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="32857-128">Authorization</span></span>|<span data-ttu-id="32857-129">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="32857-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32857-130">Accept</span><span class="sxs-lookup"><span data-stu-id="32857-130">Accept</span></span>|<span data-ttu-id="32857-131">application/json</span><span class="sxs-lookup"><span data-stu-id="32857-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32857-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="32857-132">Request body</span></span>
<span data-ttu-id="32857-133">Geben Sie im Textkörper Anforderung für das Objekt [WindowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="32857-133">In the request body, supply a JSON representation for the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

<span data-ttu-id="32857-134">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [WindowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="32857-134">The following table shows the properties that are required when you create the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>

|<span data-ttu-id="32857-135">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="32857-135">Property</span></span>|<span data-ttu-id="32857-136">Typ</span><span class="sxs-lookup"><span data-stu-id="32857-136">Type</span></span>|<span data-ttu-id="32857-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="32857-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32857-138">id</span><span class="sxs-lookup"><span data-stu-id="32857-138">id</span></span>|<span data-ttu-id="32857-139">String</span><span class="sxs-lookup"><span data-stu-id="32857-139">String</span></span>|<span data-ttu-id="32857-140">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="32857-140">Key of the entity.</span></span> <span data-ttu-id="32857-141">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="32857-141">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32857-142">**deviceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="32857-142">**Device configuration**</span></span>|
|<span data-ttu-id="32857-143">activeDirectoryDomainName</span><span class="sxs-lookup"><span data-stu-id="32857-143">activeDirectoryDomainName</span></span>|<span data-ttu-id="32857-144">String</span><span class="sxs-lookup"><span data-stu-id="32857-144">String</span></span>|<span data-ttu-id="32857-145">Active Directory-Domänennamen zur Teilnahme an.</span><span class="sxs-lookup"><span data-stu-id="32857-145">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="32857-146">computerNameStaticPrefix</span><span class="sxs-lookup"><span data-stu-id="32857-146">computerNameStaticPrefix</span></span>|<span data-ttu-id="32857-147">String</span><span class="sxs-lookup"><span data-stu-id="32857-147">String</span></span>|<span data-ttu-id="32857-148">Feste Präfix für Computername verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="32857-148">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="32857-149">computerNameSuffixRandomCharCount</span><span class="sxs-lookup"><span data-stu-id="32857-149">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="32857-150">Int32</span><span class="sxs-lookup"><span data-stu-id="32857-150">Int32</span></span>|<span data-ttu-id="32857-151">Dynamisch generierte Zeichen als Suffix für den Computer verwendet.</span><span class="sxs-lookup"><span data-stu-id="32857-151">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="32857-152">Gültige Werte 3 bis 14</span><span class="sxs-lookup"><span data-stu-id="32857-152">Valid values 3 to 14</span></span>|
|<span data-ttu-id="32857-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="32857-153">createdDateTime</span></span>|<span data-ttu-id="32857-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32857-154">DateTimeOffset</span></span>|<span data-ttu-id="32857-155">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="32857-155">DateTime the object was created.</span></span> <span data-ttu-id="32857-156">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="32857-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32857-157">description</span><span class="sxs-lookup"><span data-stu-id="32857-157">description</span></span>|<span data-ttu-id="32857-158">String</span><span class="sxs-lookup"><span data-stu-id="32857-158">String</span></span>|<span data-ttu-id="32857-159">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="32857-159">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="32857-160">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="32857-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32857-161">displayName</span><span class="sxs-lookup"><span data-stu-id="32857-161">displayName</span></span>|<span data-ttu-id="32857-162">String</span><span class="sxs-lookup"><span data-stu-id="32857-162">String</span></span>|<span data-ttu-id="32857-163">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="32857-163">Admin provided name of the device configuration.</span></span> <span data-ttu-id="32857-164">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="32857-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32857-165">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="32857-165">lastModifiedDateTime</span></span>|<span data-ttu-id="32857-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32857-166">DateTimeOffset</span></span>|<span data-ttu-id="32857-167">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="32857-167">DateTime the object was last modified.</span></span> <span data-ttu-id="32857-168">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="32857-168">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32857-169">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="32857-169">organizationalUnit</span></span>|<span data-ttu-id="32857-170">String</span><span class="sxs-lookup"><span data-stu-id="32857-170">String</span></span>|<span data-ttu-id="32857-171">Organisationseinheit (OU), in dem das Computerkonto erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="32857-171">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="32857-172">Wenn dieser Parameter auf NULL ist, wird der bekannten Computer-Container-Objekt verwendet werden, wie in der Domäne veröffentlicht.</span><span class="sxs-lookup"><span data-stu-id="32857-172">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="32857-173">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="32857-173">roleScopeTagIds</span></span>|<span data-ttu-id="32857-174">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="32857-174">String collection</span></span>|<span data-ttu-id="32857-175">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="32857-175">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="32857-176">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="32857-176">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32857-177">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="32857-177">supportsScopeTags</span></span>|<span data-ttu-id="32857-178">Boolesch</span><span class="sxs-lookup"><span data-stu-id="32857-178">Boolean</span></span>|<span data-ttu-id="32857-179">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="32857-179">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="32857-180">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="32857-180">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="32857-181">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="32857-181">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="32857-182">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="32857-182">This property is read-only.</span></span> <span data-ttu-id="32857-183">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="32857-183">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32857-184">Version</span><span class="sxs-lookup"><span data-stu-id="32857-184">version</span></span>|<span data-ttu-id="32857-185">Int32</span><span class="sxs-lookup"><span data-stu-id="32857-185">Int32</span></span>|<span data-ttu-id="32857-186">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="32857-186">Version of the device configuration.</span></span> <span data-ttu-id="32857-187">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="32857-187">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



<span data-ttu-id="32857-188">Hinweis: Anforderung Body-Eigenschaften Unterstützung hängt vom Kontext des Anrufs ab.</span><span class="sxs-lookup"><span data-stu-id="32857-188">Note: Request body properties support depends on the context of the call.</span></span>  <span data-ttu-id="32857-189">Nicht alle Eigenschaften sind für alle Workflows geeignet.</span><span class="sxs-lookup"><span data-stu-id="32857-189">Not all properties are appropriate for all workflows.</span></span>

## <a name="response"></a><span data-ttu-id="32857-190">Antwort</span><span class="sxs-lookup"><span data-stu-id="32857-190">Response</span></span>
<span data-ttu-id="32857-191">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [WindowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="32857-191">If successful, this method returns a `200 OK` response code and an updated [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32857-192">Beispiel</span><span class="sxs-lookup"><span data-stu-id="32857-192">Example</span></span>
### <a name="request"></a><span data-ttu-id="32857-193">Anforderung</span><span class="sxs-lookup"><span data-stu-id="32857-193">Request</span></span>
<span data-ttu-id="32857-194">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="32857-194">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 344

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "computerNameStaticPrefix": "Computer Name Static Prefix value",
  "computerNameSuffixRandomCharCount": 1,
  "activeDirectoryDomainName": "Active Directory Domain Name value"
}
```

### <a name="response"></a><span data-ttu-id="32857-195">Antwort</span><span class="sxs-lookup"><span data-stu-id="32857-195">Response</span></span>
<span data-ttu-id="32857-196">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="32857-196">Here is an example of the response.</span></span> <span data-ttu-id="32857-197">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="32857-197">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="32857-198">Eigenschaften von tatsächlichen Aufrufe zurückgegebene variieren je nach Kontext.</span><span class="sxs-lookup"><span data-stu-id="32857-198">Properties returned by actual calls vary according to the context.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 521

{
  "@odata.type": "#microsoft.graph.windowsDomainJoinConfiguration",
  "id": "40118d08-8d08-4011-088d-1140088d1140",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "computerNameStaticPrefix": "Computer Name Static Prefix value",
  "computerNameSuffixRandomCharCount": 1,
  "activeDirectoryDomainName": "Active Directory Domain Name value"
}
```



