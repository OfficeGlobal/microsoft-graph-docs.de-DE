# <a name="privacyprofile-resource-type"></a><span data-ttu-id="07e2a-101">privacyProfile-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="07e2a-101">privacyProfile resource type</span></span>

<span data-ttu-id="07e2a-102">Stellt das Datenschutzprofil eines Unternehmens dar, das eine URL zu einer Datenschutzerklärung sowie eine Kontaktperson für Fragen im Zusammenhang mit der Datenschutzerklärung umfasst.</span><span class="sxs-lookup"><span data-stu-id="07e2a-102">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="07e2a-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="07e2a-103">Properties</span></span>
| <span data-ttu-id="07e2a-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="07e2a-104">Property</span></span>   | <span data-ttu-id="07e2a-105">Typ</span><span class="sxs-lookup"><span data-stu-id="07e2a-105">Type</span></span>|<span data-ttu-id="07e2a-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="07e2a-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07e2a-107">contactEmail</span><span class="sxs-lookup"><span data-stu-id="07e2a-107">contactEmail</span></span>|<span data-ttu-id="07e2a-108">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="07e2a-108">String</span></span>| <span data-ttu-id="07e2a-109">Eine gültige SMTP-E-Mail-Adresse für den Kontakt für die Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="07e2a-109">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="07e2a-110">Nicht erforderlich.</span><span class="sxs-lookup"><span data-stu-id="07e2a-110">Not required</span></span>|
|<span data-ttu-id="07e2a-111">statementUrl</span><span class="sxs-lookup"><span data-stu-id="07e2a-111">statementUrl</span></span>|<span data-ttu-id="07e2a-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="07e2a-112">String</span></span>| <span data-ttu-id="07e2a-113">Ein gültiges URL-Format, das mit „http://“ oder „https://“ beginnt.</span><span class="sxs-lookup"><span data-stu-id="07e2a-113">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="07e2a-114">Die maximale Länge beträgt 255 Zeichen.</span><span class="sxs-lookup"><span data-stu-id="07e2a-114">The maximum length is 255 characters.</span></span> <span data-ttu-id="07e2a-115">Die URL, die zur Datenschutzerklärung des Unternehmens weiterleitet.</span><span class="sxs-lookup"><span data-stu-id="07e2a-115">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="07e2a-116">Nicht erforderlich.</span><span class="sxs-lookup"><span data-stu-id="07e2a-116">Not required</span></span>|

## <a name="json-representation"></a><span data-ttu-id="07e2a-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="07e2a-117">JSON representation</span></span>

<span data-ttu-id="07e2a-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="07e2a-118">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privacyProfile"
}-->

```json
{
  "contactEmail": "string",
  "statementUrl": "string"
}
```