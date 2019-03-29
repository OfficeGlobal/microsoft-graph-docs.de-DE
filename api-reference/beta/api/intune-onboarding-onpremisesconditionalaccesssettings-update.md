---
title: onPremisesConditionalAccessSettings aktualisieren
description: Aktualisieren der Eigenschaften eines onPremisesConditionalAccessSettings-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7f3f493770185605ad8339d8aa354c82aec8b2d1
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30961847"
---
# <a name="update-onpremisesconditionalaccesssettings"></a><span data-ttu-id="314fd-103">onPremisesConditionalAccessSettings aktualisieren</span><span class="sxs-lookup"><span data-stu-id="314fd-103">Update onPremisesConditionalAccessSettings</span></span>

> <span data-ttu-id="314fd-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="314fd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="314fd-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="314fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="314fd-106">Aktualisieren der Eigenschaften eines [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="314fd-106">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="314fd-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="314fd-107">Prerequisites</span></span>
<span data-ttu-id="314fd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="314fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="314fd-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="314fd-110">Permission type</span></span>|<span data-ttu-id="314fd-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="314fd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="314fd-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="314fd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="314fd-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="314fd-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="314fd-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="314fd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="314fd-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="314fd-115">Not supported.</span></span>|
|<span data-ttu-id="314fd-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="314fd-116">Application</span></span>|<span data-ttu-id="314fd-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="314fd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="314fd-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="314fd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/conditionalAccessSettings
PATCH /deviceManagement/exchangeOnPremisesPolicy/conditionalAccessSettings
```

## <a name="request-headers"></a><span data-ttu-id="314fd-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="314fd-119">Request headers</span></span>
|<span data-ttu-id="314fd-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="314fd-120">Header</span></span>|<span data-ttu-id="314fd-121">Wert</span><span class="sxs-lookup"><span data-stu-id="314fd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="314fd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="314fd-122">Authorization</span></span>|<span data-ttu-id="314fd-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="314fd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="314fd-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="314fd-124">Accept</span></span>|<span data-ttu-id="314fd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="314fd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="314fd-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="314fd-126">Request body</span></span>
<span data-ttu-id="314fd-127">Geben Sie im Anforderungstext eine JSON-Darstellung des [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="314fd-127">In the request body, supply a JSON representation for the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

<span data-ttu-id="314fd-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="314fd-128">The following table shows the properties that are required when you create the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span></span>

|<span data-ttu-id="314fd-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="314fd-129">Property</span></span>|<span data-ttu-id="314fd-130">Typ</span><span class="sxs-lookup"><span data-stu-id="314fd-130">Type</span></span>|<span data-ttu-id="314fd-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="314fd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="314fd-132">id</span><span class="sxs-lookup"><span data-stu-id="314fd-132">id</span></span>|<span data-ttu-id="314fd-133">String</span><span class="sxs-lookup"><span data-stu-id="314fd-133">String</span></span>|<span data-ttu-id="314fd-134">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="314fd-134">Not yet documented</span></span>|
|<span data-ttu-id="314fd-135">aktiviert</span><span class="sxs-lookup"><span data-stu-id="314fd-135">enabled</span></span>|<span data-ttu-id="314fd-136">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="314fd-136">Boolean</span></span>|<span data-ttu-id="314fd-137">Gibt an, ob lokaler bedingter Zugriff für diese Organisation aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="314fd-137">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="314fd-138">includedGroups</span><span class="sxs-lookup"><span data-stu-id="314fd-138">includedGroups</span></span>|<span data-ttu-id="314fd-139">GUID-Sammlung</span><span class="sxs-lookup"><span data-stu-id="314fd-139">Guid collection</span></span>|<span data-ttu-id="314fd-140">Benutzergruppen, für die der lokale bedingte Zugriff gilt.</span><span class="sxs-lookup"><span data-stu-id="314fd-140">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="314fd-141">Alle Benutzer in diesen Gruppen müssen verwaltete und für den E-Mail-Zugriff kompatible Mobilgeräte verwenden.</span><span class="sxs-lookup"><span data-stu-id="314fd-141">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="314fd-142">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="314fd-142">excludedGroups</span></span>|<span data-ttu-id="314fd-143">GUID-Sammlung</span><span class="sxs-lookup"><span data-stu-id="314fd-143">Guid collection</span></span>|<span data-ttu-id="314fd-144">Benutzergruppen, die vom lokalen bedingten Zugriff ausgenommen werden.</span><span class="sxs-lookup"><span data-stu-id="314fd-144">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="314fd-145">Alle Benutzer in diesen Gruppen werden von der Richtlinie zu bedingtem Zugriff ausgenommen.</span><span class="sxs-lookup"><span data-stu-id="314fd-145">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="314fd-146">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="314fd-146">overrideDefaultRule</span></span>|<span data-ttu-id="314fd-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="314fd-147">Boolean</span></span>|<span data-ttu-id="314fd-148">Überschreibt die Standardzugriffsregel, wenn zugelassen wird, dass einem Gerät Zugriff gewährt wird.</span><span class="sxs-lookup"><span data-stu-id="314fd-148">Override the default access rule when allowing a device to ensure access is granted.</span></span>|



## <a name="response"></a><span data-ttu-id="314fd-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="314fd-149">Response</span></span>
<span data-ttu-id="314fd-150">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="314fd-150">If successful, this method returns a `200 OK` response code and an updated [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="314fd-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="314fd-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="314fd-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="314fd-152">Request</span></span>
<span data-ttu-id="314fd-153">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="314fd-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/conditionalAccessSettings
Content-type: application/json
Content-length: 275

{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "enabled": true,
  "includedGroups": [
    "77c9d466-d466-77c9-66d4-c97766d4c977"
  ],
  "excludedGroups": [
    "2a0afae4-fae4-2a0a-e4fa-0a2ae4fa0a2a"
  ],
  "overrideDefaultRule": true
}
```

### <a name="response"></a><span data-ttu-id="314fd-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="314fd-154">Response</span></span>
<span data-ttu-id="314fd-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="314fd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 324

{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "a0efde21-de21-a0ef-21de-efa021deefa0",
  "enabled": true,
  "includedGroups": [
    "77c9d466-d466-77c9-66d4-c97766d4c977"
  ],
  "excludedGroups": [
    "2a0afae4-fae4-2a0a-e4fa-0a2ae4fa0a2a"
  ],
  "overrideDefaultRule": true
}
```




