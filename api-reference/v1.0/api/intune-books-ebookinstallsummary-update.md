---
title: eBookInstallSummary aktualisieren
description: Aktualisieren der Eigenschaften des eBookInstallSummary-Objekts.
ms.openlocfilehash: 261dd70883992b2aa1b2d480407969c1c887c421
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016301"
---
# <a name="update-ebookinstallsummary"></a><span data-ttu-id="15460-103">eBookInstallSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="15460-103">Update eBookInstallSummary</span></span>

> <span data-ttu-id="15460-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="15460-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15460-105">Aktualisieren der Eigenschaften des [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="15460-105">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="15460-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="15460-106">Prerequisites</span></span>
<span data-ttu-id="15460-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15460-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15460-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="15460-109">Permission type</span></span>|<span data-ttu-id="15460-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="15460-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15460-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="15460-111">Delegated (work or school account)</span></span>|<span data-ttu-id="15460-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15460-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="15460-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="15460-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15460-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="15460-114">Not supported.</span></span>|
|<span data-ttu-id="15460-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="15460-115">Application</span></span>|<span data-ttu-id="15460-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="15460-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15460-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="15460-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="15460-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="15460-118">Request headers</span></span>
|<span data-ttu-id="15460-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="15460-119">Header</span></span>|<span data-ttu-id="15460-120">Wert</span><span class="sxs-lookup"><span data-stu-id="15460-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15460-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="15460-121">Authorization</span></span>|<span data-ttu-id="15460-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="15460-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15460-123">Accept</span><span class="sxs-lookup"><span data-stu-id="15460-123">Accept</span></span>|<span data-ttu-id="15460-124">application/json</span><span class="sxs-lookup"><span data-stu-id="15460-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15460-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="15460-125">Request body</span></span>
<span data-ttu-id="15460-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="15460-126">In the request body, supply a JSON representation for the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

<span data-ttu-id="15460-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="15460-127">The following table shows the properties that are required when you create the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span></span>

|<span data-ttu-id="15460-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="15460-128">Property</span></span>|<span data-ttu-id="15460-129">Typ</span><span class="sxs-lookup"><span data-stu-id="15460-129">Type</span></span>|<span data-ttu-id="15460-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="15460-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15460-131">id</span><span class="sxs-lookup"><span data-stu-id="15460-131">id</span></span>|<span data-ttu-id="15460-132">String</span><span class="sxs-lookup"><span data-stu-id="15460-132">String</span></span>|<span data-ttu-id="15460-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="15460-133">Key of the entity.</span></span>|
|<span data-ttu-id="15460-134">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="15460-134">installedDeviceCount</span></span>|<span data-ttu-id="15460-135">Int32</span><span class="sxs-lookup"><span data-stu-id="15460-135">Int32</span></span>|<span data-ttu-id="15460-136">Die Anzahl der Geräte, auf denen das Buch erfolgreich installiert wurde.</span><span class="sxs-lookup"><span data-stu-id="15460-136">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="15460-137">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="15460-137">failedDeviceCount</span></span>|<span data-ttu-id="15460-138">Int32</span><span class="sxs-lookup"><span data-stu-id="15460-138">Int32</span></span>|<span data-ttu-id="15460-139">Die Anzahl der Geräte, auf denen die Installation des Buchs fehlgeschlagen ist.</span><span class="sxs-lookup"><span data-stu-id="15460-139">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="15460-140">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="15460-140">notInstalledDeviceCount</span></span>|<span data-ttu-id="15460-141">Int32</span><span class="sxs-lookup"><span data-stu-id="15460-141">Int32</span></span>|<span data-ttu-id="15460-142">Die Anzahl von Geräten, auf denen das Buch nicht installiert ist.</span><span class="sxs-lookup"><span data-stu-id="15460-142">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="15460-143">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="15460-143">installedUserCount</span></span>|<span data-ttu-id="15460-144">Int32</span><span class="sxs-lookup"><span data-stu-id="15460-144">Int32</span></span>|<span data-ttu-id="15460-145">Die Anzahl der Benutzer, deren Geräte das Buch erfolgreich installiert haben.</span><span class="sxs-lookup"><span data-stu-id="15460-145">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="15460-146">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="15460-146">failedUserCount</span></span>|<span data-ttu-id="15460-147">Int32</span><span class="sxs-lookup"><span data-stu-id="15460-147">Int32</span></span>|<span data-ttu-id="15460-148">Die Anzahl der Benutzer, die mindestens ein Gerät besitzen, auf dem die Installation des Buchs fehlgeschlagen ist.</span><span class="sxs-lookup"><span data-stu-id="15460-148">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="15460-149">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="15460-149">notInstalledUserCount</span></span>|<span data-ttu-id="15460-150">Int32</span><span class="sxs-lookup"><span data-stu-id="15460-150">Int32</span></span>|<span data-ttu-id="15460-151">Die Anzahl der Benutzer, die das Buch nicht installiert haben.</span><span class="sxs-lookup"><span data-stu-id="15460-151">Number of Users that did not install this book.</span></span>|



## <a name="response"></a><span data-ttu-id="15460-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="15460-152">Response</span></span>
<span data-ttu-id="15460-153">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="15460-153">If successful, this method returns a `200 OK` response code and an updated [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15460-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="15460-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="15460-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="15460-155">Request</span></span>
<span data-ttu-id="15460-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="15460-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
Content-type: application/json
Content-length: 236

{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```

### <a name="response"></a><span data-ttu-id="15460-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="15460-157">Response</span></span>
<span data-ttu-id="15460-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="15460-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "id": "9708ad78-ad78-9708-78ad-089778ad0897",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```



