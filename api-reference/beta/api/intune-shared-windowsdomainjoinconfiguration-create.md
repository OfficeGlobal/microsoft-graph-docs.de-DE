---
title: Erstellen von windowsDomainJoinConfiguration
description: Erstellen eines neuen WindowsDomainJoinConfiguration-Objekts.
ms.openlocfilehash: 8069dfac727ee24d96f72875a4cec19fa42b8baa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065461"
---
# <a name="create-windowsdomainjoinconfiguration"></a><span data-ttu-id="174c7-103">Erstellen von windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="174c7-103">Create windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="174c7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="174c7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="174c7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="174c7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="174c7-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="174c7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="174c7-107">Erstellen eines neuen [WindowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="174c7-107">Create a new [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="174c7-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="174c7-108">Prerequisites</span></span>
<span data-ttu-id="174c7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="174c7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="174c7-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="174c7-111">Permission type</span></span>|<span data-ttu-id="174c7-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="174c7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="174c7-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="174c7-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="174c7-114">&nbsp;&nbsp; **Gerätekonfiguration**</span><span class="sxs-lookup"><span data-stu-id="174c7-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="174c7-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="174c7-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="174c7-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="174c7-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="174c7-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="174c7-117">Not supported.</span></span>|
|<span data-ttu-id="174c7-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="174c7-118">Application</span></span>|<span data-ttu-id="174c7-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="174c7-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="174c7-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="174c7-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="174c7-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="174c7-121">Request headers</span></span>

|<span data-ttu-id="174c7-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="174c7-122">Header</span></span>|<span data-ttu-id="174c7-123">Wert</span><span class="sxs-lookup"><span data-stu-id="174c7-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="174c7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="174c7-124">Authorization</span></span>|<span data-ttu-id="174c7-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="174c7-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="174c7-126">Accept</span><span class="sxs-lookup"><span data-stu-id="174c7-126">Accept</span></span>|<span data-ttu-id="174c7-127">application/json</span><span class="sxs-lookup"><span data-stu-id="174c7-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="174c7-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="174c7-128">Request body</span></span>

<span data-ttu-id="174c7-129">Geben Sie im Textkörper Anforderung für das Objekt WindowsDomainJoinConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="174c7-129">In the request body, supply a JSON representation for the windowsDomainJoinConfiguration object.</span></span>

<span data-ttu-id="174c7-130">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die WindowsDomainJoinConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="174c7-130">The following table shows the properties that are required when you create the windowsDomainJoinConfiguration.</span></span>

