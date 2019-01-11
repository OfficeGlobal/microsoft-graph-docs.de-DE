---
title: Erstellen von windowsPhone81TrustedRootCertificate
description: Erstellen eines neuen windowsPhone81TrustedRootCertificate-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 55c36c25ab8eaa4895df21d0b7c60dc37179462d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844373"
---
# <a name="create-windowsphone81trustedrootcertificate"></a><span data-ttu-id="19b53-103">Erstellen von windowsPhone81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="19b53-103">Create windowsPhone81TrustedRootCertificate</span></span>

> <span data-ttu-id="19b53-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="19b53-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19b53-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19b53-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="19b53-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="19b53-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="19b53-107">Erstellen eines neuen [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="19b53-107">Create a new [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="19b53-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="19b53-108">Prerequisites</span></span>
<span data-ttu-id="19b53-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19b53-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19b53-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="19b53-111">Permission type</span></span>|<span data-ttu-id="19b53-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="19b53-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19b53-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="19b53-113">Delegated (work or school account)</span></span>|<span data-ttu-id="19b53-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19b53-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="19b53-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="19b53-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19b53-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="19b53-116">Not supported.</span></span>|
|<span data-ttu-id="19b53-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="19b53-117">Application</span></span>|<span data-ttu-id="19b53-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="19b53-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19b53-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="19b53-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="19b53-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="19b53-120">Request headers</span></span>
|<span data-ttu-id="19b53-121">Header</span><span class="sxs-lookup"><span data-stu-id="19b53-121">Header</span></span>|<span data-ttu-id="19b53-122">Wert</span><span class="sxs-lookup"><span data-stu-id="19b53-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19b53-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="19b53-123">Authorization</span></span>|<span data-ttu-id="19b53-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="19b53-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19b53-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="19b53-125">Accept</span></span>|<span data-ttu-id="19b53-126">application/json</span><span class="sxs-lookup"><span data-stu-id="19b53-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19b53-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="19b53-127">Request body</span></span>
<span data-ttu-id="19b53-128">Geben Sie im Textkörper Anforderung für das Objekt windowsPhone81TrustedRootCertificate eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="19b53-128">In the request body, supply a JSON representation for the windowsPhone81TrustedRootCertificate object.</span></span>

<span data-ttu-id="19b53-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die windowsPhone81TrustedRootCertificate erstellen.</span><span class="sxs-lookup"><span data-stu-id="19b53-129">The following table shows the properties that are required when you create the windowsPhone81TrustedRootCertificate.</span></span>

|<span data-ttu-id="19b53-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="19b53-130">Property</span></span>|<span data-ttu-id="19b53-131">Typ</span><span class="sxs-lookup"><span data-stu-id="19b53-131">Type</span></span>|<span data-ttu-id="19b53-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="19b53-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19b53-133">id</span><span class="sxs-lookup"><span data-stu-id="19b53-133">id</span></span>|<span data-ttu-id="19b53-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="19b53-134">String</span></span>|<span data-ttu-id="19b53-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="19b53-135">Key of the entity.</span></span> <span data-ttu-id="19b53-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19b53-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19b53-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="19b53-137">lastModifiedDateTime</span></span>|<span data-ttu-id="19b53-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19b53-138">DateTimeOffset</span></span>|<span data-ttu-id="19b53-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="19b53-139">DateTime the object was last modified.</span></span> <span data-ttu-id="19b53-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19b53-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19b53-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="19b53-141">roleScopeTagIds</span></span>|<span data-ttu-id="19b53-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="19b53-142">String collection</span></span>|<span data-ttu-id="19b53-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="19b53-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="19b53-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19b53-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19b53-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="19b53-145">supportsScopeTags</span></span>|<span data-ttu-id="19b53-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="19b53-146">Boolean</span></span>|<span data-ttu-id="19b53-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19b53-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="19b53-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="19b53-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="19b53-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="19b53-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="19b53-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="19b53-150">This property is read-only.</span></span> <span data-ttu-id="19b53-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19b53-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19b53-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="19b53-152">createdDateTime</span></span>|<span data-ttu-id="19b53-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19b53-153">DateTimeOffset</span></span>|<span data-ttu-id="19b53-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="19b53-154">DateTime the object was created.</span></span> <span data-ttu-id="19b53-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19b53-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19b53-156">description</span><span class="sxs-lookup"><span data-stu-id="19b53-156">description</span></span>|<span data-ttu-id="19b53-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="19b53-157">String</span></span>|<span data-ttu-id="19b53-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="19b53-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="19b53-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19b53-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19b53-160">displayName</span><span class="sxs-lookup"><span data-stu-id="19b53-160">displayName</span></span>|<span data-ttu-id="19b53-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="19b53-161">String</span></span>|<span data-ttu-id="19b53-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="19b53-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="19b53-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19b53-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19b53-164">Version</span><span class="sxs-lookup"><span data-stu-id="19b53-164">version</span></span>|<span data-ttu-id="19b53-165">Int32</span><span class="sxs-lookup"><span data-stu-id="19b53-165">Int32</span></span>|<span data-ttu-id="19b53-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="19b53-166">Version of the device configuration.</span></span> <span data-ttu-id="19b53-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19b53-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19b53-168">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="19b53-168">trustedRootCertificate</span></span>|<span data-ttu-id="19b53-169">Binär</span><span class="sxs-lookup"><span data-stu-id="19b53-169">Binary</span></span>|<span data-ttu-id="19b53-170">Vertrauenswürdiges Zertifikat</span><span class="sxs-lookup"><span data-stu-id="19b53-170">Trusted Root Certificate</span></span>|
|<span data-ttu-id="19b53-171">Aus</span><span class="sxs-lookup"><span data-stu-id="19b53-171">certFileName</span></span>|<span data-ttu-id="19b53-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="19b53-172">String</span></span>|<span data-ttu-id="19b53-173">Der Dateiname in der Benutzeroberfläche angezeigt.</span><span class="sxs-lookup"><span data-stu-id="19b53-173">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="19b53-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="19b53-174">Response</span></span>
<span data-ttu-id="19b53-175">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="19b53-175">If successful, this method returns a `201 Created` response code and a [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19b53-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="19b53-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="19b53-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="19b53-177">Request</span></span>
<span data-ttu-id="19b53-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="19b53-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 438

{
  "@odata.type": "#microsoft.graph.windowsPhone81TrustedRootCertificate",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value"
}
```

### <a name="response"></a><span data-ttu-id="19b53-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="19b53-179">Response</span></span>
<span data-ttu-id="19b53-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="19b53-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 546

{
  "@odata.type": "#microsoft.graph.windowsPhone81TrustedRootCertificate",
  "id": "6316bf01-bf01-6316-01bf-166301bf1663",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value"
}
```





