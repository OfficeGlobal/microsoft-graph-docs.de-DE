---
title: journalLines-Ressourcentyp
description: Eine Journal Zeile in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 7a6841bcc2f893f8ca794e7d8e6aeafbcd4e48ca
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365955"
---
# <a name="journallines-resource-type"></a><span data-ttu-id="7b12c-103">journalLines-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7b12c-103">journalLines resource type</span></span>
<span data-ttu-id="7b12c-104">Stellt eine Zeile in einem Journal in Dynamics 365 Business Central dar.</span><span class="sxs-lookup"><span data-stu-id="7b12c-104">Represents a line in a journal in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="7b12c-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="7b12c-105">Methods</span></span>

| <span data-ttu-id="7b12c-106">Methode</span><span class="sxs-lookup"><span data-stu-id="7b12c-106">Method</span></span>                                                    | <span data-ttu-id="7b12c-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="7b12c-107">Return Type</span></span>|<span data-ttu-id="7b12c-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7b12c-108">Description</span></span>         |
|:----------------------------------------------------------|:-----------|:-------------------|
|[<span data-ttu-id="7b12c-109">JournalLines abrufen</span><span class="sxs-lookup"><span data-stu-id="7b12c-109">Get journalLines</span></span>](../api/dynamics-journalline-get.md)      |<span data-ttu-id="7b12c-110">journalLines</span><span class="sxs-lookup"><span data-stu-id="7b12c-110">journalLines</span></span>|<span data-ttu-id="7b12c-111">Ruft eine Journal Zeile ab.</span><span class="sxs-lookup"><span data-stu-id="7b12c-111">Gets a journal line.</span></span>   |
|[<span data-ttu-id="7b12c-112">Post journalLines</span><span class="sxs-lookup"><span data-stu-id="7b12c-112">Post journalLines</span></span>](../api/dynamics-create-journalline.md)  |<span data-ttu-id="7b12c-113">journalLines</span><span class="sxs-lookup"><span data-stu-id="7b12c-113">journalLines</span></span>|<span data-ttu-id="7b12c-114">Erstellt eine Journal Zeile.</span><span class="sxs-lookup"><span data-stu-id="7b12c-114">Creates a journal line.</span></span>|
|[<span data-ttu-id="7b12c-115">Patch-journalLines</span><span class="sxs-lookup"><span data-stu-id="7b12c-115">Patch journalLines</span></span>](../api/dynamics-journalline-update.md) |<span data-ttu-id="7b12c-116">journalLines</span><span class="sxs-lookup"><span data-stu-id="7b12c-116">journalLines</span></span>|<span data-ttu-id="7b12c-117">Aktualisiert eine Journal Zeile.</span><span class="sxs-lookup"><span data-stu-id="7b12c-117">Updates a journal line.</span></span>|
|[<span data-ttu-id="7b12c-118">JournalLines löschen</span><span class="sxs-lookup"><span data-stu-id="7b12c-118">Delete journalLines</span></span>](../api/dynamics-journalline-delete.md)|<span data-ttu-id="7b12c-119">Keine</span><span class="sxs-lookup"><span data-stu-id="7b12c-119">none</span></span>        |<span data-ttu-id="7b12c-120">Löscht eine Journal Zeile.</span><span class="sxs-lookup"><span data-stu-id="7b12c-120">Deletes a journal line.</span></span>|

