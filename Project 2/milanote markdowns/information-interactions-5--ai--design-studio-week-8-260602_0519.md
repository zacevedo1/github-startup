# Information Interactions #5 // AI + Design Studio - week 8

## 1st Notebook summary

This notebook provides a comprehensive look at the intersection of computing infrastructure, artificial intelligence, and environmental sustainability. It explores how the tech industry is tackling its massive energy and resource footprint through innovative hardware, software optimizations, circular economy principles, and compliance with emerging European regulations.

Building on our previous discussions about Microsoft and embodied carbon, here is a detailed, thematic summary of the notebook's contents:

**1. Corporate Sustainability Targets and "Green AI"** The notebook uses Microsoft’s 2025 Environmental Sustainability Report as a primary case study for corporate climate action. Microsoft is aiming to be carbon negative, water positive, and zero waste by 2030. To achieve this, companies are employing a variety of tactics:

- **Infrastructure:** Transitioning to carbon-free energy (including nuclear power), using low-carbon building materials like mass timber, and running backup generators on renewable diesel.

- **AI for Earth:** Utilizing AI foundation models (like Microsoft's Aurora for weather prediction) and the Planetary Computer to monitor global ecosystems, protect biodiversity, and optimize water and energy resources.

- **The AI Energy Wall:** Research on "Energy-Aware Computing" highlights that training and running Large Language Models (LLMs) requires massive power. To combat this, the industry is exploring Small Language Models (SLMs) for edge computing, optimizing code, and using techniques like "Carbon-Aware Prompt Caching" to avoid redundant, power-heavy computations.

**2. Advanced Cooling and Waste Heat Recovery** As server racks become denser, traditional air cooling is no longer sufficient.

- **Liquid & Immersion Cooling:** To handle the immense heat of AI chips, the industry is moving toward closed-loop liquid cooling and two-phase immersion cooling. These systems are designed to minimize or entirely eliminate water evaporation, driving a facility's Water Usage Effectiveness (WUE) down to zero.

- **District Heating:** Rather than venting waste heat into the atmosphere, companies are capturing it to heat local communities. For example, Google is recovering heat from its Hamina data center in Finland to supply 80% of the heating demand for nearby households and schools. Other global data centers are undertaking similar "heat reuse" projects across Europe and North America.

**3. The Circular Economy and Digital Product Passports (DPP)** A major focus of the notebook is how to reduce electronic waste and extend the lifespan of hardware.

- **Ecodesign for Sustainable Products Regulation (ESPR):** The EU is pushing for a circular economy by mandating a Digital Product Passport (DPP) for physical goods. The DPP acts as a digital technical file containing data on a product's origin, materials, repair instructions, and recycling guidance.

- **Decentralized Identifiers (DIDs) & Verifiable Credentials (VCs):** To implement these passports securely without exposing trade secrets, researchers propose using DIDs and VCs. This allows a manufacturer to prove what a product is made of, and lets owners or repair shops seamlessly log repairs to the passport over the product's lifecycle.

- **SME Impact:** Studies (like CIRPASS) are evaluating how these new DPP data requirements will impact Small and Medium-sized Enterprises, noting both the administrative costs of compliance and the benefits of increased supply chain transparency.

**4. Strict New EU Regulatory Mandates** Beyond the DPP, the notebook outlines stringent new legal requirements for data centers operating in Europe:

- **Energy Efficiency Directive (EED):** The EU now requires data centers with an installed IT power demand of at least 500kW to publicly report highly detailed sustainability KPIs, including their energy consumption, power utilization, and water usage.

- **Mandatory Heat Reuse:** Under the EED, new data centers commencing operations after July 2026 will be legally required to reuse a minimum share of their waste heat (starting at 10% and scaling up).

In short, the notebook is a deep dive into **how the tech sector is trying to balance the explosive growth of AI and cloud computing with hard physical limits on energy, water, and materials**, driven both by corporate climate pledges and aggressive new European legislation.

## LM Notebook Chat

<mark>does this notebook also cover the embodied carbon impact?</mark>

Yes, the notebook covers the embodied carbon impact extensively, addressing it across data center construction, computing hardware manufacturing, and cooling technologies.

Here are the key ways embodied carbon is addressed in the sources:

**Data Center Construction and Infrastructure** Microsoft focuses heavily on reducing the embodied carbon footprint of the built environment:

- **Low-Carbon Materials:** Microsoft is using a hybrid construction model featuring mass timber (cross-laminated timber), which is projected to reduce the embodied carbon footprint of new data centers by 35% compared to conventional steel and up to 65% compared to typical precast concrete.

- **HVAC and Hardware Structures:** Heating, ventilation, and air conditioning (HVAC) systems represent a significant portion of a data center's embodied carbon. Microsoft is testing alternative materials like polyethylene terephthalate (PET) film and fiber-reinforced plastic to replace steel in hot aisle containment units, which reduces material mass by up to 75% and cuts embodied carbon.

- **Measurement Tools:** To precisely track and manage these emissions, Microsoft utilizes Environmental Product Declarations (EPDs) and Building Transparency’s Embodied Carbon in Construction Calculator (EC3). These tools enable project teams to move away from broad estimates to make data-driven decisions that prioritize low-carbon materials.

**Computing Hardware and Semiconductors** As power grids decarbonize, the _Energy-Aware Computing in the Year 2026_ report notes that the predominant environmental impact of computing is shifting from operational carbon toward embodied carbon—specifically the emissions tied to semiconductor manufacturing, rare earth mining, server production, and transportation.

- **Life Cycle Assessments (LCA):** The report emphasizes the need for a unified "Pareto LCA frontier" to balance the operational energy savings of custom AI chips (ASICs) against the massive embodied carbon footprint required to manufacture them. Replacing servers every two to three years prevents data centers from ever achieving true carbon neutrality.

- **Chiplets and Heterogeneous Integration:** By fragmenting monolithic silicon into "chiplets," manufacturers can reduce embodied carbon emissions by 30% compared to traditional monolithic systems.

- **Photonic Computing:** Replacing copper interconnects with light-based data buses is another promising avenue, as manufacturing photonic hardware requires at least 4.1 times less manufacturing energy (embedded carbon) while offering higher yields.

**Cooling Technologies** While advanced liquid and immersion cooling strategies vastly improve operational efficiency, researchers note a current blind spot regarding embodied carbon: the embodied energy and environmental costs of manufacturing the dielectric fluids (particularly high-Global Warming Potential fluorocarbons) used in these systems have not yet been comprehensively evaluated.

<mark>is this notebook using Microsoft as an example for progress of sustainable AI</mark>

Yes, the notebook extensively features Microsoft as a primary case study and example for the progress and implementation of sustainable AI. The sources highlight Microsoft's efforts across several key areas:

**Optimizing AI Infrastructure and Cooling**

- **Zero-Water Cooling for AI:** To address the intense heat generated by GPU servers supporting AI, Microsoft is deploying a new datacenter design that uses chip-level liquid cooling. This method provides precise temperature control without evaporation, consuming zero water for cooling and saving an estimated 125,000 cubic meters of water annually per facility.

- **Offsetting AI's Carbon Footprint:** Through the DACinDC program, Microsoft is prototyping ways to repurpose the excess waste heat generated by AI workloads to power Direct Air Capture (DAC) systems, effectively offsetting the carbon footprint of AI computations.

**Green Software and AI Architecture**

- **Efficiency Guidelines:** Microsoft is developing the "Azure Well-Architected Framework for AI," which provides best practices for designers and developers to ensure AI applications are optimized for energy and cost efficiency across the entire infrastructure stack.

- **Inference Optimization:** Microsoft research teams are pioneering novel approaches to Large Language Model (LLM) inference, such as splitting the "prefill" and "decode" phases of inference requests across separate, specialized machines. This technique can deliver 2.35 times more throughput under the same power budget.

**Applying AI to Solve Global Sustainability Challenges (AI for Good)** The sources also detail how Microsoft uses AI as a tool to accelerate environmental sustainability:

- **Water Conservation:** Microsoft funds projects that use AI to rapidly and accurately detect pipe leaks in city water distribution networks and optimize precision irrigation for farmers.

- **Biodiversity and Ecosystems:** Microsoft's AI for Good Lab supports projects like Project Guacamaya (using AI bioacoustics to protect the Amazon) and the Wild Nature Institute (using computer vision to track and protect endangered Masai giraffes in Tanzania).

- **Climate Forecasting:** Microsoft developed Aurora, a 1.3-billion parameter AI foundation model that predicts atmospheric processes, extreme weather events, and air pollution, providing high-resolution global environmental forecasts.

- **Renewable Energy Monitoring:** In collaboration with partners, Microsoft helped build the Global Renewables Watch, which uses AI and satellite imagery to map and monitor utility-scale wind and solar installations worldwide to track clean energy transitions.

<mark>in the information interactions i did not see anything about timber nor did it mention it, why is it an important factor to Microsofts sustainability plans</mark>

Timber—specifically "mass timber" or cross-laminated timber (CLT)—is a critical component in Microsoft's strategy to decarbonize the built environment of its data centers.

While I briefly mentioned it in our first exchange regarding embodied carbon, here is exactly why it plays such a major role in their sustainability plans:

- **Tackling High-Emission Materials:** Traditional construction materials like steel and cement are highly carbon-intensive, together contributing to an estimated 13.5% of global carbon emissions.

- **Significant Carbon Reductions:** By substituting these traditional materials with mass timber, which is a strong yet ultra-lightweight wood, Microsoft can drastically reduce a facility's embodied carbon.

- **The Hybrid Construction Model:** In 2024, Microsoft launched its first data centers using a hybrid model that incorporates CLT alongside traditional steel and concrete. This specific approach is projected to reduce the embodied carbon footprint of new data centers by 35% compared to conventional steel construction, and by up to 65% compared to typical precast concrete.

Ultimately, because over 97% of Microsoft's total emissions fall under Scope 3 (value chain emissions, which includes capital goods like building materials), finding sustainable alternatives to concrete and steel is essential. Utilizing low-carbon materials like timber is a primary way Microsoft plans to reduce these emissions and reach its goal of becoming carbon negative by 2030.

How does mass timber compare to traditional steel for datacenters?

What other low-carbon materials is Microsoft using in construction?

How does mass timber help Microsoft reach its carbon-negative goal?

<mark>what exactly is the scope 1,2, and 3 emissons, i keep seeing them but i dont understand what they are or what they mean</mark>

Here is how greenhouse gas emissions are categorized into three "scopes," which helps organizations track exactly where their carbon footprint comes from:

- **Scope 1:** These are the **direct emissions** created by a company's own activities. This includes emissions from sources the company directly owns or controls, such as the fuel burned in their own facilities or company vehicles.

- **Scope 2:** These are **indirect emissions** that come from the generation of the purchased electricity, steam, heat, or cooling that a company buys to run its operations.

- **Scope 3:** These are all **other indirect emissions** that occur up and down the company's entire value chain. This covers everything outside of their direct control, such as the materials they purchase from suppliers, the transportation of their goods, employee business travel, and even the electricity customers use to run the company's sold products.

**Why Scope 3 is so critical (and why we talked about timber):** For Microsoft, Scope 3 is by far the biggest challenge, accounting for more than 97% of their total emissions. The vast majority of these emissions come from "Capital Goods" (nearly 41%) and "Purchased Goods and Services" (34%).

This means that to effectively reach their goal of being carbon negative, Microsoft has to focus heavily on decarbonizing the industrial processes of their suppliers. This includes the manufacturing of computer chips, jet fuel for logistics, and the heavy building materials (like steel and concrete) used to construct their data centers.

This is exactly why substituting highly emissive concrete and steel with low-carbon mass timber (as we discussed earlier) is such a crucial part of their strategy to tackle these massive Scope 3 emissions!

<mark>all is well in having goals but what are the physical actions Microsoft is taking to meet these goals?</mark>

To move beyond abstract strategies and look at exactly what Microsoft is physically doing in the real world, here are the tangible actions they are taking across their infrastructure, hardware, and environmental projects:

**Physical Construction and Infrastructure**

- **Building with Wood:** As we discussed earlier, Microsoft is physically swapping out highly emissive steel and concrete for mass timber (cross-laminated timber) in the construction of their new data centers.

- **Geothermal Plants:** At their Puget Sound headquarters, they physically built the "Thermal Energy Center," a facility that uses deep geothermal energy to provide carbon-free heating and cooling to their buildings.

- **Alternative Cooling Hardware:** They are outfitting their new AI data centers with closed-loop, direct-to-chip liquid cooling systems where cooling liquid is physically circulated directly onto the silicon chips, completely eliminating the need to evaporate municipal water for cooling.

**Energy and Logistics Modifications**

- **Restarting a Nuclear Plant:** Microsoft signed a physical procurement agreement to help restart the retired 835-megawatt Crane Clean Energy Center nuclear facility in Pennsylvania to put reliable, carbon-free energy back onto the power grid.

- **Retrofitting Generators:** They are physically modifying their data centers' backup power generators to run on renewable diesel instead of conventional fossil fuel, which includes installing new local tank permitting and specific physical heaters to keep the renewable fuel warm in cold climates.

- **Electric Freight and Sustainable Fuel:** They are physically replacing traditional shipping methods by using electric vehicle trucking fleets for data center deliveries and substituting standard jet fuel for sustainable aviation fuel when flying cloud hardware across the world.

**Water and Ecosystem Interventions**

- **Building Fake Beaver Dams:** To help restore water quality and flow in watersheds, Microsoft is funding the physical construction of "beaver dam analogs"—human-made structures in rivers that mimic natural beaver dams.

- **Extracting Water from the Air:** At their Hyderabad campus in India, they installed roughly 300 solar-powered air-to-water panels that physically extract water vapor from the atmosphere to generate over 1,600 liters of clean drinking water daily.

- **Harvesting Rain and Condensate:** In Malaysia, they are installing physical rainwater harvesting and filtration systems at 50 schools. In India, they are capturing the physical water condensation that steams off of sugarcane during the sugar manufacturing process, purifying it, and distributing it to local villages for drinking water.

- **Planting Trees:** They have planted over 77,000 trees in urban forestry projects and contracted to plant over 10 million seedlings across 16,000 hectares in Brazil to naturally regenerate the Atlantic and Amazon Forests.

**Tackling Physical Waste**

- **Manual Server Teardowns:** Microsoft has physically built six "Circular Centers" globally (with more on the way) where workers manually harvest, recertify, and reuse parts from decommissioned cloud servers, achieving a 90.9% reuse and recycling rate.

- **Making Devices Repairable:** They have completely physically redesigned their Surface laptops and Xbox consoles to include "field replaceable units" (like screens, batteries, motherboards, and HDMI ports) held together with accessible screws so that users or repair shops can physically fix broken devices rather than throwing them away.

- **Scrapping Plastic Foam:** They have physically removed hard-to-recycle expanded plastic foam from their cloud server and Xbox packaging, replacing it with recyclable paper and pulp alternatives.

## Report

2025 Microsoft Environmental Sustainability Report: Briefing Document

Executive Summary

This document synthesizes the progress, challenges, and strategic shifts outlined in the 2025 Microsoft Environmental Sustainability Report, covering the 2024 fiscal year. At the halfway point to its 2030 goals, Microsoft remains committed to becoming carbon negative, water positive, and zero waste, while protecting more land than it consumes.

A primary challenge identified is the tension between rapid business growth—driven by the expansion of AI and cloud services—and the company's carbon reduction targets. While total emissions have increased by 23.4% since the 2020 baseline, this growth is significantly lower than the 168% increase in energy use and 71% revenue growth over the same period.

**Critical Takeaways:**

- **Carbon Dynamics:** Scope 1 and 2 emissions have decreased by 29.9%, but Scope 3 emissions (representing 97.29% of the total) have increased by 26%.

- **Energy Leadership:** Microsoft has contracted 34 GW of carbon-free electricity (CFE) across 24 countries, an eighteenfold increase since 2020.

- **Infrastructure Innovation:** The company is transitioning to "mass timber" datacenters (reducing embodied carbon by up to 65%) and chip-level liquid cooling to handle heat-intensive AI workloads.

- **Market Scaling:** In FY24 alone, Microsoft contracted nearly 22 million metric tons of carbon removal, more than all previous years combined.

- **Goal Milestones:** Targets for land protection and clean water access (1.5 million people) have already been achieved or exceeded ahead of the 2030 deadline.

\--------------------------------------------------------------------------------

Strategic Framework: The Three Pillars

Microsoft organizes its sustainability efforts into three distinct but interconnected pillars designed to scale impact beyond its internal operations.

Table element string placeholder

\--------------------------------------------------------------------------------

Carbon Negative: A "Marathon, Not a Sprint"

The report characterizes the journey to becoming carbon negative as a long-term endeavor requiring a transition from short-term stopgaps to fundamental infrastructure changes.

The Emissions Profile

The vast majority of Microsoft's carbon footprint resides in Scope 3 (indirect value chain emissions), primarily from purchased goods, services, and capital goods.

- **Scope 1 & 2:** Decreased 30% from 2020 baseline through clean energy procurement and carbon fees.

- **Scope 3:** Increased 26% from 2020 baseline.

- **Key Drivers:** AI and cloud expansion are the primary contributors to increased emissions.

Decarbonizing the Value Chain

To address Scope 3 growth, Microsoft has implemented several aggressive strategies:

- **Supplier Mandates:** The 2024 Supplier Code of Conduct now requires select large-scale suppliers to transition to 100% carbon-free electricity for goods and services delivered to Microsoft by 2030.

- **Sustainable Aviation Fuel (SAF):** New guidance launching in July 2030 will target the use of SAF for business-related air travel.

- **Logistics Optimization:** Adoption of renewable diesel for road freight in Europe and California has reduced emissions for those shipments by 50%.

\--------------------------------------------------------------------------------

Infrastructure and Operational Efficiency

Microsoft is redefining how it builds and operates the physical infrastructure necessary for the AI era.

Datacenter Transformation

- **Low-Carbon Materials:** The launch of mass timber datacenters uses cross-laminated timber (CLT) to reduce embodied carbon by 35% compared to steel and 65% compared to precast concrete.

- **Advanced Cooling:** Transitioning from air-cooled systems to chip-level liquid cooling at all owned datacenters. This eliminates water consumption for evaporation and supports higher rack capacity.

- **Energy Optimization:** "Power harvesting" and low-power server states have reduced energy usage on unallocated servers by up to 35%.

Campus Modernization

- **Thermal Energy Center:** The Puget Sound headquarters modernization includes a facility using geothermal energy for carbon-free heating and cooling.

- **Electrification:** Following the success of 100% electric food halls in the U.S., Microsoft is expanding kitchen electrification to India and fully electrifying vehicle fleets in regions like Dublin, Paris, Shanghai, and Suzhou.

\--------------------------------------------------------------------------------

Scaling Availability of Green Solutions

Microsoft acts as a "first-mover" to build the markets it needs to reach its goals, particularly in energy and carbon removal.

Carbon-Free Electricity (CFE)

- **Renewable Expansion:** In 2024, the company contracted 19 GW of new renewable energy. This includes a 10.5 GW framework with Brookfield Renewable.

- **Nuclear Energy:** Signed a first-of-its-kind large-scale PPA to restart the 835-MW Crane Clean Energy Center in Pennsylvania, aiming to provide reliable CFE to the PJM power grid.

- **Circular PPAs:** Agreements with Engie require 100% of solar modules to be recycled or reused at end-of-life.

Carbon Removal Portfolio

Microsoft is shifting exclusively to carbon _removal_ rather than _avoidance_ credits.

- **FY24 Milestone:** Nearly 22 million metric tons contracted in FY24 alone.

- **Diverse Pathways:**

    - **BECCS:** A 10-year agreement with Stockholm Exergi for 3 million metric tons.

    - **ARR (Reforestation):** 15-year agreement with re.green to plant 10 million seedlings in the Amazon.

    - **DAC (Direct Air Capture):** Innovative "DACinDC" programs explore using waste heat from datacenters to power carbon capture systems.

\--------------------------------------------------------------------------------

Water, Waste, and Ecosystems

Progress in non-carbon categories remains ahead of or on track with 2030 targets.

Water Positive

- **Clean Water Access:** Met the goal of providing 1.5 million people with water and sanitation solutions.

- **Replenishment:** On track to replenish more water than consumed; contracted 104 million cubic meters of lifetime replenishment to date.

Zero Waste

- **Circular Hardware:** Reached a 90.9% reuse and recycling rate for servers and components.

- **Construction Waste:** Diverted 85% of construction and demolition waste in FY24, exceeding the 75% target six years early.

- **Packaging:** Redirected over 2,500 metric tons of waste from landfills by recycling packaging from 30,000 server racks.

Protecting Ecosystems

- **Land Protection:** Achieved the 2025 goal in 2022. Microsoft now protects 17,000 acres, exceeding its land-use footprint by more than 30%.

- **AI for Good:** Utilizing the Planetary Computer and AI for Good Lab to drive biodiversity conservation and climate resilience research.

\--------------------------------------------------------------------------------

Global Innovation and Investment

The **Climate Innovation Fund (CIF)**, a $1 billion commitment, has allocated $793 million to 63 investments. These focus on high-impact technologies such as:

- Industrial decarbonization (e.g., Stegra's near-zero-carbon steel).

- Sustainable fuels and long-duration energy storage.

- Nature-based solutions through the **Symbiosis Coalition**, targeting 20 million metric tons of carbon removal credits by 2030.

"We remain pragmatically optimistic because of the promise of new sustainability technologies, innovations in AI, and market solutions that are emerging which can accelerate progress across challenging sectors."

## Data Table

Table element string placeholder

## Reflection

When i was going into this information interaction i was not expecting to learn that Microsoft is actually on a path to try and create sustainable AI, and after reading it and looking deeper into it, i believe this is going to be apart of my strongest backings for my website, to show that it actually is possible. While all of the other information interactions did provide me with useful information, i believe this information interaction provided me a path to follow, to show what a sustainable AI data infrastructure looks like, that not only applies to green energy but also tackles the biggest challenge, embodied carbon. A few interactions ago i figured that the AI chips within the data centers were one of the main issues when it came down to carbon emissions and that to tackle that challenge we had to focuses on that only within that category, however after learning how Microsoft is also planing on fighting the embodied carbon issue with the way the actual infrastructure is build on, now i believe i have a solid understanding on sustainable AI. Like when i learned it i literally went "why did i not think of that", basically opening up new doors of understanding. 

Not only that but the closed-loop design and direct-to-chip liquid cooling i learned about last time, actually make sense now because these process help optimize and push the life span of these chips, and whats even better is that this design eliminates the need for water evaporation for cooling by recycling water within a sealed system. The best part about this too is the way Microsoft is being transparent about this process by releasing sustainability reports every year, and the fact that theres a whole team of people and auditors to review and check this information. This information interactions was like a fresh breath of air, because as i've been going through this project i've been having a lot of doubt if i can even put this together, let alone change someones mind on what we actually need to fight for rather then completely getting rid of AI.  However, this all seems a little to good to be true so im still planing on being on the skeptical side of things, however this has provided me with a good idea of a stable infrastructure (for now of course).

My next step after this is to finalize the last part of this project which is talking about advocacy and the importance of people staying aware of whats going on with AI.

## 2nd NoteBook sumary

This notebook provides a comprehensive overview of Microsoft’s environmental sustainability strategy, focusing heavily on its ambitious 2030 commitments, the specific projects it is funding to reach those goals, and its 2025 Environmental Sustainability Report detailing progress and challenges.

Microsoft has committed to becoming **carbon negative, water positive, and zero waste by 2030**, while also protecting more land than it uses. The company characterizes this journey as a "marathon, not a sprint," acknowledging the challenges posed by business growth, particularly the massive infrastructure and energy demands required for artificial intelligence (AI) and cloud computing.

Here is an extremely detailed summary of the notebook, broken down by its core pillars:

1\. Carbon Negative by 2030

By 2030, Microsoft aims to cut its emissions by more than half and remove more carbon than it emits. By 2050, it intends to remove all the carbon the company has emitted since its founding in 1975.

**Progress and Carbon Math:**

- **Scopes 1 & 2:** Microsoft has successfully reduced its direct operational and purchased electricity emissions by nearly 30% from a 2020 baseline.

- **Scope 3:** Indirect value chain emissions represent over 97% of Microsoft's total footprint. These emissions increased by 26% in FY24 due to the construction of new datacenters and the manufacturing of hardware.

- **Internal Carbon Fee:** Microsoft utilizes an internal carbon tax paid by its business divisions to fund sustainability improvements. This fee has been expanded to cover all Scope 1, 2, and 3 emissions.

**Decarbonizing Infrastructure and Operations:**

- **Mass Timber Datacenters:** Microsoft is pioneering hybrid construction models using cross-laminated timber (mass timber), steel, and concrete to build datacenters. This method reduces embodied carbon by up to 65% compared to traditional precast concrete.

- **Supply Chain & Logistics:** A new Supplier Code of Conduct requires select suppliers to transition to 100% carbon-free electricity by 2030. The company is also utilizing renewable diesel in its road freight operations (cutting emissions by 50%) and expanding sustainable aviation and marine fuels for hardware shipments.

- **Energy Procurement:** Microsoft has contracted over 34 gigawatts (GW) of carbon-free electricity across 24 countries, an eighteenfold increase since 2020. This includes solar, wind, and a recent major agreement with Constellation to restart an 835-MW nuclear facility in Pennsylvania.

**Scaling Carbon Dioxide Removal (CDR):** Reduction is the first priority, but Microsoft also procures high-quality carbon removal credits to offset residual and historical emissions. The company takes a "portfolio approach" investing in projects with varying durability. In FY24 alone, they contracted nearly 22 million metric tons of CDR.

- **Enhanced Rock Weathering:** A partnership with **Lithos Carbon** crushes volcanic basalt and spreads it on farmlands. Rainwater reacts with the rock to form bicarbonate ions, locking carbon in the ocean for over 10,000 years while improving soil health.

- **Bioenergy with Carbon Capture and Storage (BECCS):** **Stockholm Exergi** captures carbon from a bioenergy plant that burns sustainable forestry waste. The condensed carbon is then shipped and stored deep under the North Sea.

- **Regenerative Farming & Reforestation:** **Agoro Carbon Alliance** helps farmers use no-till methods and cover crops to sequester carbon in the soil. In Brazil, **re.green** uses drones and AI to restore native tropical forests in the Amazon and Atlantic Forest biomes.

- **Biochar:** **Exomad Green** thermally decomposes forestry residues without oxygen to lock up carbon in a soil enhancement.

2\. Water Positive by 2030

Microsoft’s strategy focuses on reducing water use, increasing clean water access, and replenishing more water than it consumes in highly stressed basins.

**Progress & Efficiency:**

- Microsoft met its target of providing 1.5 million people with clean water access in 2023, funding projects that use air-to-water generation, rainwater harvesting, and even capturing condensate from sugarcane manufacturing in India.

- **Zero-Water Datacenters:** New datacenter designs optimizing AI workloads have transitioned to chip-level liquid cooling. This closed-loop system applies cooling liquid directly to silicon chips without relying on evaporation, saving an estimated 125,000 cubic meters of water annually per facility.

**Replenishment Projects:** Since 2020, Microsoft has contracted 76 projects aimed at delivering over 100 million cubic meters of replenishment volume.

- **Beaver Dam Analogs:** Partnering with Trout Unlimited, Microsoft funds human-made structures that mimic beaver dams to restore aquatic habitats, control flooding, and replenish groundwater.

- **AI for Water Management:** Microsoft funds AI leak-detection technologies in major cities (reducing global water loss from leaking pipes) and AI-powered precision irrigation systems for farmers in drought-stricken regions like Chile.

3\. Zero Waste by 2030

Microsoft has integrated circular economy principles into its cloud hardware, campuses, and consumer devices.

**Cloud Hardware & Datacenters:**

- Microsoft exceeded its 2025 target early, achieving a **90.9% reuse and recycling rate** for cloud hardware servers and components in FY24. This is driven by their global "Circular Centers," which harvest and recertify decommissioned server parts.

- They achieved an **85.3% waste diversion rate** for construction and demolition projects, six years ahead of schedule.

**Devices and Packaging:**

- The company is phasing out single-use plastics, with packaging recyclability currently at 94.8%.

- **Surface Devices:** The newest Surface Copilot+ PCs feature 100% recycled aluminum alloy enclosures and 100% recycled rare earth metals in their magnets. Devices are designed to be highly repairable, with replacement components (like displays, motherboards, and batteries) and published service guides freely available.

4\. Protecting Ecosystems

Microsoft committed to protecting more land than it uses by 2025, a goal it met in 2022 and has currently exceeded by more than 30%.

**Key Initiatives:**

- Datacenters and campuses are designed using ecological principles, utilizing native landscaping, pollinator gardens (with bee hotels), and bird-safe glass.

- **The Planetary Computer:** A massive open-source data platform hosting over 50 petabytes of Earth observation data. It allows researchers, governments, and organizations to use spatial analysis and AI to monitor global ecosystem health, track climate risks, and build environmental resilience.

- **AI for Biodiversity:** Microsoft supports projects like "Project Guacamaya" in Colombia (using bioacoustics and AI to protect the Amazon) and AI models that automate the identification of endangered Masai giraffes in Tanzania.

The Role of AI and Software

The notebook highlights a profound duality: AI is a massive resource challenge, but it is also a powerful tool for sustainability.

- **Green Software:** Microsoft co-founded the Green Software Foundation to build standards that measure the software carbon intensity of applications. They optimize Azure cloud computing to run workloads during times of high renewable energy availability.

- **Gaming:** Xbox has introduced energy-saving "shutdown" modes (saving 20x the power of Sleep mode), highly efficient 6-nm chips, and tools for developers to measure and reduce the energy impact of their games. Through Minecraft, Microsoft also drives real-world climate education and tree planting.

- **Climate Innovation Fund:** A $1 billion fund that has allocated $793 million across 63 companies to scale climate technologies, including sustainable aviation fuel, sustainable steel, and advanced battery storage.

In summary, this notebook details a highly structured, data-driven approach by Microsoft. The company uses advanced life cycle assessments (LCAs), internal carbon fees, global policy advocacy, and unprecedented investments in nascent technologies to combat its growing energy footprint and move the entire technology sector toward a more circular and decarbonized economy.

## LM Notebook Chat

<mark>for embedded carbon foot print what about the chips, how do they plan on tackling that</mark>

To tackle the embedded carbon footprint of chips (semiconductors), Microsoft is focusing on precise measurement, industry collaboration, and advanced cooling technologies. Specifically, their strategy includes:

- **Partnering for Semiconductor Sustainability:** Microsoft participates in the Interuniversity Microelectronics Centre (IMEC) Sustainable Semiconductor Technologies and Systems program, which is dedicated to assessing and reducing the environmental impacts of semiconductor manufacturing.

- **Customized Tracking and Forecasting:** Through this partnership, Microsoft uses customized life cycle inventories for over 400 chip configurations. This allows them to track different chip generations, forecast emissions, and precisely differentiate the environmental impacts across various devices and Azure hardware configurations.

- **Improving Life Cycle Assessments (LCAs):** Microsoft integrates this semiconductor manufacturing data from IMEC, along with carbon-free electricity data from its suppliers, into its product environmental LCAs. This results in highly accurate, primary-data-driven assessments that help identify carbon hotspots and prioritize reduction strategies.

- **Chip-Level Liquid Cooling:** To maximize the lifespan and efficiency of these chips, Microsoft is transitioning to chip-level liquid cooling designs in its datacenters. This technology allows for significantly greater rack capacity, which reduces the need to construct new datacenters and cuts down on the associated embodied carbon emissions.

- **Supplier Carbon-Free Electricity Requirements:** Broader supply chain initiatives also help reduce the embedded carbon of components like chips. For instance, Microsoft now requires its suppliers to transition to 100% carbon-free electricity for goods and services delivered to the company by 203

## Report

Briefing Document: 2025 Microsoft Environmental Sustainability Report

Executive Summary

The 2025 Environmental Sustainability Report marks the halfway point in Microsoft’s ten-year journey to fulfill its 2030 commitments of becoming carbon negative, water positive, and zero waste, while protecting more land than it uses. The report characterizes this journey as "a marathon, not a sprint," highlighting a complex landscape where rapid business growth—driven largely by the expansion of AI and cloud services—presents a significant resource challenge even as those same technologies offer new tools for climate solutions.

**Critical Takeaways:**

- **Carbon Resilience:** While total emissions have increased by 23.4% since 2020 due to AI and cloud expansion, Scope 1 and 2 emissions have decreased by 29.9%. Scope 3 emissions remain the primary challenge, rising 26% from the 2020 baseline.

- **Energy Transformation:** Microsoft has increased its carbon-free electricity (CFE) program eighteenfold since 2020, contracting over 34 GW of renewable energy across 24 countries and signing its first large-scale nuclear power purchase agreement (PPA).

- **Water and Waste Success:** The company has met its 2030 target for providing clean water access to 1.5 million people and reached a 90.9% reuse and recycling rate for server components.

- **Ecosystem Protection:** Microsoft exceeded its land protection target by more than 30%, protecting 17,000 acres—far more land than it currently uses.

- **Strategic Shift:** The company is moving away from non-additional environmental attribute certificates toward bringing more new carbon-free electricity onto the grids where it operates.

\--------------------------------------------------------------------------------

Core Sustainability Pillars and Progress to 2030

Microsoft’s sustainability strategy is organized into three pillars: managing its own operational footprint (**Microsoft sustainability**), empowering partners and customers (**Customer sustainability**), and catalyzing market conditions for a net-zero economy (**Global sustainability**).

1\. Carbon Negative: Addressing the "AI Growth" Challenge

Microsoft aims to reduce emissions by more than half compared to 2020 and remove more carbon than it emits by 2030. By 2050, the company plans to remove all historical operational emissions since its founding in 1975.

**Current Emissions Profile**

Table element string placeholder

Efficiency and Infrastructure Innovation

To mitigate the resource intensity of AI, Microsoft is rethinking datacenter design:

- **Low-Carbon Materials:** Launched the first datacenters using mass timber (cross-laminated timber), projected to reduce embodied carbon by 35% compared to steel and 65% compared to precast concrete.

- **Power Harvesting:** Maximizing power use by reallocating unused power from workloads, doubling the rate of power savings in the last year.

- **Cooling Technology:** Transitioning to chip-level liquid cooling designs which eliminate evaporation and support higher rack capacity, reducing the need for new construction.

- **Operational States:** Implementing low-power server states, reducing energy usage on unallocated servers by up to 35%.

Availability and Market Scaling

- **Carbon-Free Electricity (CFE):** Contracted 19 GW of renewable energy in 2024 alone. A landmark deal with the Crane Clean Energy Center will restart an 835-MW nuclear facility in Pennsylvania to provide reliable CFE to the PJM grid.

- **Carbon Removal:** In FY24, Microsoft signed long-term agreements for nearly 22 million metric tons of carbon removal—more than all previous years combined. This includes bioenergy with carbon capture and storage (BECCS), direct air capture (DAC), and reforestation.

- **Circular Energy:** Groundbreaking PPAs now require 100% of solar modules to be reused or recycled at the end of their life cycle.

2\. Water Positive: Replenishment and Access

The "water positive" goal involves replenishing more water than is consumed across global operations and providing 1.5 million people with clean water access.

- **Target Achieved:** The clean water access target was met in 2023.

- **Innovative Designs:** New datacenter designs for AI workloads aim for zero water consumption for cooling, avoiding an estimated 125,000 cubic meters of water use per facility annually.

- **Replenishment:** Microsoft has contracted 104 million cubic meters in lifetime water replenishment.

3\. Zero Waste: Circularity in the Cloud

Microsoft’s zero-waste strategy focuses on the circularity of hardware and packaging.

- **Cloud Hardware:** Surpassed the target for server and component reuse and recycling, reaching a 90.9% rate.

- **Construction Waste:** Exceeded the 75% diversion target six years early, achieving an 85% diversion rate for construction and demolition waste in FY24.

- **Supply Chain Logistics:** Diverted over 2,500 metric tons of waste from landfills by processing packaging from more than 30,000 server racks.

4\. Protecting Ecosystems: AI-Driven Conservation

The company remains committed to protecting more land than it uses, a target originally met in 2022.

- **Land Management:** Currently protecting 17,000 acres, exceeding the original target by 30%.

- **Technology for Nature:** Using the AI for Good Lab and tools like the Microsoft Planetary Computer to drive biodiversity research and habitat protection.

\--------------------------------------------------------------------------------

Global Impact and Innovation

Microsoft leverages its capital and technology to accelerate the broader global energy transition.

- **Climate Innovation Fund (CIF):** A $1 billion commitment to advance climate technologies. To date, CIF has allocated over $793 million to 63 investments, including sustainable aviation fuel, industrial decarbonization, and direct air capture.

- **Supplier Engagement:** A new target in the Supplier Code of Conduct requires large-scale suppliers to transition to 100% CFE for Microsoft-delivered goods and services by 2030.

- **Logistics Decarbonization:** Adopted renewable diesel for road freight in Europe and California (cutting emissions by 50%) and partnered with airlines/shipping lines to use sustainable fuels, reducing CO2 emissions by over 17,000 metric tons.

- **Symbiosis Coalition:** Co-founded to target 20 million metric tons of high-quality, nature-based carbon removal credits by 2030.

\--------------------------------------------------------------------------------

Key Insight Quotes

"Microsoft remains pragmatically optimistic because of the promise of new sustainability technologies, innovations in AI, and market solutions that are emerging which can accelerate progress across challenging sectors." — **Brad Smith & Melanie Nakagawa**

"Sustainability is not simply a set of isolated initiatives, but a fundamental principle that must be integrated into every aspect of our business."

"We remain resolute in our commitment not only to meeting our climate goals but to empowering others with the technology they need to build a more sustainable future."

\--------------------------------------------------------------------------------

Conclusion: Learnings and the Path Ahead

The report acknowledges that the road to 2030 is non-linear. While Microsoft has seen success in water, waste, and land targets, the increase in total carbon emissions due to AI expansion requires a pivot toward long-term structural changes. The company is prioritizing "long-term solutions over short-term stopgaps," focusing on decarbonizing building materials (steel and concrete), scaling carbon removal markets, and enforcing stricter supplier standards. This approach seeks to build a "sustainable engine" that can support continued technological innovation without compromising environmental integrity.

## Data Table

Table element string placeholder