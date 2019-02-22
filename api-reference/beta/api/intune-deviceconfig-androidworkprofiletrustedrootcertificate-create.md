---
title: AndroidWorkProfileTrustedRootCertificate erstellen
description: Erstellen eines neuen androidWorkProfileTrustedRootCertificate-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 18222441d62bee45ff7ce3be77236d719e1d69cf
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152927"
---
# <a name="create-androidworkprofiletrustedrootcertificate"></a><span data-ttu-id="7211b-103">AndroidWorkProfileTrustedRootCertificate erstellen</span><span class="sxs-lookup"><span data-stu-id="7211b-103">Create androidWorkProfileTrustedRootCertificate</span></span>

> <span data-ttu-id="7211b-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7211b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7211b-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7211b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7211b-106">Erstellen eines neuen [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="7211b-106">Create a new [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7211b-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7211b-107">Prerequisites</span></span>
<span data-ttu-id="7211b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7211b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7211b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7211b-110">Permission type</span></span>|<span data-ttu-id="7211b-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7211b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7211b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7211b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7211b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7211b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7211b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7211b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7211b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7211b-115">Not supported.</span></span>|
|<span data-ttu-id="7211b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7211b-116">Application</span></span>|<span data-ttu-id="7211b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7211b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7211b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7211b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7211b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7211b-119">Request headers</span></span>
|<span data-ttu-id="7211b-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7211b-120">Header</span></span>|<span data-ttu-id="7211b-121">Wert</span><span class="sxs-lookup"><span data-stu-id="7211b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7211b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7211b-122">Authorization</span></span>|<span data-ttu-id="7211b-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7211b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7211b-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7211b-124">Accept</span></span>|<span data-ttu-id="7211b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7211b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7211b-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7211b-126">Request body</span></span>
<span data-ttu-id="7211b-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das androidWorkProfileTrustedRootCertificate-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="7211b-127">In the request body, supply a JSON representation for the androidWorkProfileTrustedRootCertificate object.</span></span>

<span data-ttu-id="7211b-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der androidWorkProfileTrustedRootCertificate erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="7211b-128">The following table shows the properties that are required when you create the androidWorkProfileTrustedRootCertificate.</span></span>

|<span data-ttu-id="7211b-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7211b-129">Property</span></span>|<span data-ttu-id="7211b-130">Typ</span><span class="sxs-lookup"><span data-stu-id="7211b-130">Type</span></span>|<span data-ttu-id="7211b-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7211b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7211b-132">id</span><span class="sxs-lookup"><span data-stu-id="7211b-132">id</span></span>|<span data-ttu-id="7211b-133">string</span><span class="sxs-lookup"><span data-stu-id="7211b-133">String</span></span>|<span data-ttu-id="7211b-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="7211b-134">Key of the entity.</span></span> <span data-ttu-id="7211b-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7211b-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7211b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7211b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="7211b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7211b-137">DateTimeOffset</span></span>|<span data-ttu-id="7211b-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="7211b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="7211b-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7211b-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7211b-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="7211b-140">roleScopeTagIds</span></span>|<span data-ttu-id="7211b-141">String collection</span><span class="sxs-lookup"><span data-stu-id="7211b-141">String collection</span></span>|<span data-ttu-id="7211b-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="7211b-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7211b-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7211b-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7211b-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7211b-144">supportsScopeTags</span></span>|<span data-ttu-id="7211b-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7211b-145">Boolean</span></span>|<span data-ttu-id="7211b-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7211b-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7211b-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="7211b-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7211b-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="7211b-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7211b-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7211b-149">This property is read-only.</span></span> <span data-ttu-id="7211b-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7211b-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7211b-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7211b-151">createdDateTime</span></span>|<span data-ttu-id="7211b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7211b-152">DateTimeOffset</span></span>|<span data-ttu-id="7211b-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="7211b-153">DateTime the object was created.</span></span> <span data-ttu-id="7211b-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7211b-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7211b-155">description</span><span class="sxs-lookup"><span data-stu-id="7211b-155">description</span></span>|<span data-ttu-id="7211b-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7211b-156">String</span></span>|<span data-ttu-id="7211b-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="7211b-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7211b-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7211b-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7211b-159">displayName</span><span class="sxs-lookup"><span data-stu-id="7211b-159">displayName</span></span>|<span data-ttu-id="7211b-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7211b-160">String</span></span>|<span data-ttu-id="7211b-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="7211b-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7211b-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7211b-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7211b-163">Version</span><span class="sxs-lookup"><span data-stu-id="7211b-163">version</span></span>|<span data-ttu-id="7211b-164">Int32</span><span class="sxs-lookup"><span data-stu-id="7211b-164">Int32</span></span>|<span data-ttu-id="7211b-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="7211b-165">Version of the device configuration.</span></span> <span data-ttu-id="7211b-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7211b-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7211b-167">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="7211b-167">trustedRootCertificate</span></span>|<span data-ttu-id="7211b-168">Binär</span><span class="sxs-lookup"><span data-stu-id="7211b-168">Binary</span></span>|<span data-ttu-id="7211b-169">Vertrauenswürdiges Stammzertifikat</span><span class="sxs-lookup"><span data-stu-id="7211b-169">Trusted Root Certificate</span></span>|
|<span data-ttu-id="7211b-170">certFileName</span><span class="sxs-lookup"><span data-stu-id="7211b-170">certFileName</span></span>|<span data-ttu-id="7211b-171">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7211b-171">String</span></span>|<span data-ttu-id="7211b-172">Dateiname, der in der Benutzeroberfläche angezeigt werden soll.</span><span class="sxs-lookup"><span data-stu-id="7211b-172">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="7211b-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="7211b-173">Response</span></span>
<span data-ttu-id="7211b-174">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7211b-174">If successful, this method returns a `201 Created` response code and a [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7211b-175">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7211b-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="7211b-176">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7211b-176">Request</span></span>
<span data-ttu-id="7211b-177">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7211b-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 378

{
  "@odata.type": "#microsoft.graph.androidWorkProfileTrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="7211b-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="7211b-178">Response</span></span>
<span data-ttu-id="7211b-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7211b-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 550

{
  "@odata.type": "#microsoft.graph.androidWorkProfileTrustedRootCertificate",
  "id": "37cc7454-7454-37cc-5474-cc375474cc37",
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




