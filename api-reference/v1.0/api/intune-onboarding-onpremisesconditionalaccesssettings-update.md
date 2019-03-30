---
title: onPremisesConditionalAccessSettings aktualisieren
description: Aktualisieren der Eigenschaften eines onPremisesConditionalAccessSettings-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a4d72f4f4de4dfc3096b78665f9bf5c9953b2527
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30989008"
---
# <a name="update-onpremisesconditionalaccesssettings"></a><span data-ttu-id="08995-103">onPremisesConditionalAccessSettings aktualisieren</span><span class="sxs-lookup"><span data-stu-id="08995-103">Update onPremisesConditionalAccessSettings</span></span>

> <span data-ttu-id="08995-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="08995-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08995-105">Aktualisieren der Eigenschaften eines [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="08995-105">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08995-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="08995-106">Prerequisites</span></span>
<span data-ttu-id="08995-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08995-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08995-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="08995-109">Permission type</span></span>|<span data-ttu-id="08995-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="08995-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08995-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="08995-111">Delegated (work or school account)</span></span>|<span data-ttu-id="08995-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08995-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="08995-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="08995-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08995-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="08995-114">Not supported.</span></span>|
|<span data-ttu-id="08995-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="08995-115">Application</span></span>|<span data-ttu-id="08995-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="08995-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="08995-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="08995-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/conditionalAccessSettings
```

## <a name="request-headers"></a><span data-ttu-id="08995-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="08995-118">Request headers</span></span>
|<span data-ttu-id="08995-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="08995-119">Header</span></span>|<span data-ttu-id="08995-120">Wert</span><span class="sxs-lookup"><span data-stu-id="08995-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08995-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="08995-121">Authorization</span></span>|<span data-ttu-id="08995-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="08995-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08995-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="08995-123">Accept</span></span>|<span data-ttu-id="08995-124">application/json</span><span class="sxs-lookup"><span data-stu-id="08995-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08995-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="08995-125">Request body</span></span>
<span data-ttu-id="08995-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="08995-126">In the request body, supply a JSON representation for the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

<span data-ttu-id="08995-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="08995-127">The following table shows the properties that are required when you create the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span></span>

|<span data-ttu-id="08995-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="08995-128">Property</span></span>|<span data-ttu-id="08995-129">Typ</span><span class="sxs-lookup"><span data-stu-id="08995-129">Type</span></span>|<span data-ttu-id="08995-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08995-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08995-131">id</span><span class="sxs-lookup"><span data-stu-id="08995-131">id</span></span>|<span data-ttu-id="08995-132">String</span><span class="sxs-lookup"><span data-stu-id="08995-132">String</span></span>|<span data-ttu-id="08995-133">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="08995-133">Not yet documented</span></span>|
|<span data-ttu-id="08995-134">aktiviert</span><span class="sxs-lookup"><span data-stu-id="08995-134">enabled</span></span>|<span data-ttu-id="08995-135">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="08995-135">Boolean</span></span>|<span data-ttu-id="08995-136">Gibt an, ob lokaler bedingter Zugriff für diese Organisation aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="08995-136">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="08995-137">includedGroups</span><span class="sxs-lookup"><span data-stu-id="08995-137">includedGroups</span></span>|<span data-ttu-id="08995-138">GUID-Sammlung</span><span class="sxs-lookup"><span data-stu-id="08995-138">Guid collection</span></span>|<span data-ttu-id="08995-139">Benutzergruppen, für die der lokale bedingte Zugriff gilt.</span><span class="sxs-lookup"><span data-stu-id="08995-139">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="08995-140">Alle Benutzer in diesen Gruppen müssen verwaltete und für den E-Mail-Zugriff kompatible Mobilgeräte verwenden.</span><span class="sxs-lookup"><span data-stu-id="08995-140">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="08995-141">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="08995-141">excludedGroups</span></span>|<span data-ttu-id="08995-142">GUID-Sammlung</span><span class="sxs-lookup"><span data-stu-id="08995-142">Guid collection</span></span>|<span data-ttu-id="08995-143">Benutzergruppen, die vom lokalen bedingten Zugriff ausgenommen werden.</span><span class="sxs-lookup"><span data-stu-id="08995-143">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="08995-144">Alle Benutzer in diesen Gruppen werden von der Richtlinie zu bedingtem Zugriff ausgenommen.</span><span class="sxs-lookup"><span data-stu-id="08995-144">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="08995-145">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="08995-145">overrideDefaultRule</span></span>|<span data-ttu-id="08995-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="08995-146">Boolean</span></span>|<span data-ttu-id="08995-147">Überschreibt die Standardzugriffsregel, wenn zugelassen wird, dass einem Gerät Zugriff gewährt wird.</span><span class="sxs-lookup"><span data-stu-id="08995-147">Override the default access rule when allowing a device to ensure access is granted.</span></span>|



## <a name="response"></a><span data-ttu-id="08995-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="08995-148">Response</span></span>
<span data-ttu-id="08995-149">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="08995-149">If successful, this method returns a `200 OK` response code and an updated [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08995-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="08995-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="08995-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="08995-151">Request</span></span>
<span data-ttu-id="08995-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="08995-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/conditionalAccessSettings
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

### <a name="response"></a><span data-ttu-id="08995-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="08995-153">Response</span></span>
<span data-ttu-id="08995-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="08995-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