|<span data-ttu-id="174c7-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="174c7-131">Property</span></span>|<span data-ttu-id="174c7-132">Typ</span><span class="sxs-lookup"><span data-stu-id="174c7-132">Type</span></span>|<span data-ttu-id="174c7-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="174c7-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="174c7-134">id</span><span class="sxs-lookup"><span data-stu-id="174c7-134">id</span></span>|<span data-ttu-id="174c7-135">String</span><span class="sxs-lookup"><span data-stu-id="174c7-135">String</span></span>|<span data-ttu-id="174c7-136">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="174c7-136">Key of the entity.</span></span> <span data-ttu-id="174c7-137">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="174c7-137">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="174c7-138">**deviceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="174c7-138">**Device configuration**</span></span>|
|<span data-ttu-id="174c7-139">activeDirectoryDomainName</span><span class="sxs-lookup"><span data-stu-id="174c7-139">activeDirectoryDomainName</span></span>|<span data-ttu-id="174c7-140">String</span><span class="sxs-lookup"><span data-stu-id="174c7-140">String</span></span>|<span data-ttu-id="174c7-141">Active Directory-Domänennamen zur Teilnahme an.</span><span class="sxs-lookup"><span data-stu-id="174c7-141">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="174c7-142">computerNameStaticPrefix</span><span class="sxs-lookup"><span data-stu-id="174c7-142">computerNameStaticPrefix</span></span>|<span data-ttu-id="174c7-143">String</span><span class="sxs-lookup"><span data-stu-id="174c7-143">String</span></span>|<span data-ttu-id="174c7-144">Feste Präfix für Computername verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="174c7-144">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="174c7-145">computerNameSuffixRandomCharCount</span><span class="sxs-lookup"><span data-stu-id="174c7-145">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="174c7-146">Int32</span><span class="sxs-lookup"><span data-stu-id="174c7-146">Int32</span></span>|<span data-ttu-id="174c7-147">Dynamisch generierte Zeichen als Suffix für den Computer verwendet.</span><span class="sxs-lookup"><span data-stu-id="174c7-147">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="174c7-148">Gültige Werte 3 bis 14</span><span class="sxs-lookup"><span data-stu-id="174c7-148">Valid values 3 to 14</span></span>|
|<span data-ttu-id="174c7-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="174c7-149">createdDateTime</span></span>|<span data-ttu-id="174c7-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="174c7-150">DateTimeOffset</span></span>|<span data-ttu-id="174c7-151">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="174c7-151">DateTime the object was created.</span></span> <span data-ttu-id="174c7-152">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="174c7-152">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="174c7-153">description</span><span class="sxs-lookup"><span data-stu-id="174c7-153">description</span></span>|<span data-ttu-id="174c7-154">String</span><span class="sxs-lookup"><span data-stu-id="174c7-154">String</span></span>|<span data-ttu-id="174c7-155">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="174c7-155">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="174c7-156">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="174c7-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="174c7-157">displayName</span><span class="sxs-lookup"><span data-stu-id="174c7-157">displayName</span></span>|<span data-ttu-id="174c7-158">String</span><span class="sxs-lookup"><span data-stu-id="174c7-158">String</span></span>|<span data-ttu-id="174c7-159">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="174c7-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="174c7-160">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="174c7-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="174c7-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="174c7-161">lastModifiedDateTime</span></span>|<span data-ttu-id="174c7-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="174c7-162">DateTimeOffset</span></span>|<span data-ttu-id="174c7-163">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="174c7-163">DateTime the object was last modified.</span></span> <span data-ttu-id="174c7-164">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="174c7-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="174c7-165">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="174c7-165">organizationalUnit</span></span>|<span data-ttu-id="174c7-166">String</span><span class="sxs-lookup"><span data-stu-id="174c7-166">String</span></span>|<span data-ttu-id="174c7-167">Organisationseinheit (OU), in dem das Computerkonto erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="174c7-167">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="174c7-168">Wenn dieser Parameter auf NULL ist, wird der bekannten Computer-Container-Objekt verwendet werden, wie in der Domäne veröffentlicht.</span><span class="sxs-lookup"><span data-stu-id="174c7-168">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="174c7-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="174c7-169">roleScopeTagIds</span></span>|<span data-ttu-id="174c7-170">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="174c7-170">String collection</span></span>|<span data-ttu-id="174c7-171">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="174c7-171">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="174c7-172">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="174c7-172">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="174c7-173">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="174c7-173">supportsScopeTags</span></span>|<span data-ttu-id="174c7-174">Boolesch</span><span class="sxs-lookup"><span data-stu-id="174c7-174">Boolean</span></span>|<span data-ttu-id="174c7-175">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="174c7-175">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="174c7-176">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="174c7-176">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="174c7-177">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="174c7-177">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="174c7-178">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="174c7-178">This property is read-only.</span></span> <span data-ttu-id="174c7-179">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="174c7-179">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="174c7-180">Version</span><span class="sxs-lookup"><span data-stu-id="174c7-180">version</span></span>|<span data-ttu-id="174c7-181">Int32</span><span class="sxs-lookup"><span data-stu-id="174c7-181">Int32</span></span>|<span data-ttu-id="174c7-182">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="174c7-182">Version of the device configuration.</span></span> <span data-ttu-id="174c7-183">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="174c7-183">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="174c7-184">Antwort</span><span class="sxs-lookup"><span data-stu-id="174c7-184">Response</span></span>

<span data-ttu-id="174c7-185">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [WindowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="174c7-185">If successful, this method returns a `201 Created` response code and a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="174c7-186">Beispiel</span><span class="sxs-lookup"><span data-stu-id="174c7-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="174c7-187">Anforderung</span><span class="sxs-lookup"><span data-stu-id="174c7-187">Request</span></span>

<span data-ttu-id="174c7-188">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="174c7-188">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 559

{
  "@odata.type": "#microsoft.graph.windowsDomainJoinConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "computerNameStaticPrefix": "Computer Name Static Prefix value",
  "computerNameSuffixRandomCharCount": 1,
  "activeDirectoryDomainName": "Active Directory Domain Name value",
  "organizationalUnit": "Organizational Unit value"
}
```

### <a name="response"></a><span data-ttu-id="174c7-189">Antwort</span><span class="sxs-lookup"><span data-stu-id="174c7-189">Response</span></span>

<span data-ttu-id="174c7-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="174c7-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 667

{
  "@odata.type": "#microsoft.graph.windowsDomainJoinConfiguration",
  "id": "40118d08-8d08-4011-088d-1140088d1140",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "computerNameStaticPrefix": "Computer Name Static Prefix value",
  "computerNameSuffixRandomCharCount": 1,
  "activeDirectoryDomainName": "Active Directory Domain Name value",
  "organizationalUnit": "Organizational Unit value"
}
```



