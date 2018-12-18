---
title: targetedManagedAppConfiguration erstellen
description: Erstellen eines neuen targetedManagedAppConfiguration-Objekts.
author: tfitzmac
ms.openlocfilehash: 36183c117ecf3e8d6c48dbd3e92e02a16535dbc5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349035"
---
# <a name="create-targetedmanagedappconfiguration"></a><span data-ttu-id="c51f2-103">targetedManagedAppConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="c51f2-103">Create targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="c51f2-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c51f2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c51f2-105">Erstellen eines neuen [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c51f2-105">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c51f2-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c51f2-106">Prerequisites</span></span>
<span data-ttu-id="c51f2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c51f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c51f2-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c51f2-109">Permission type</span></span>|<span data-ttu-id="c51f2-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c51f2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c51f2-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c51f2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c51f2-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c51f2-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c51f2-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c51f2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c51f2-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c51f2-114">Not supported.</span></span>|
|<span data-ttu-id="c51f2-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c51f2-115">Application</span></span>|<span data-ttu-id="c51f2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c51f2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c51f2-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c51f2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c51f2-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c51f2-118">Request headers</span></span>
|<span data-ttu-id="c51f2-119">Header</span><span class="sxs-lookup"><span data-stu-id="c51f2-119">Header</span></span>|<span data-ttu-id="c51f2-120">Wert</span><span class="sxs-lookup"><span data-stu-id="c51f2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c51f2-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c51f2-121">Authorization</span></span>|<span data-ttu-id="c51f2-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c51f2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c51f2-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c51f2-123">Accept</span></span>|<span data-ttu-id="c51f2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c51f2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c51f2-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c51f2-125">Request body</span></span>
<span data-ttu-id="c51f2-126">Geben Sie im Anforderungstext eine JSON-Darstellung des targetedManagedAppConfiguration-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="c51f2-126">In the request body, supply a JSON representation for the targetedManagedAppConfiguration object.</span></span>

<span data-ttu-id="c51f2-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs targetedManagedAppConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="c51f2-127">The following table shows the properties that are required when you create the targetedManagedAppConfiguration.</span></span>

|<span data-ttu-id="c51f2-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c51f2-128">Property</span></span>|<span data-ttu-id="c51f2-129">Typ</span><span class="sxs-lookup"><span data-stu-id="c51f2-129">Type</span></span>|<span data-ttu-id="c51f2-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c51f2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c51f2-131">displayName</span><span class="sxs-lookup"><span data-stu-id="c51f2-131">displayName</span></span>|<span data-ttu-id="c51f2-132">String</span><span class="sxs-lookup"><span data-stu-id="c51f2-132">String</span></span>|<span data-ttu-id="c51f2-133">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="c51f2-133">Policy display name.</span></span> <span data-ttu-id="c51f2-134">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c51f2-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c51f2-135">description</span><span class="sxs-lookup"><span data-stu-id="c51f2-135">description</span></span>|<span data-ttu-id="c51f2-136">String</span><span class="sxs-lookup"><span data-stu-id="c51f2-136">String</span></span>|<span data-ttu-id="c51f2-137">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="c51f2-137">The policy's description.</span></span> <span data-ttu-id="c51f2-138">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c51f2-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c51f2-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c51f2-139">createdDateTime</span></span>|<span data-ttu-id="c51f2-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c51f2-140">DateTimeOffset</span></span>|<span data-ttu-id="c51f2-141">Datum und Uhrzeit der Erstellung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="c51f2-141">The date and time the policy was created.</span></span> <span data-ttu-id="c51f2-142">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c51f2-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c51f2-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c51f2-143">lastModifiedDateTime</span></span>|<span data-ttu-id="c51f2-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c51f2-144">DateTimeOffset</span></span>|<span data-ttu-id="c51f2-145">Datum und Uhrzeit der letzten Änderung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="c51f2-145">Last time the policy was modified.</span></span> <span data-ttu-id="c51f2-146">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c51f2-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c51f2-147">id</span><span class="sxs-lookup"><span data-stu-id="c51f2-147">id</span></span>|<span data-ttu-id="c51f2-148">String</span><span class="sxs-lookup"><span data-stu-id="c51f2-148">String</span></span>|<span data-ttu-id="c51f2-149">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c51f2-149">Key of the entity.</span></span> <span data-ttu-id="c51f2-150">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c51f2-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c51f2-151">Version</span><span class="sxs-lookup"><span data-stu-id="c51f2-151">version</span></span>|<span data-ttu-id="c51f2-152">String</span><span class="sxs-lookup"><span data-stu-id="c51f2-152">String</span></span>|<span data-ttu-id="c51f2-153">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="c51f2-153">Version of the entity.</span></span> <span data-ttu-id="c51f2-154">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c51f2-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c51f2-155">customSettings</span><span class="sxs-lookup"><span data-stu-id="c51f2-155">customSettings</span></span>|<span data-ttu-id="c51f2-156">[keyValuePair](../resources/intune-mam-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="c51f2-156">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="c51f2-157">Eine Gruppe von Paaren aus Schlüsselzeichenfolge und Wertzeichenfolge, die an Apps für Benutzer im Bereich der Konfiguration gesendet werden sollen, und zwar ohne Veränderungen durch den Dienst. Geerbt von [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c51f2-157">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="c51f2-158">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="c51f2-158">deployedAppCount</span></span>|<span data-ttu-id="c51f2-159">Int32</span><span class="sxs-lookup"><span data-stu-id="c51f2-159">Int32</span></span>|<span data-ttu-id="c51f2-160">Anzahl der Apps, für die die aktuelle Richtlinie bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="c51f2-160">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="c51f2-161">isAssigned</span><span class="sxs-lookup"><span data-stu-id="c51f2-161">isAssigned</span></span>|<span data-ttu-id="c51f2-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c51f2-162">Boolean</span></span>|<span data-ttu-id="c51f2-163">Gibt an, ob die Richtlinie für eine oder mehrere Einschlussgruppen bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="c51f2-163">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="c51f2-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="c51f2-164">Response</span></span>
<span data-ttu-id="c51f2-165">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c51f2-165">If successful, this method returns a `201 Created` response code and a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c51f2-166">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c51f2-166">Example</span></span>
### <a name="request"></a><span data-ttu-id="c51f2-167">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c51f2-167">Request</span></span>
<span data-ttu-id="c51f2-168">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c51f2-168">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations
Content-type: application/json
Content-length: 388

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="c51f2-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="c51f2-169">Response</span></span>
<span data-ttu-id="c51f2-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c51f2-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 560

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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