## <a name="properties"></a><span data-ttu-id="7b12c-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7b12c-121">Properties</span></span>
| <span data-ttu-id="7b12c-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7b12c-122">Property</span></span>             | <span data-ttu-id="7b12c-123">Typ</span><span class="sxs-lookup"><span data-stu-id="7b12c-123">Type</span></span>                   |<span data-ttu-id="7b12c-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7b12c-124">Description</span></span>                                                        |
|:---------------------|:-----------------------|:------------------------------------------------------------------|
|<span data-ttu-id="7b12c-125">id</span><span class="sxs-lookup"><span data-stu-id="7b12c-125">id</span></span>                    |<span data-ttu-id="7b12c-126">GUID</span><span class="sxs-lookup"><span data-stu-id="7b12c-126">GUID</span></span>                    |<span data-ttu-id="7b12c-127">Die eindeutige ID der Erf.-Journal Zeile.</span><span class="sxs-lookup"><span data-stu-id="7b12c-127">The unique ID of the journal line.</span></span> <span data-ttu-id="7b12c-128">Nicht bearbeitbar.</span><span class="sxs-lookup"><span data-stu-id="7b12c-128">Non-editable.</span></span>                   |
|<span data-ttu-id="7b12c-129">journalDisplayName</span><span class="sxs-lookup"><span data-stu-id="7b12c-129">journalDisplayName</span></span>    |<span data-ttu-id="7b12c-130">Zeichenfolge, maximale Größe 10</span><span class="sxs-lookup"><span data-stu-id="7b12c-130">string, maximum size 10</span></span> |<span data-ttu-id="7b12c-131">Der Anzeigename des Journals, zu dem diese Zeile gehört.</span><span class="sxs-lookup"><span data-stu-id="7b12c-131">The display name of the journal that this line belongs to.</span></span> <span data-ttu-id="7b12c-132">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7b12c-132">Read-Only.</span></span>|
|<span data-ttu-id="7b12c-133">lineNumber</span><span class="sxs-lookup"><span data-stu-id="7b12c-133">lineNumber</span></span>            |<span data-ttu-id="7b12c-134">integer</span><span class="sxs-lookup"><span data-stu-id="7b12c-134">integer</span></span>                 |<span data-ttu-id="7b12c-135">Die Nummer der Erf.-Journal Zeile.</span><span class="sxs-lookup"><span data-stu-id="7b12c-135">The number of the journal line.</span></span>                                    |
|<span data-ttu-id="7b12c-136">accountId</span><span class="sxs-lookup"><span data-stu-id="7b12c-136">accountId</span></span>             |<span data-ttu-id="7b12c-137">GUID</span><span class="sxs-lookup"><span data-stu-id="7b12c-137">GUID</span></span>                    |<span data-ttu-id="7b12c-138">Die eindeutige ID des Kontos, mit dem die Journal Zeile verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="7b12c-138">The unique ID of the account that the journal line is related to.</span></span>  |
|<span data-ttu-id="7b12c-139">accountNumber</span><span class="sxs-lookup"><span data-stu-id="7b12c-139">accountNumber</span></span>         |<span data-ttu-id="7b12c-140">Zeichenfolge, maximale Größe 20</span><span class="sxs-lookup"><span data-stu-id="7b12c-140">string, maximum size 20</span></span> |<span data-ttu-id="7b12c-141">Die Nummer des Kontos, mit dem die Erf.-Journal Zeile verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="7b12c-141">The number of the account that the journal line is related to.</span></span>     |
|<span data-ttu-id="7b12c-142">postingDate</span><span class="sxs-lookup"><span data-stu-id="7b12c-142">postingDate</span></span>           |<span data-ttu-id="7b12c-143">date</span><span class="sxs-lookup"><span data-stu-id="7b12c-143">date</span></span>                    |<span data-ttu-id="7b12c-144">Das Datum, an dem die Erf.-Journal Zeile gebucht wurde.</span><span class="sxs-lookup"><span data-stu-id="7b12c-144">The date that the journal line is posted.</span></span>                          |
|<span data-ttu-id="7b12c-145">documentNumber</span><span class="sxs-lookup"><span data-stu-id="7b12c-145">documentNumber</span></span>        |<span data-ttu-id="7b12c-146">Zeichenfolge, maximale Größe 20</span><span class="sxs-lookup"><span data-stu-id="7b12c-146">string, maximum size 20</span></span> |<span data-ttu-id="7b12c-147">Gibt eine Dokumentnummer für die Erf.-Journal Zeile an.</span><span class="sxs-lookup"><span data-stu-id="7b12c-147">Specifies a document number for the journal line.</span></span>                  |
|<span data-ttu-id="7b12c-148">externalDocumentNumber</span><span class="sxs-lookup"><span data-stu-id="7b12c-148">externalDocumentNumber</span></span>|<span data-ttu-id="7b12c-149">Zeichenfolge, maximale Größe 20</span><span class="sxs-lookup"><span data-stu-id="7b12c-149">string, maximum size 20</span></span> |<span data-ttu-id="7b12c-150">Gibt eine externe Dokumentnummer für die Erf.-Journal Zeile an.</span><span class="sxs-lookup"><span data-stu-id="7b12c-150">Specifies an external document number for the journal line.</span></span>        |
|<span data-ttu-id="7b12c-151">Menge</span><span class="sxs-lookup"><span data-stu-id="7b12c-151">amount</span></span>                |<span data-ttu-id="7b12c-152">decimal</span><span class="sxs-lookup"><span data-stu-id="7b12c-152">decimal</span></span>                 |<span data-ttu-id="7b12c-153">Gibt den Gesamtbetrag (einschließlich MwSt.) an, aus dem die Erf.-Journal Zeile besteht.</span><span class="sxs-lookup"><span data-stu-id="7b12c-153">Specifies the total amount (including VAT) that the journal line consists of.</span></span>|
|<span data-ttu-id="7b12c-154">description</span><span class="sxs-lookup"><span data-stu-id="7b12c-154">description</span></span>           |<span data-ttu-id="7b12c-155">Zeichenfolge, maximale Größe 50</span><span class="sxs-lookup"><span data-stu-id="7b12c-155">string, maximum size 50</span></span> |<span data-ttu-id="7b12c-156">Die Beschreibung der Erf.-Journal Zeile, die vom Benutzer bereitgestellt oder selbst erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="7b12c-156">The description of the journal line, provided by the user or autocreated.</span></span>|
|<span data-ttu-id="7b12c-157">Kommentar</span><span class="sxs-lookup"><span data-stu-id="7b12c-157">comment</span></span>               |<span data-ttu-id="7b12c-158">Zeichenfolge, maximale Größe 250</span><span class="sxs-lookup"><span data-stu-id="7b12c-158">string, maximum size 250</span></span>|<span data-ttu-id="7b12c-159">Ein benutzerdefinierter Kommentar in der Erf.-Journal Zeile.</span><span class="sxs-lookup"><span data-stu-id="7b12c-159">A user specified comment on the journal line.</span></span>                      |
|<span data-ttu-id="7b12c-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7b12c-160">lastModifiedDateTime</span></span>  |<span data-ttu-id="7b12c-161">DateTime</span><span class="sxs-lookup"><span data-stu-id="7b12c-161">datetime</span></span>                |<span data-ttu-id="7b12c-162">Die letzte Uhrzeit, zu der die Journal Zeile geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="7b12c-162">The last datetime the journal line was modified.</span></span> <span data-ttu-id="7b12c-163">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7b12c-163">Read-Only.</span></span>        |

