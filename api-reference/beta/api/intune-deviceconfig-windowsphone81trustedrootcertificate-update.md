---
title: WindowsPhone81TrustedRootCertificate aktualisieren
description: Aktualisieren Sie die Eigenschaften eines windowsPhone81TrustedRootCertificate-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3dfd30e558fc043a4b0154b5b2a8bb913d19db86
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919141"
---
# <a name="update-windowsphone81trustedrootcertificate"></a><span data-ttu-id="f1290-103">WindowsPhone81TrustedRootCertificate aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f1290-103">Update windowsPhone81TrustedRootCertificate</span></span>

> <span data-ttu-id="f1290-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f1290-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f1290-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f1290-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f1290-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f1290-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1290-107">Aktualisieren Sie die Eigenschaften eines [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f1290-107">Update the properties of a [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f1290-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f1290-108">Prerequisites</span></span>
<span data-ttu-id="f1290-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1290-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1290-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f1290-111">Permission type</span></span>|<span data-ttu-id="f1290-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f1290-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1290-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f1290-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f1290-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1290-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f1290-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f1290-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1290-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f1290-116">Not supported.</span></span>|
|<span data-ttu-id="f1290-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f1290-117">Application</span></span>|<span data-ttu-id="f1290-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f1290-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1290-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f1290-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/rootCertificate
```

## <a name="request-headers"></a><span data-ttu-id="f1290-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f1290-120">Request headers</span></span>
|<span data-ttu-id="f1290-121">Header</span><span class="sxs-lookup"><span data-stu-id="f1290-121">Header</span></span>|<span data-ttu-id="f1290-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f1290-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1290-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1290-123">Authorization</span></span>|<span data-ttu-id="f1290-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f1290-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1290-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f1290-125">Accept</span></span>|<span data-ttu-id="f1290-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f1290-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1290-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f1290-127">Request body</span></span>
<span data-ttu-id="f1290-128">Geben Sie im Textkörper Anforderung für das Objekt [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="f1290-128">In the request body, supply a JSON representation for the [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object.</span></span>

<span data-ttu-id="f1290-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="f1290-129">The following table shows the properties that are required when you create the [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md).</span></span>

|<span data-ttu-id="f1290-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f1290-130">Property</span></span>|<span data-ttu-id="f1290-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f1290-131">Type</span></span>|<span data-ttu-id="f1290-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f1290-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1290-133">id</span><span class="sxs-lookup"><span data-stu-id="f1290-133">id</span></span>|<span data-ttu-id="f1290-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f1290-134">String</span></span>|<span data-ttu-id="f1290-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f1290-135">Key of the entity.</span></span> <span data-ttu-id="f1290-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1290-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1290-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f1290-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f1290-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1290-138">DateTimeOffset</span></span>|<span data-ttu-id="f1290-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f1290-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f1290-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1290-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1290-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f1290-141">roleScopeTagIds</span></span>|<span data-ttu-id="f1290-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="f1290-142">String collection</span></span>|<span data-ttu-id="f1290-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="f1290-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f1290-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1290-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1290-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f1290-145">supportsScopeTags</span></span>|<span data-ttu-id="f1290-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f1290-146">Boolean</span></span>|<span data-ttu-id="f1290-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f1290-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f1290-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="f1290-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f1290-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="f1290-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f1290-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f1290-150">This property is read-only.</span></span> <span data-ttu-id="f1290-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1290-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1290-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f1290-152">createdDateTime</span></span>|<span data-ttu-id="f1290-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1290-153">DateTimeOffset</span></span>|<span data-ttu-id="f1290-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f1290-154">DateTime the object was created.</span></span> <span data-ttu-id="f1290-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1290-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1290-156">description</span><span class="sxs-lookup"><span data-stu-id="f1290-156">description</span></span>|<span data-ttu-id="f1290-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f1290-157">String</span></span>|<span data-ttu-id="f1290-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f1290-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f1290-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1290-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1290-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f1290-160">displayName</span></span>|<span data-ttu-id="f1290-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f1290-161">String</span></span>|<span data-ttu-id="f1290-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f1290-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f1290-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1290-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1290-164">Version</span><span class="sxs-lookup"><span data-stu-id="f1290-164">version</span></span>|<span data-ttu-id="f1290-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f1290-165">Int32</span></span>|<span data-ttu-id="f1290-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="f1290-166">Version of the device configuration.</span></span> <span data-ttu-id="f1290-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1290-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1290-168">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="f1290-168">trustedRootCertificate</span></span>|<span data-ttu-id="f1290-169">Binär</span><span class="sxs-lookup"><span data-stu-id="f1290-169">Binary</span></span>|<span data-ttu-id="f1290-170">Vertrauenswürdiges Zertifikat</span><span class="sxs-lookup"><span data-stu-id="f1290-170">Trusted Root Certificate</span></span>|
|<span data-ttu-id="f1290-171">Aus</span><span class="sxs-lookup"><span data-stu-id="f1290-171">certFileName</span></span>|<span data-ttu-id="f1290-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f1290-172">String</span></span>|<span data-ttu-id="f1290-173">Der Dateiname in der Benutzeroberfläche angezeigt.</span><span class="sxs-lookup"><span data-stu-id="f1290-173">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="f1290-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="f1290-174">Response</span></span>
<span data-ttu-id="f1290-175">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f1290-175">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1290-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f1290-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="f1290-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f1290-177">Request</span></span>
<span data-ttu-id="f1290-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f1290-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/rootCertificate
Content-type: application/json
Content-length: 363

{
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

### <a name="response"></a><span data-ttu-id="f1290-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="f1290-179">Response</span></span>
<span data-ttu-id="f1290-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f1290-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





