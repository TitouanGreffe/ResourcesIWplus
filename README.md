# Additional energy Cost Potential (ACP) and Resource Services Deficit Assessment (RESEDA) methods
Python code to generate marginal characterization factors of 50 metallic elements (copper, aluminium, lithium, etc.) and three fossil resources (crude oil, natural gas, coal) dissipative flows using the WILMFLo model (https://github.com/TitouanGreffe/WILMFlo) introduced in Greffe et al. 2025 (https://doi.org/10.1016/j.resconrec.2025.108482).

## Classification method
The elemental composition of elementary flows in life cycle inventory databases, such as ecoinvent, are derived using _cirpy_ and _pubchempy_ python packages. Regarding the characterization of metals dissipative flows, we characterize emissions of substances to the environment which contain at least one characterized element (e.g. copper). Regarding the characterization of fossil dissipative flows, we characterize emissions of fossil carbon dioxide, fossil methane, fossil carbon monoxide and microplastics emissions to air/water/soil (11 polymers, 5 particle sizes) using the ratio of carbon content in emissions relatively to the carbon content in both crude oil, natural gas and coal. Radioisotopes emissions are also characterized as dissipative flows, by converting the mass of a radionuclide to its activity in kiloBecquerel, since radionuclide are reported in kBq in LCI databases, such as ecoinvent.
An article entitled "Operationalizing the characterization of potential impacts of dissipative flows of mineral and fossil resources" presenting in detail the classification method will be submitted soon and will be available in a pre-print by the end of 2026.

# Impact pathways

![Impact pathways from resource dissipation to damage on ecosystem services through adaptation and respectively non-adaptation pathways. The first one addressed by the additional energy cost potential (ACP, blue arrows) and the second one by the Resource Services Deficit Assessment (RESEDA, red arrows)](doc/impact_pathway.png)


## Adaptation to resources services loss: the ACP method
This midpoint indicator assesses the additional effort to extract resources, resulting from the adaptation to a marginal dissipative flow of resources. This additional cost is assessed in terms of MJ, i.e., the additional energy required to extract the resource, because of dissipation.

## Resources services deficit: the RESEDA method
This midpoint indicator assesses the potential deficit of resources resulting from a marginal dissipative flow, considering the global demand and resulting dissipation until 2100 as the background dissipation. According to the model of Greffe et al. (2026), a marginal dissipative flow of only three resources may lead to a potential deficit under a business-as-usual trajectory: copper, cobalt and lithium. Thus, only elementary flows containing those three elements have are characterized by this indicator.


# Characterization factors

Developped characterization factors integrated in version 2.2.1 of IMPACT World+ are available on openLCA, SimaPro and brightway here: https://zenodo.org/records/18892673

# Author 
Titouan Greffe (greffe.titouan@uqam.ca)

# Reference
Greffe, T., Margni, M., & Bulle, C. (2026). Scenario-specific temporally differentiated characterization factors of dissipative flows of abiotic resources: introduction to the ACP and RESEDA methods. The International Journal of Life Cycle Assessment, 31(1–3), 42. https://doi.org/10.1007/s11367-026-02593-5
