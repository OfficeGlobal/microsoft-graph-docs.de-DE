---
title: Aktualisieren von „androidForWorkSettings“
description: Aktualisiert die Eigenschaften eines androidForWorkSettings-Objekts.
author: tfitzmac
ms.openlocfilehash: 5514de226d138291743c5b017a50682e91e1e9ce
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352542"
---
# <a name="update-androidforworksettings"></a><span data-ttu-id="16440-103">Aktualisieren von „androidForWorkSettings“</span><span class="sxs-lookup"><span data-stu-id="16440-103">Update androidForWorkSettings</span></span>

> <span data-ttu-id="16440-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="16440-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16440-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="16440-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="16440-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="16440-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16440-107">Aktualisiert die Eigenschaften eines [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="16440-107">Update the properties of a [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="16440-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="16440-108">Prerequisites</span></span>
<span data-ttu-id="16440-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16440-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16440-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="16440-111">Permission type</span></span>|<span data-ttu-id="16440-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="16440-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16440-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="16440-113">Delegated (work or school account)</span></span>|<span data-ttu-id="16440-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16440-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="16440-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="16440-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16440-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="16440-116">Not supported.</span></span>|
|<span data-ttu-id="16440-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="16440-117">Application</span></span>|<span data-ttu-id="16440-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="16440-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16440-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="16440-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkSettings
```

## <a name="request-headers"></a><span data-ttu-id="16440-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="16440-120">Request headers</span></span>
|<span data-ttu-id="16440-121">Header</span><span class="sxs-lookup"><span data-stu-id="16440-121">Header</span></span>|<span data-ttu-id="16440-122">Wert</span><span class="sxs-lookup"><span data-stu-id="16440-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16440-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="16440-123">Authorization</span></span>|<span data-ttu-id="16440-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="16440-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16440-125">Accept</span><span class="sxs-lookup"><span data-stu-id="16440-125">Accept</span></span>|<span data-ttu-id="16440-126">application/json</span><span class="sxs-lookup"><span data-stu-id="16440-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16440-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="16440-127">Request body</span></span>
<span data-ttu-id="16440-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="16440-128">In the request body, supply a JSON representation for the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

<span data-ttu-id="16440-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="16440-129">The following table shows the properties that are required when you create the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span></span>

|<span data-ttu-id="16440-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="16440-130">Property</span></span>|<span data-ttu-id="16440-131">Typ</span><span class="sxs-lookup"><span data-stu-id="16440-131">Type</span></span>|<span data-ttu-id="16440-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="16440-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16440-133">id</span><span class="sxs-lookup"><span data-stu-id="16440-133">id</span></span>|<span data-ttu-id="16440-134">String</span><span class="sxs-lookup"><span data-stu-id="16440-134">String</span></span>|<span data-ttu-id="16440-135">Android for Work-Einstellungsbezeichner.</span><span class="sxs-lookup"><span data-stu-id="16440-135">The Android for Work settings identifier</span></span>|
|<span data-ttu-id="16440-136">bindStatus</span><span class="sxs-lookup"><span data-stu-id="16440-136">bindStatus</span></span>|[<span data-ttu-id="16440-137">androidForWorkBindStatus</span><span class="sxs-lookup"><span data-stu-id="16440-137">androidForWorkBindStatus</span></span>](../resources/intune-androidforwork-androidforworkbindstatus.md)|<span data-ttu-id="16440-138">Status des Mandanten mit der Google EMM-API zu binden.</span><span class="sxs-lookup"><span data-stu-id="16440-138">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="16440-139">Mögliche Werte: sind `notBound`, `bound`, `boundAndValidated` und `unbinding`.</span><span class="sxs-lookup"><span data-stu-id="16440-139">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="16440-140">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="16440-140">lastAppSyncDateTime</span></span>|<span data-ttu-id="16440-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16440-141">DateTimeOffset</span></span>|<span data-ttu-id="16440-142">Zeitpunkt, zu dem zuletzt eine App-Synchronisierung abgeschlossen wurde.</span><span class="sxs-lookup"><span data-stu-id="16440-142">Last completion time for app sync</span></span>|
|<span data-ttu-id="16440-143">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="16440-143">lastAppSyncStatus</span></span>|[<span data-ttu-id="16440-144">androidForWorkSyncStatus</span><span class="sxs-lookup"><span data-stu-id="16440-144">androidForWorkSyncStatus</span></span>](../resources/intune-androidforwork-androidforworksyncstatus.md)|<span data-ttu-id="16440-145">Letzte Anwendung Sync Ergebnis.</span><span class="sxs-lookup"><span data-stu-id="16440-145">Last application sync result.</span></span> <span data-ttu-id="16440-146">Mögliche Werte sind: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError` und `none`.</span><span class="sxs-lookup"><span data-stu-id="16440-146">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="16440-147">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="16440-147">ownerUserPrincipalName</span></span>|<span data-ttu-id="16440-148">String</span><span class="sxs-lookup"><span data-stu-id="16440-148">String</span></span>|<span data-ttu-id="16440-149">Besitzer-UPN, der das Unternehmen erstellt hat</span><span class="sxs-lookup"><span data-stu-id="16440-149">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="16440-150">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="16440-150">ownerOrganizationName</span></span>|<span data-ttu-id="16440-151">String</span><span class="sxs-lookup"><span data-stu-id="16440-151">String</span></span>|<span data-ttu-id="16440-152">Organisationsname, der beim Android for Work-Onboarding verwendet wird</span><span class="sxs-lookup"><span data-stu-id="16440-152">Organization name used when onboarding Android for Work</span></span>|
|<span data-ttu-id="16440-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="16440-153">lastModifiedDateTime</span></span>|<span data-ttu-id="16440-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16440-154">DateTimeOffset</span></span>|<span data-ttu-id="16440-155">Zeitpunkt, zu dem die Android for Work-Einstellungen zuletzt geändert wurden</span><span class="sxs-lookup"><span data-stu-id="16440-155">Last modification time for Android for Work settings</span></span>|
|<span data-ttu-id="16440-156">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="16440-156">enrollmentTarget</span></span>|[<span data-ttu-id="16440-157">androidForWorkEnrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="16440-157">androidForWorkEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidforworkenrollmenttarget.md)|<span data-ttu-id="16440-158">Gibt an, welche Benutzer Geräte in Android für die Verwaltung von Geräten registrieren können.</span><span class="sxs-lookup"><span data-stu-id="16440-158">Indicates which users can enroll devices in Android for Work device management.</span></span> <span data-ttu-id="16440-159">Mögliche Werte: sind `none`, `all`, `targeted` und `targetedAsEnrollmentRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="16440-159">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="16440-160">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="16440-160">targetGroupIds</span></span>|<span data-ttu-id="16440-161">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="16440-161">String collection</span></span>|<span data-ttu-id="16440-162">Gibt an, welche AAD-Gruppen Geräte in der Android for Work-Geräteverwaltung registrieren dürfen, wenn die Eigenschaft „enrollmentTarget“ auf „Targeted“ gesetzt ist.</span><span class="sxs-lookup"><span data-stu-id="16440-162">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="16440-163">deviceOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="16440-163">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="16440-164">Boolesch</span><span class="sxs-lookup"><span data-stu-id="16440-164">Boolean</span></span>|<span data-ttu-id="16440-165">Gibt an, ob dieses Konto für Android Besitzer Gerätemanagement mit CloudDPC flighting ist.</span><span class="sxs-lookup"><span data-stu-id="16440-165">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|



## <a name="response"></a><span data-ttu-id="16440-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="16440-166">Response</span></span>
<span data-ttu-id="16440-167">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="16440-167">If successful, this method returns a `200 OK` response code and an updated [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16440-168">Beispiel</span><span class="sxs-lookup"><span data-stu-id="16440-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="16440-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="16440-169">Request</span></span>
<span data-ttu-id="16440-170">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="16440-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidForWorkSettings
Content-type: application/json
Content-length: 458

{
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ],
  "deviceOwnerManagementEnabled": true
}
```

### <a name="response"></a><span data-ttu-id="16440-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="16440-171">Response</span></span>
<span data-ttu-id="16440-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="16440-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 568

{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "id": "97adc169-c169-97ad-69c1-ad9769c1ad97",
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ],
  "deviceOwnerManagementEnabled": true
}
```





