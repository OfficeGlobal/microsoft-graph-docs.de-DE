---
title: eBookInstallSummary aktualisieren
description: Aktualisieren der Eigenschaften des eBookInstallSummary-Objekts.
ms.openlocfilehash: a3484eed0a52278616039b7cc5e2427f4a0e1510
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065999"
---
# <a name="update-ebookinstallsummary"></a><span data-ttu-id="32630-103">eBookInstallSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="32630-103">Update eBookInstallSummary</span></span>

> <span data-ttu-id="32630-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="32630-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="32630-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="32630-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="32630-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="32630-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="32630-107">Aktualisieren der Eigenschaften des [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="32630-107">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="32630-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="32630-108">Prerequisites</span></span>
<span data-ttu-id="32630-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32630-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32630-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="32630-111">Permission type</span></span>|<span data-ttu-id="32630-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="32630-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32630-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="32630-113">Delegated (work or school account)</span></span>|<span data-ttu-id="32630-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32630-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="32630-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="32630-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32630-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="32630-116">Not supported.</span></span>|
|<span data-ttu-id="32630-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="32630-117">Application</span></span>|<span data-ttu-id="32630-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="32630-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32630-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="32630-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="32630-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="32630-120">Request headers</span></span>
|<span data-ttu-id="32630-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="32630-121">Header</span></span>|<span data-ttu-id="32630-122">Wert</span><span class="sxs-lookup"><span data-stu-id="32630-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32630-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="32630-123">Authorization</span></span>|<span data-ttu-id="32630-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="32630-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32630-125">Accept</span><span class="sxs-lookup"><span data-stu-id="32630-125">Accept</span></span>|<span data-ttu-id="32630-126">application/json</span><span class="sxs-lookup"><span data-stu-id="32630-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32630-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="32630-127">Request body</span></span>
<span data-ttu-id="32630-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="32630-128">In the request body, supply a JSON representation for the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

<span data-ttu-id="32630-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="32630-129">The following table shows the properties that are required when you create the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span></span>

|<span data-ttu-id="32630-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="32630-130">Property</span></span>|<span data-ttu-id="32630-131">Typ</span><span class="sxs-lookup"><span data-stu-id="32630-131">Type</span></span>|<span data-ttu-id="32630-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="32630-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32630-133">id</span><span class="sxs-lookup"><span data-stu-id="32630-133">id</span></span>|<span data-ttu-id="32630-134">String</span><span class="sxs-lookup"><span data-stu-id="32630-134">String</span></span>|<span data-ttu-id="32630-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="32630-135">Key of the entity.</span></span>|
|<span data-ttu-id="32630-136">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="32630-136">installedDeviceCount</span></span>|<span data-ttu-id="32630-137">Int32</span><span class="sxs-lookup"><span data-stu-id="32630-137">Int32</span></span>|<span data-ttu-id="32630-138">Die Anzahl der Geräte, auf denen das Buch erfolgreich installiert wurde.</span><span class="sxs-lookup"><span data-stu-id="32630-138">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="32630-139">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="32630-139">failedDeviceCount</span></span>|<span data-ttu-id="32630-140">Int32</span><span class="sxs-lookup"><span data-stu-id="32630-140">Int32</span></span>|<span data-ttu-id="32630-141">Die Anzahl der Geräte, auf denen die Installation des Buchs fehlgeschlagen ist.</span><span class="sxs-lookup"><span data-stu-id="32630-141">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="32630-142">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="32630-142">notInstalledDeviceCount</span></span>|<span data-ttu-id="32630-143">Int32</span><span class="sxs-lookup"><span data-stu-id="32630-143">Int32</span></span>|<span data-ttu-id="32630-144">Die Anzahl von Geräten, auf denen das Buch nicht installiert ist.</span><span class="sxs-lookup"><span data-stu-id="32630-144">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="32630-145">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="32630-145">installedUserCount</span></span>|<span data-ttu-id="32630-146">Int32</span><span class="sxs-lookup"><span data-stu-id="32630-146">Int32</span></span>|<span data-ttu-id="32630-147">Die Anzahl der Benutzer, deren Geräte das Buch erfolgreich installiert haben.</span><span class="sxs-lookup"><span data-stu-id="32630-147">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="32630-148">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="32630-148">failedUserCount</span></span>|<span data-ttu-id="32630-149">Int32</span><span class="sxs-lookup"><span data-stu-id="32630-149">Int32</span></span>|<span data-ttu-id="32630-150">Die Anzahl der Benutzer, die mindestens ein Gerät besitzen, auf dem die Installation des Buchs fehlgeschlagen ist.</span><span class="sxs-lookup"><span data-stu-id="32630-150">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="32630-151">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="32630-151">notInstalledUserCount</span></span>|<span data-ttu-id="32630-152">Int32</span><span class="sxs-lookup"><span data-stu-id="32630-152">Int32</span></span>|<span data-ttu-id="32630-153">Die Anzahl der Benutzer, die das Buch nicht installiert haben.</span><span class="sxs-lookup"><span data-stu-id="32630-153">Number of Users that did not install this book.</span></span>|



## <a name="response"></a><span data-ttu-id="32630-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="32630-154">Response</span></span>
<span data-ttu-id="32630-155">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="32630-155">If successful, this method returns a `200 OK` response code and an updated [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32630-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="32630-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="32630-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="32630-157">Request</span></span>
<span data-ttu-id="32630-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="32630-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
Content-type: application/json
Content-length: 178

{
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```

### <a name="response"></a><span data-ttu-id="32630-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="32630-159">Response</span></span>
<span data-ttu-id="32630-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="32630-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





