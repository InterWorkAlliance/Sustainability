# Carbon Reference Token (CRT)

A Carbon Reference Token (CRT) references one or more CRU tokens to represent a specified volume of
metric tons of greenhouse gas (GHG) emissions reduced or removed by the underlying CRUs.
The CRT has standard data elements that represent the shared view required by the parties in
the carbon market from suppliers, buyers, validation and verification bodies (“VVB”), registries, and
exchanges. These standard data elements are based on the recommendations from the ICVCM, with the
included CCP property-set.

Every CRT will have the following behaviors and properties:
- Is a fungible token that represents one metric ton of CO2 (tCO2) or 1 tCO2e of reduction or
avoidance.
- Is divisible, transferable, encumberable, revokable, delegable, offsetable and mintable with role
support.
- Unique identifier (Id): An identifier that is assigned when issued.
- Quantity: The amount of CO2e in tonnes, can have up to 4 decimal place precision.
- Owner: The Id of the account that is the owner of the token.
- Listing Agent Id (optional): If the CRT is listed on a marketplace or exchange.
- Core Carbon Principles (CCP): A set of properties that every CRT will have.
- Climate Labels (optional): Name/value pair of additional climate labels for compatibility.
- Issuer: The Id for the issuing standard registry.
- Retired (optional): True or false for implementations where it is not implicit.
- Offset Applied to Id (optional): A link to an ESG Scorecard or goal that the offset should apply.
- CRUs: A collection of the Ids of the CRUs referenced and encumbered by this token. 

**The complete draft of the TTF specification, including its token base and behaviors, for the [Carbon Removal Unit token](https://github.com/InterWorkAlliance/TokenTaxonomyFramework/tree/main/artifacts/token-templates/specifications/Carbon-Reference-Token/latest).**

## Using CRT

CRTs can be held for their value or spent to offset reported emissions in either a voluntary or a regulated
market. When an owner offsets using a CRT, they may retire the whole token or choose to decouple the
CRUs from the CRT, retire a select number of them, and then re-compose a new CRT with the unspent
CRUs. Any retirement can be applied towards an ESG Goal or another target and is retired or burned
and cannot be offset again. See ESG Scorecard.

## Issues with CRT

Narrowing the list of attributes to cover most demand signals may cause limitations when it comes to
value variables including:

- Year scale for Global Warming Potential (GWP) for calculating GHG CO2e:
  - 100yr GWP vs. 20yr GWP for methane (CH4) that has greater warming potential in the 20yr vs.
100yr GWP.

### Additionality

Additionality, for carbon reduction, is whether it would have happened without the existence of the
project. This is a complicated and controversial topic—relying on logic that can be difficult to prove in
either direction.

There is not a single, clear market agreement for how to calculate the baseline against which a project’s
impact gets measured. Project developers can misuse baselines, resulting in inflated credit values.
Baselines against which removals are estimated must be set conservatively to minimize risk of overcrediting.
No best practice, or common authoritative standards body guiding best practices, exists to guide
decisions on how carbon finance and corporate procurement of credits contribute to additionality. Some
projects have received criticism because payments for carbon credits are only a percentage of the entire
project funding stack or because landowners don’t know that the project is generating carbon credits.

### Baseline

Establishing an accurate and fair baseline to measure progress, like reductions measurement requires a
baseline level to be established. Historically, establishing a baseline has been troublesome for validation
of claims.

### Leakage

Some projects inadvertently shift emissions from one geographic area to another area that is not
counted in the project claim. Activity leakage occurs when an activity is displaced from one geographic
area to another. Market leakage occurs when a project reduces the supply of a specific product, but
market demand encourages others to provide that product instead. For example, carbon removal
might be achieved in one area by letting trees grow longer but may indirectly result in trees being cut
elsewhere to satisfy timber market demands. To improve leakage determinations, registries should
develop stronger science-based benchmarks for leakage that are informed by research. 
