# Proposal Pack — HS-2026-02-09-F6C7 (DRAFT / INTAKE)

⚠️ DRAFT: This pack is a **blind build-up** of pricing recommendations (Paint Price Cube triangle + recommendation). Any “sent pricing” belongs in a separate REFERENCE section once we have it.

## Identity (per Luke)
- Client: **[REDACTED]**
- Realtor partner: **[REDACTED]**

## Source artifacts
- FastField zip: `source.zip` (extracted to `intake/`)
- FastField JSON: `FastField JSON/2faca561-6818-45f2-b095-6a6caf4ef6c7.json`
- Renamed photos: `renamed-images/` + `RENAMED-MANIFEST.json`

---

# 0) What’s in this pack
- Paint Price Cube (triangle) + recommendation
- Quick room list + tiers (from FastField notes)
- Gaps / confidence notes

---

# 1) PAINT — Cube + Recommendation

## Rooms included (paint-required)
(13 rooms; see JSON for full details)

## Tier calls (from FastField room notes)
- Tier 2: 10 rooms
- Tier 3: 3 rooms

## WorkedFloorSF (sanity)
- WorkedFloorSF is computed as Σ(L×W) across paint rooms.
- **Data normalization applied:** one room had a dimension captured as `515` (confirmed by Luke: should be **5.5 ft**, not 515 ft).
- WorkedFloorSF (normalized): **~1,669 sf**

## Paint Price Cube — triangle (DRAFT)
Constants used for back-into costs (benchmarks): fees f=10.25% pass-through; GM target g=40% net of fees; materials target m=13%.

### 1) Room Rate benchmark (preferred anchor)
- Room Rate LOW: **$7,125**  (~$4.27/sf)
- Room Rate MID: **$7,523**  (~$4.51/sf)
- Room Rate HIGH: **$7,920** (~$4.74/sf)

Back-into costs (MID):
- Materials cost (target): **~$978**
- Labor cost (allowed): **~$3,073**

### 2) $/Floor-sqft method (sanity band)
- $/sf LOW: **~$6,132**  (~$3.67/sf)
- $/sf MID: **~$6,475**  (~$3.88/sf)
- $/sf HIGH: **~$6,817** (~$4.08/sf)

Back-into costs (MID):
- Materials cost (target): **~$842**
- Labor cost (allowed): **~$2,645**

### 3) Cost Plus (production anchor)
Baseline heuristic (from Pricing Journal template): **2-person crew @ $300 per painter-day** (=$600 per crew-day).

Draft production assumption (paint):
- **2 painters × 5.0 days** = **10 painter-days**
- Internal labor cost estimate: **$3,000** (10 × $300)

Back into customer price using standard benchmarks (f=10.25% fees; g=40% GM net of fees; m=13% materials):
- Customer price (Cost Plus point): **~$7,345**
- Materials cost target (~13%): **~$955**
- Labor cost allowed: **~$3,000**
- Cost Plus customer $/sf (vs WorkedFloorSF ~1,669): **~$4.40/sf**

Assumptions note: this anchor assumes walls+ceilings in most rooms and no trim-pack/door repainting folded into base. If trim/doors are included, days and Cost Plus price should be increased.

## Recommendation (paint)
Given Tier 2/3 mix and walls+ceilings prevalence, recommend anchoring near Room Rate MID:
- **Recommended paint customer price: $7,500**

---

# 2) HANDYMAN — Labor estimate + scope list (FastField-driven; notes override)

## Labor estimate (draft)
- Estimated labor: **10.75 hours**
- Estimated labor $ (@$100/hr): **$1,075**

## Scope list (walkthrough order)
- Foyer — Install light fixture (flush mount)
- Kitchen — Install (2) light fixtures
- Dining Room — Install light fixture
- Family Room — Install (2) light fixtures (flush mount)
- Bathroom 1 — Mirror swap
- Bathroom 1 — Replace strip light fixture
- 2nd Floor Hallway — Install light fixture (flush mount)
- Main Bedroom — Install light fixture
- Main Bedroom — Install mirror
- Main Bathroom — Replace vanity fixture
- Main Bathroom — Replace panel mirror
- Bedroom 2 — Install light fixture
- Bedroom 3 — Install light fixture

## Copy/paste minutes list (line breaks)
30
60
45
90
45
60
30
45
60
45
45
45
45

## Copy/paste allowance list (tax-loaded, rounded; line breaks)
0
0
0
0
0
0
0
0
0
0
0
0
0

## Handyman — SCOPE DETAILS (paste-ready)
$100 Per Hour Plus the Cost of Materials:
- Foyer: Install flush-mount light fixture.
- Kitchen: Install (2) light fixtures.
- Dining Room: Install light fixture.
- Family Room: Install (2) flush-mount light fixtures.
- Bathroom 1: Swap/replace mirror and replace strip light fixture.
- 2nd Floor Hallway: Install flush-mount light fixture.
- Main Bedroom: Install light fixture and install mirror.
- Main Bathroom: Replace vanity light fixture and replace panel mirror.
- Bedroom 2: Install light fixture.
- Bedroom 3: Install light fixture.

Handyman terms (paste):

"The final handyman invoice is calculated based on actual hours, in 15 min increments, worked on completing the above tasks and the cost of purchasing any necessary materials to complete the job.

For the purposes of this quote, we've inserted our best estimate of the time needed to perform the above tasks. The final cost may be more or less than the provided number based on actual time spent.

Client is responsible for purchasing materials. Please confirm compatibility with HOMEStretch before purchasing to avoid delays and additional fees. HOMEstretch will make product recommendations and provide links for purchasing at no additional cost at clients request.

HOMEstretch can purchase on your behalf and deliver the necessary fixtures, faucets, and hardware to make this project easier for you. If you’d prefer this, please let us know, a 17% service fee will be added to the final cost of materials.

The time begins as soon as a HOMEstretch Team Member is on the client's property and ends as soon as a HOMEstretch Team Member leaves the client's property. Drive time is not billed."

### Notes override rule (FastField glitch aware)
- Include selected handyman dropdown tasks when present.
- If dropdown tasks are missing (common glitch; e.g., Bathroom 1), treat `handyman_handyman_notes` as authoritative scope text.

---

# 3) Gaps / confidence notes
- **Foyer dimension anomaly** in capture required normalization (see WorkedFloorSF note).
- If you want a tighter production-days estimate, confirm whether trim/doors are included and any high-sheen/dark-to-light color change notes.
