---
title: targetedManagedAppConfiguration erstellen
description: Erstellen eines neuen targetedManagedAppConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c95a6116a8d929623a0d48a58b6a4c2c410476b0
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970275"
---
# <a name="create-targetedmanagedappconfiguration"></a><span data-ttu-id="c5a65-103">targetedManagedAppConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="c5a65-103">Create targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="c5a65-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c5a65-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5a65-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c5a65-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5a65-106">Erstellen eines neuen [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c5a65-106">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5a65-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c5a65-107">Prerequisites</span></span>
<span data-ttu-id="c5a65-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5a65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5a65-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c5a65-110">Permission type</span></span>|<span data-ttu-id="c5a65-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c5a65-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5a65-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c5a65-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c5a65-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5a65-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c5a65-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c5a65-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5a65-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c5a65-115">Not supported.</span></span>|
|<span data-ttu-id="c5a65-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c5a65-116">Application</span></span>|<span data-ttu-id="c5a65-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c5a65-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5a65-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c5a65-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c5a65-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c5a65-119">Request headers</span></span>
|<span data-ttu-id="c5a65-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c5a65-120">Header</span></span>|<span data-ttu-id="c5a65-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c5a65-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5a65-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5a65-122">Authorization</span></span>|<span data-ttu-id="c5a65-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c5a65-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5a65-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c5a65-124">Accept</span></span>|<span data-ttu-id="c5a65-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c5a65-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5a65-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c5a65-126">Request body</span></span>
<span data-ttu-id="c5a65-127">Geben Sie im Anforderungstext eine JSON-Darstellung des targetedManagedAppConfiguration-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="c5a65-127">In the request body, supply a JSON representation for the targetedManagedAppConfiguration object.</span></span>

<span data-ttu-id="c5a65-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs targetedManagedAppConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="c5a65-128">The following table shows the properties that are required when you create the targetedManagedAppConfiguration.</span></span>

|<span data-ttu-id="c5a65-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c5a65-129">Property</span></span>|<span data-ttu-id="c5a65-130">Typ</span><span class="sxs-lookup"><span data-stu-id="c5a65-130">Type</span></span>|<span data-ttu-id="c5a65-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c5a65-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5a65-132">displayName</span><span class="sxs-lookup"><span data-stu-id="c5a65-132">displayName</span></span>|<span data-ttu-id="c5a65-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c5a65-133">String</span></span>|<span data-ttu-id="c5a65-134">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="c5a65-134">Policy display name.</span></span> <span data-ttu-id="c5a65-135">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c5a65-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c5a65-136">description</span><span class="sxs-lookup"><span data-stu-id="c5a65-136">description</span></span>|<span data-ttu-id="c5a65-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c5a65-137">String</span></span>|<span data-ttu-id="c5a65-138">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="c5a65-138">The policy's description.</span></span> <span data-ttu-id="c5a65-139">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c5a65-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c5a65-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c5a65-140">createdDateTime</span></span>|<span data-ttu-id="c5a65-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5a65-141">DateTimeOffset</span></span>|<span data-ttu-id="c5a65-142">Datum und Uhrzeit der Erstellung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="c5a65-142">The date and time the policy was created.</span></span> <span data-ttu-id="c5a65-143">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c5a65-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c5a65-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5a65-144">lastModifiedDateTime</span></span>|<span data-ttu-id="c5a65-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5a65-145">DateTimeOffset</span></span>|<span data-ttu-id="c5a65-146">Datum und Uhrzeit der letzten Änderung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="c5a65-146">Last time the policy was modified.</span></span> <span data-ttu-id="c5a65-147">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c5a65-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c5a65-148">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="c5a65-148">roleScopeTagIds</span></span>|<span data-ttu-id="c5a65-149">String collection</span><span class="sxs-lookup"><span data-stu-id="c5a65-149">String collection</span></span>|<span data-ttu-id="c5a65-150">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="c5a65-150">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c5a65-151">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c5a65-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c5a65-152">id</span><span class="sxs-lookup"><span data-stu-id="c5a65-152">id</span></span>|<span data-ttu-id="c5a65-153">String</span><span class="sxs-lookup"><span data-stu-id="c5a65-153">String</span></span>|<span data-ttu-id="c5a65-154">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c5a65-154">Key of the entity.</span></span> <span data-ttu-id="c5a65-155">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c5a65-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c5a65-156">Version</span><span class="sxs-lookup"><span data-stu-id="c5a65-156">version</span></span>|<span data-ttu-id="c5a65-157">String</span><span class="sxs-lookup"><span data-stu-id="c5a65-157">String</span></span>|<span data-ttu-id="c5a65-158">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="c5a65-158">Version of the entity.</span></span> <span data-ttu-id="c5a65-159">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c5a65-159">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c5a65-160">customSettings</span><span class="sxs-lookup"><span data-stu-id="c5a65-160">customSettings</span></span>|<span data-ttu-id="c5a65-161">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="c5a65-161">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="c5a65-162">Eine Gruppe von Paaren aus Schlüsselzeichenfolge und Wertzeichenfolge, die an Apps für Benutzer im Bereich der Konfiguration gesendet werden sollen, und zwar ohne Veränderungen durch den Dienst. Geerbt von [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5a65-162">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="c5a65-163">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="c5a65-163">deployedAppCount</span></span>|<span data-ttu-id="c5a65-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c5a65-164">Int32</span></span>|<span data-ttu-id="c5a65-165">Anzahl der Apps, für die die aktuelle Richtlinie bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="c5a65-165">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="c5a65-166">isAssigned</span><span class="sxs-lookup"><span data-stu-id="c5a65-166">isAssigned</span></span>|<span data-ttu-id="c5a65-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5a65-167">Boolean</span></span>|<span data-ttu-id="c5a65-168">Gibt an, ob die Richtlinie für eine oder mehrere Einschlussgruppen bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="c5a65-168">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="c5a65-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="c5a65-169">Response</span></span>
<span data-ttu-id="c5a65-170">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c5a65-170">If successful, this method returns a `201 Created` response code and a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5a65-171">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c5a65-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5a65-172">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c5a65-172">Request</span></span>
<span data-ttu-id="c5a65-173">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c5a65-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations
Content-type: application/json
Content-length: 450

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "version": "Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "isAssigned": true
}
```

### <a name="response"></a><span data-ttu-id="c5a65-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="c5a65-174">Response</span></span>
<span data-ttu-id="c5a65-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c5a65-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 622

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "2444e029-e029-2444-29e0-442429e04424",
  "version": "Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "isAssigned": true
}
```




