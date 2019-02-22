---
title: managedEBook-Ressourcentyp
description: Eine abstrakte Klasse, die die grundlegenden Eigenschaften des verwalteten eBooks enthält
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 24a8619d92eee6c666b7126a84895b14e0404755
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156035"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="444cf-103">managedEBook-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="444cf-103">managedEBook resource type</span></span>

> <span data-ttu-id="444cf-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="444cf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="444cf-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="444cf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="444cf-106">Eine abstrakte Klasse, die die grundlegenden Eigenschaften des verwalteten eBooks enthält</span><span class="sxs-lookup"><span data-stu-id="444cf-106">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="444cf-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="444cf-107">Methods</span></span>
|<span data-ttu-id="444cf-108">Methode</span><span class="sxs-lookup"><span data-stu-id="444cf-108">Method</span></span>|<span data-ttu-id="444cf-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="444cf-109">Return Type</span></span>|<span data-ttu-id="444cf-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="444cf-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="444cf-111">managedEBooks auflisten</span><span class="sxs-lookup"><span data-stu-id="444cf-111">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="444cf-112">[managedEBook](../resources/intune-books-managedebook.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="444cf-112">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="444cf-113">Auflisten von Eigenschaften und Beziehungen der [managedEBook](../resources/intune-books-managedebook.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="444cf-113">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="444cf-114">managedEBook abrufen</span><span class="sxs-lookup"><span data-stu-id="444cf-114">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="444cf-115">managedEBook</span><span class="sxs-lookup"><span data-stu-id="444cf-115">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="444cf-116">Lesen von Eigenschaften und Beziehungen des [managedEBook](../resources/intune-books-managedebook.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="444cf-116">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="444cf-117">Aktion zuweisen</span><span class="sxs-lookup"><span data-stu-id="444cf-117">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="444cf-118">Keine</span><span class="sxs-lookup"><span data-stu-id="444cf-118">None</span></span>|<span data-ttu-id="444cf-119">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="444cf-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="444cf-120">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="444cf-120">Properties</span></span>
|<span data-ttu-id="444cf-121">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="444cf-121">Property</span></span>|<span data-ttu-id="444cf-122">Typ</span><span class="sxs-lookup"><span data-stu-id="444cf-122">Type</span></span>|<span data-ttu-id="444cf-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="444cf-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="444cf-124">id</span><span class="sxs-lookup"><span data-stu-id="444cf-124">id</span></span>|<span data-ttu-id="444cf-125">string</span><span class="sxs-lookup"><span data-stu-id="444cf-125">String</span></span>|<span data-ttu-id="444cf-126">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="444cf-126">Key of the entity.</span></span>|
|<span data-ttu-id="444cf-127">displayName</span><span class="sxs-lookup"><span data-stu-id="444cf-127">displayName</span></span>|<span data-ttu-id="444cf-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="444cf-128">String</span></span>|<span data-ttu-id="444cf-129">Name des E-Books</span><span class="sxs-lookup"><span data-stu-id="444cf-129">Name of the eBook.</span></span>|
|<span data-ttu-id="444cf-130">description</span><span class="sxs-lookup"><span data-stu-id="444cf-130">description</span></span>|<span data-ttu-id="444cf-131">String</span><span class="sxs-lookup"><span data-stu-id="444cf-131">String</span></span>|<span data-ttu-id="444cf-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="444cf-132">Description.</span></span>|
|<span data-ttu-id="444cf-133">publisher</span><span class="sxs-lookup"><span data-stu-id="444cf-133">publisher</span></span>|<span data-ttu-id="444cf-134">String</span><span class="sxs-lookup"><span data-stu-id="444cf-134">String</span></span>|<span data-ttu-id="444cf-135">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="444cf-135">Publisher.</span></span>|
|<span data-ttu-id="444cf-136">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="444cf-136">publishedDateTime</span></span>|<span data-ttu-id="444cf-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="444cf-137">DateTimeOffset</span></span>|<span data-ttu-id="444cf-138">Datum und Uhrzeit der Veröffentlichung des E-Books.</span><span class="sxs-lookup"><span data-stu-id="444cf-138">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="444cf-139">largeCover</span><span class="sxs-lookup"><span data-stu-id="444cf-139">largeCover</span></span>|[<span data-ttu-id="444cf-140">mimeContent</span><span class="sxs-lookup"><span data-stu-id="444cf-140">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="444cf-141">Umschlagbild des Buchs</span><span class="sxs-lookup"><span data-stu-id="444cf-141">Book cover.</span></span>|
|<span data-ttu-id="444cf-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="444cf-142">createdDateTime</span></span>|<span data-ttu-id="444cf-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="444cf-143">DateTimeOffset</span></span>|<span data-ttu-id="444cf-144">Datum und Uhrzeit der Erstellung der E-Book-Datei.</span><span class="sxs-lookup"><span data-stu-id="444cf-144">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="444cf-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="444cf-145">lastModifiedDateTime</span></span>|<span data-ttu-id="444cf-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="444cf-146">DateTimeOffset</span></span>|<span data-ttu-id="444cf-147">Datum und Uhrzeit der letzten Änderung des E-Books.</span><span class="sxs-lookup"><span data-stu-id="444cf-147">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="444cf-148">informationUrl</span><span class="sxs-lookup"><span data-stu-id="444cf-148">informationUrl</span></span>|<span data-ttu-id="444cf-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="444cf-149">String</span></span>|<span data-ttu-id="444cf-150">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="444cf-150">The more information Url.</span></span>|
|<span data-ttu-id="444cf-151">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="444cf-151">privacyInformationUrl</span></span>|<span data-ttu-id="444cf-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="444cf-152">String</span></span>|<span data-ttu-id="444cf-153">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="444cf-153">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="444cf-154">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="444cf-154">Relationships</span></span>
|<span data-ttu-id="444cf-155">Beziehung</span><span class="sxs-lookup"><span data-stu-id="444cf-155">Relationship</span></span>|<span data-ttu-id="444cf-156">Typ</span><span class="sxs-lookup"><span data-stu-id="444cf-156">Type</span></span>|<span data-ttu-id="444cf-157">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="444cf-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="444cf-158">categories</span><span class="sxs-lookup"><span data-stu-id="444cf-158">categories</span></span>|<span data-ttu-id="444cf-159">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="444cf-159">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="444cf-160">Die Liste der Kategorien für dieses eBook.</span><span class="sxs-lookup"><span data-stu-id="444cf-160">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="444cf-161">assignments</span><span class="sxs-lookup"><span data-stu-id="444cf-161">assignments</span></span>|<span data-ttu-id="444cf-162">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="444cf-162">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="444cf-163">Die Liste der Zuweisungen für dieses E-Book.</span><span class="sxs-lookup"><span data-stu-id="444cf-163">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="444cf-164">installSummary</span><span class="sxs-lookup"><span data-stu-id="444cf-164">installSummary</span></span>|[<span data-ttu-id="444cf-165">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="444cf-165">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="444cf-166">Die Installationszusammenfassung für die mobile App.</span><span class="sxs-lookup"><span data-stu-id="444cf-166">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="444cf-167">deviceStates</span><span class="sxs-lookup"><span data-stu-id="444cf-167">deviceStates</span></span>|<span data-ttu-id="444cf-168">[deviceInstallState](../resources/intune-books-deviceinstallstate.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="444cf-168">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="444cf-169">Die Liste der Installationsstatus für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="444cf-169">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="444cf-170">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="444cf-170">userStateSummary</span></span>|<span data-ttu-id="444cf-171">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="444cf-171">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="444cf-172">Die Liste der Installationsstatus für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="444cf-172">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="444cf-173">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="444cf-173">JSON Representation</span></span>
<span data-ttu-id="444cf-174">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="444cf-174">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBook"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBook",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "publishedDateTime": "String (timestamp)",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "informationUrl": "String",
  "privacyInformationUrl": "String"
}
```




