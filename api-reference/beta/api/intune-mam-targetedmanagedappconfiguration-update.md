---
title: targetedManagedAppConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines targetedManagedAppConfiguration- Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4842d48a41d51a9e9d2e2edaf1b2681c0c0b515e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30968854"
---
# <a name="update-targetedmanagedappconfiguration"></a><span data-ttu-id="fa5a8-103">targetedManagedAppConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="fa5a8-103">Update targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="fa5a8-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fa5a8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa5a8-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="fa5a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa5a8-106">Aktualisieren der Eigenschaften eines [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)- Objekts.</span><span class="sxs-lookup"><span data-stu-id="fa5a8-106">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa5a8-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fa5a8-107">Prerequisites</span></span>
<span data-ttu-id="fa5a8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa5a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa5a8-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fa5a8-110">Permission type</span></span>|<span data-ttu-id="fa5a8-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fa5a8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa5a8-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fa5a8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fa5a8-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa5a8-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fa5a8-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fa5a8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa5a8-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fa5a8-115">Not supported.</span></span>|
|<span data-ttu-id="fa5a8-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fa5a8-116">Application</span></span>|<span data-ttu-id="fa5a8-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fa5a8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa5a8-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa5a8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="fa5a8-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fa5a8-119">Request headers</span></span>
|<span data-ttu-id="fa5a8-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="fa5a8-120">Header</span></span>|<span data-ttu-id="fa5a8-121">Wert</span><span class="sxs-lookup"><span data-stu-id="fa5a8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa5a8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa5a8-122">Authorization</span></span>|<span data-ttu-id="fa5a8-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fa5a8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa5a8-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fa5a8-124">Accept</span></span>|<span data-ttu-id="fa5a8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fa5a8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa5a8-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fa5a8-126">Request body</span></span>
<span data-ttu-id="fa5a8-127">Geben Sie im Anforderungstext eine JSON-Darstellung des [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="fa5a8-127">In the request body, supply a JSON representation for the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

<span data-ttu-id="fa5a8-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="fa5a8-128">The following table shows the properties that are required when you create the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>

|<span data-ttu-id="fa5a8-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fa5a8-129">Property</span></span>|<span data-ttu-id="fa5a8-130">Typ</span><span class="sxs-lookup"><span data-stu-id="fa5a8-130">Type</span></span>|<span data-ttu-id="fa5a8-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fa5a8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa5a8-132">displayName</span><span class="sxs-lookup"><span data-stu-id="fa5a8-132">displayName</span></span>|<span data-ttu-id="fa5a8-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa5a8-133">String</span></span>|<span data-ttu-id="fa5a8-134">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="fa5a8-134">Policy display name.</span></span> <span data-ttu-id="fa5a8-135">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fa5a8-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fa5a8-136">description</span><span class="sxs-lookup"><span data-stu-id="fa5a8-136">description</span></span>|<span data-ttu-id="fa5a8-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa5a8-137">String</span></span>|<span data-ttu-id="fa5a8-138">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="fa5a8-138">The policy's description.</span></span> <span data-ttu-id="fa5a8-139">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fa5a8-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fa5a8-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fa5a8-140">createdDateTime</span></span>|<span data-ttu-id="fa5a8-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa5a8-141">DateTimeOffset</span></span>|<span data-ttu-id="fa5a8-142">Datum und Uhrzeit der Erstellung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="fa5a8-142">The date and time the policy was created.</span></span> <span data-ttu-id="fa5a8-143">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fa5a8-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fa5a8-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fa5a8-144">lastModifiedDateTime</span></span>|<span data-ttu-id="fa5a8-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa5a8-145">DateTimeOffset</span></span>|<span data-ttu-id="fa5a8-146">Datum und Uhrzeit der letzten Änderung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="fa5a8-146">Last time the policy was modified.</span></span> <span data-ttu-id="fa5a8-147">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fa5a8-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fa5a8-148">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="fa5a8-148">roleScopeTagIds</span></span>|<span data-ttu-id="fa5a8-149">String collection</span><span class="sxs-lookup"><span data-stu-id="fa5a8-149">String collection</span></span>|<span data-ttu-id="fa5a8-150">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="fa5a8-150">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fa5a8-151">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fa5a8-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fa5a8-152">id</span><span class="sxs-lookup"><span data-stu-id="fa5a8-152">id</span></span>|<span data-ttu-id="fa5a8-153">String</span><span class="sxs-lookup"><span data-stu-id="fa5a8-153">String</span></span>|<span data-ttu-id="fa5a8-154">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="fa5a8-154">Key of the entity.</span></span> <span data-ttu-id="fa5a8-155">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fa5a8-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fa5a8-156">Version</span><span class="sxs-lookup"><span data-stu-id="fa5a8-156">version</span></span>|<span data-ttu-id="fa5a8-157">String</span><span class="sxs-lookup"><span data-stu-id="fa5a8-157">String</span></span>|<span data-ttu-id="fa5a8-158">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="fa5a8-158">Version of the entity.</span></span> <span data-ttu-id="fa5a8-159">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fa5a8-159">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fa5a8-160">customSettings</span><span class="sxs-lookup"><span data-stu-id="fa5a8-160">customSettings</span></span>|<span data-ttu-id="fa5a8-161">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="fa5a8-161">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="fa5a8-162">Eine Gruppe von Paaren aus Schlüsselzeichenfolge und Wertzeichenfolge, die an Apps für Benutzer im Bereich der Konfiguration gesendet werden sollen, und zwar ohne Veränderungen durch den Dienst. Geerbt von [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa5a8-162">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="fa5a8-163">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="fa5a8-163">deployedAppCount</span></span>|<span data-ttu-id="fa5a8-164">Int32</span><span class="sxs-lookup"><span data-stu-id="fa5a8-164">Int32</span></span>|<span data-ttu-id="fa5a8-165">Anzahl der Apps, für die die aktuelle Richtlinie bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="fa5a8-165">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="fa5a8-166">isAssigned</span><span class="sxs-lookup"><span data-stu-id="fa5a8-166">isAssigned</span></span>|<span data-ttu-id="fa5a8-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa5a8-167">Boolean</span></span>|<span data-ttu-id="fa5a8-168">Gibt an, ob die Richtlinie für eine oder mehrere Einschlussgruppen bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="fa5a8-168">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="fa5a8-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa5a8-169">Response</span></span>
<span data-ttu-id="fa5a8-170">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fa5a8-170">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa5a8-171">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fa5a8-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa5a8-172">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa5a8-172">Request</span></span>
<span data-ttu-id="fa5a8-173">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fa5a8-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
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

### <a name="response"></a><span data-ttu-id="fa5a8-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa5a8-174">Response</span></span>
<span data-ttu-id="fa5a8-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fa5a8-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




