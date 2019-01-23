---
title: ManagedEBookCategory aktualisieren
description: Aktualisieren Sie die Eigenschaften eines ManagedEBookCategory-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 832fb3f2ddc180a88a21d9484057332800e062a5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398331"
---
# <a name="update-managedebookcategory"></a><span data-ttu-id="0b21b-103">ManagedEBookCategory aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0b21b-103">Update managedEBookCategory</span></span>

> <span data-ttu-id="0b21b-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="0b21b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0b21b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0b21b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0b21b-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0b21b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b21b-107">Aktualisieren Sie die Eigenschaften eines [ManagedEBookCategory](../resources/intune-books-managedebookcategory.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0b21b-107">Update the properties of a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b21b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0b21b-108">Prerequisites</span></span>
<span data-ttu-id="0b21b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0b21b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0b21b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0b21b-111">Permission type</span></span>|<span data-ttu-id="0b21b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0b21b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b21b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0b21b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0b21b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b21b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0b21b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0b21b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b21b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0b21b-116">Not supported.</span></span>|
|<span data-ttu-id="0b21b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0b21b-117">Application</span></span>|<span data-ttu-id="0b21b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0b21b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b21b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0b21b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/categories/{managedEBookCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="0b21b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0b21b-120">Request headers</span></span>
|<span data-ttu-id="0b21b-121">Header</span><span class="sxs-lookup"><span data-stu-id="0b21b-121">Header</span></span>|<span data-ttu-id="0b21b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0b21b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b21b-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="0b21b-123">Authorization</span></span>|<span data-ttu-id="0b21b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0b21b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b21b-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0b21b-125">Accept</span></span>|<span data-ttu-id="0b21b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0b21b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b21b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0b21b-127">Request body</span></span>
<span data-ttu-id="0b21b-128">Geben Sie im Textkörper Anforderung für das Objekt [ManagedEBookCategory](../resources/intune-books-managedebookcategory.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="0b21b-128">In the request body, supply a JSON representation for the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

<span data-ttu-id="0b21b-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [ManagedEBookCategory](../resources/intune-books-managedebookcategory.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="0b21b-129">The following table shows the properties that are required when you create the [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span></span>

|<span data-ttu-id="0b21b-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0b21b-130">Property</span></span>|<span data-ttu-id="0b21b-131">Typ</span><span class="sxs-lookup"><span data-stu-id="0b21b-131">Type</span></span>|<span data-ttu-id="0b21b-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0b21b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b21b-133">id</span><span class="sxs-lookup"><span data-stu-id="0b21b-133">id</span></span>|<span data-ttu-id="0b21b-134">String</span><span class="sxs-lookup"><span data-stu-id="0b21b-134">String</span></span>|<span data-ttu-id="0b21b-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0b21b-135">The key of the entity.</span></span>|
|<span data-ttu-id="0b21b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0b21b-136">displayName</span></span>|<span data-ttu-id="0b21b-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0b21b-137">String</span></span>|<span data-ttu-id="0b21b-138">Der Name der Kategorie eBook.</span><span class="sxs-lookup"><span data-stu-id="0b21b-138">The name of the eBook category.</span></span>|
|<span data-ttu-id="0b21b-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0b21b-139">lastModifiedDateTime</span></span>|<span data-ttu-id="0b21b-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b21b-140">DateTimeOffset</span></span>|<span data-ttu-id="0b21b-141">Datum und Uhrzeit der letzten Änderung der ManagedEBookCategory.</span><span class="sxs-lookup"><span data-stu-id="0b21b-141">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="0b21b-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="0b21b-142">Response</span></span>
<span data-ttu-id="0b21b-143">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [ManagedEBookCategory](../resources/intune-books-managedebookcategory.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="0b21b-143">If successful, this method returns a `200 OK` response code and an updated [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b21b-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0b21b-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b21b-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0b21b-145">Request</span></span>
<span data-ttu-id="0b21b-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0b21b-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="0b21b-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="0b21b-147">Response</span></span>
<span data-ttu-id="0b21b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0b21b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 215

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "id": "3c71fb14-fb14-3c71-14fb-713c14fb713c",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




