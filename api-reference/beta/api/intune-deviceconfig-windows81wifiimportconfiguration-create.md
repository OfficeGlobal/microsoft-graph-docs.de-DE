---
title: Erstellen von windows81WifiImportConfiguration
description: Erstellen eines neuen windows81WifiImportConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5d39b658fcea9b761096ca87b12fc5ce7a9c269c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396462"
---
# <a name="create-windows81wifiimportconfiguration"></a><span data-ttu-id="aeafb-103">Erstellen von windows81WifiImportConfiguration</span><span class="sxs-lookup"><span data-stu-id="aeafb-103">Create windows81WifiImportConfiguration</span></span>

> <span data-ttu-id="aeafb-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="aeafb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="aeafb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="aeafb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aeafb-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="aeafb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aeafb-107">Erstellen eines neuen [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="aeafb-107">Create a new [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aeafb-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="aeafb-108">Prerequisites</span></span>
<span data-ttu-id="aeafb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="aeafb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="aeafb-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="aeafb-111">Permission type</span></span>|<span data-ttu-id="aeafb-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="aeafb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aeafb-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="aeafb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aeafb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aeafb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aeafb-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="aeafb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aeafb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aeafb-116">Not supported.</span></span>|
|<span data-ttu-id="aeafb-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="aeafb-117">Application</span></span>|<span data-ttu-id="aeafb-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aeafb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aeafb-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aeafb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="aeafb-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="aeafb-120">Request headers</span></span>
|<span data-ttu-id="aeafb-121">Header</span><span class="sxs-lookup"><span data-stu-id="aeafb-121">Header</span></span>|<span data-ttu-id="aeafb-122">Wert</span><span class="sxs-lookup"><span data-stu-id="aeafb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aeafb-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="aeafb-123">Authorization</span></span>|<span data-ttu-id="aeafb-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="aeafb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aeafb-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="aeafb-125">Accept</span></span>|<span data-ttu-id="aeafb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aeafb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aeafb-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="aeafb-127">Request body</span></span>
<span data-ttu-id="aeafb-128">Geben Sie im Textkörper Anforderung für das Objekt windows81WifiImportConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="aeafb-128">In the request body, supply a JSON representation for the windows81WifiImportConfiguration object.</span></span>

<span data-ttu-id="aeafb-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die windows81WifiImportConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="aeafb-129">The following table shows the properties that are required when you create the windows81WifiImportConfiguration.</span></span>

|<span data-ttu-id="aeafb-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="aeafb-130">Property</span></span>|<span data-ttu-id="aeafb-131">Typ</span><span class="sxs-lookup"><span data-stu-id="aeafb-131">Type</span></span>|<span data-ttu-id="aeafb-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aeafb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aeafb-133">id</span><span class="sxs-lookup"><span data-stu-id="aeafb-133">id</span></span>|<span data-ttu-id="aeafb-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="aeafb-134">String</span></span>|<span data-ttu-id="aeafb-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="aeafb-135">Key of the entity.</span></span> <span data-ttu-id="aeafb-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aeafb-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aeafb-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aeafb-137">lastModifiedDateTime</span></span>|<span data-ttu-id="aeafb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aeafb-138">DateTimeOffset</span></span>|<span data-ttu-id="aeafb-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="aeafb-139">DateTime the object was last modified.</span></span> <span data-ttu-id="aeafb-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aeafb-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aeafb-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="aeafb-141">roleScopeTagIds</span></span>|<span data-ttu-id="aeafb-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="aeafb-142">String collection</span></span>|<span data-ttu-id="aeafb-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="aeafb-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="aeafb-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aeafb-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aeafb-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="aeafb-145">supportsScopeTags</span></span>|<span data-ttu-id="aeafb-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="aeafb-146">Boolean</span></span>|<span data-ttu-id="aeafb-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="aeafb-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="aeafb-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="aeafb-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="aeafb-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="aeafb-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="aeafb-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="aeafb-150">This property is read-only.</span></span> <span data-ttu-id="aeafb-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aeafb-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aeafb-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aeafb-152">createdDateTime</span></span>|<span data-ttu-id="aeafb-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aeafb-153">DateTimeOffset</span></span>|<span data-ttu-id="aeafb-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="aeafb-154">DateTime the object was created.</span></span> <span data-ttu-id="aeafb-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aeafb-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aeafb-156">description</span><span class="sxs-lookup"><span data-stu-id="aeafb-156">description</span></span>|<span data-ttu-id="aeafb-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="aeafb-157">String</span></span>|<span data-ttu-id="aeafb-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="aeafb-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="aeafb-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aeafb-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aeafb-160">displayName</span><span class="sxs-lookup"><span data-stu-id="aeafb-160">displayName</span></span>|<span data-ttu-id="aeafb-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="aeafb-161">String</span></span>|<span data-ttu-id="aeafb-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="aeafb-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="aeafb-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aeafb-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aeafb-164">Version</span><span class="sxs-lookup"><span data-stu-id="aeafb-164">version</span></span>|<span data-ttu-id="aeafb-165">Int32</span><span class="sxs-lookup"><span data-stu-id="aeafb-165">Int32</span></span>|<span data-ttu-id="aeafb-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="aeafb-166">Version of the device configuration.</span></span> <span data-ttu-id="aeafb-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aeafb-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aeafb-168">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="aeafb-168">payloadFileName</span></span>|<span data-ttu-id="aeafb-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="aeafb-169">String</span></span>|<span data-ttu-id="aeafb-170">Name der Nutzlast (\*.XML).</span><span class="sxs-lookup"><span data-stu-id="aeafb-170">Payload file name (\*.xml).</span></span>|
|<span data-ttu-id="aeafb-171">Profilname</span><span class="sxs-lookup"><span data-stu-id="aeafb-171">profileName</span></span>|<span data-ttu-id="aeafb-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="aeafb-172">String</span></span>|<span data-ttu-id="aeafb-173">Name der Benutzerprofildienst in der Benutzeroberfläche angezeigt.</span><span class="sxs-lookup"><span data-stu-id="aeafb-173">Profile name displayed in the UI.</span></span>|
|<span data-ttu-id="aeafb-174">payload</span><span class="sxs-lookup"><span data-stu-id="aeafb-174">payload</span></span>|<span data-ttu-id="aeafb-175">Binär</span><span class="sxs-lookup"><span data-stu-id="aeafb-175">Binary</span></span>|<span data-ttu-id="aeafb-176">Nutzlast</span><span class="sxs-lookup"><span data-stu-id="aeafb-176">Payload.</span></span> <span data-ttu-id="aeafb-177">(UTF8 codiert Byte-Array).</span><span class="sxs-lookup"><span data-stu-id="aeafb-177">(UTF8 encoded byte array).</span></span> <span data-ttu-id="aeafb-178">Dies ist der XML-Datei gespeichert haben, auf dem Gerät, die, das Sie an den Endpunkt Wi-Fi-Verbindung verwendet.</span><span class="sxs-lookup"><span data-stu-id="aeafb-178">This is the XML file saved on the device you used to connect to the Wi-Fi endpoint.</span></span>|



## <a name="response"></a><span data-ttu-id="aeafb-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="aeafb-179">Response</span></span>
<span data-ttu-id="aeafb-180">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="aeafb-180">If successful, this method returns a `201 Created` response code and a [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aeafb-181">Beispiel</span><span class="sxs-lookup"><span data-stu-id="aeafb-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="aeafb-182">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aeafb-182">Request</span></span>
<span data-ttu-id="aeafb-183">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="aeafb-183">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 381

{
  "@odata.type": "#microsoft.graph.windows81WifiImportConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadFileName": "Payload File Name value",
  "profileName": "Profile Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="aeafb-184">Antwort</span><span class="sxs-lookup"><span data-stu-id="aeafb-184">Response</span></span>
<span data-ttu-id="aeafb-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aeafb-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 553

{
  "@odata.type": "#microsoft.graph.windows81WifiImportConfiguration",
  "id": "534a2f07-2f07-534a-072f-4a53072f4a53",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadFileName": "Payload File Name value",
  "profileName": "Profile Name value",
  "payload": "cGF5bG9hZA=="
}
```