## <a name="relationships"></a><span data-ttu-id="7b12c-164">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7b12c-164">Relationships</span></span>
<span data-ttu-id="7b12c-165">Eine Buch.-Blattzeile ist eine Unterseite eines Journals.</span><span class="sxs-lookup"><span data-stu-id="7b12c-165">A journal line is a subpage of a journal.</span></span> <span data-ttu-id="7b12c-166">Er kann nicht direkt zugegriffen werden.</span><span class="sxs-lookup"><span data-stu-id="7b12c-166">It cannot be accessed directly.</span></span>

<span data-ttu-id="7b12c-167">Eine Buch.-Blattzeile kann eine "übergeordnete Entität" der Maßlinie sein.</span><span class="sxs-lookup"><span data-stu-id="7b12c-167">A journal line can be a "Parent Entity" of the dimension lines.</span></span>

<span data-ttu-id="7b12c-168">In der Tabelle Konten muss ein Konto (Konto-Nr.) vorhanden sein.</span><span class="sxs-lookup"><span data-stu-id="7b12c-168">An Account (accountId) must exist in the Accounts table.</span></span>


## <a name="json-representation"></a><span data-ttu-id="7b12c-169">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7b12c-169">JSON representation</span></span>

<span data-ttu-id="7b12c-170">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7b12c-170">Here is a JSON representation of the resource.</span></span>


```json
{
    "id": "GUID",
    "journalDisplayName": "string",
    "lineNumber": "integer",
    "accountId": "GUID",
    "accountNumber": "string",
    "postingDate": "date",
    "documentNumber": "string",
    "externalDocumentNumber": "string",
    "amount": "decimal",
    "description": "string",
    "comment": "string",
    "lastModifiedDateTime": "datetime"
}
```
