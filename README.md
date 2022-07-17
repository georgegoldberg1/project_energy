# README for Project Energy

Analysis of UK Energy Use

Part of my personal "Ignorance reduction" series. This series is about understanding the issues that are so commonly spoken about in the media, but rarely I take the effort to look through the raw data. Ideally, if the media or politicians say something is "really bad" I want to know, how bad in reality, are the underselling it or is the issue less priority than other issues and theyre using it as a stunt for publicity.

Goal: to understand the extent of energy use in the uk. How much of the national grid is from renewable sources, how is this changing, and how far is there to go?

# Renewables/sustainable energy Considerations:

Manufacture components for energy collection

- Energy cost of building/maintaining/using machinery to extract materials and construct components for sale/purchase
- Land ownership/leasing/fees of mining raw materials - country of origin / ownership etc
- Technology ownership - eg for Processing raw materials -  Chinese cobalt processing Dem.Rep.Congo monopoly?
- Sustainability of using non-renewable /non-recyclable materials in components
- Illegal Labor/exploitation practices

Maintenance costs

- cleaning solar panels
- replacing/fixing wind turbine blades
- Theft of components from site location: eg people stealing copper wiring solar farms

Grid connectivity

- Efficiency of transit/ distance from source to home/industry

Components performance

- Efficiency of power conversion and Power output of the components
- Consistency of power output (eg day >> night for solar)
- Consistency of voltage output (fine-tuning to grid fluctuations)
- Useable life of components
- Ease and cost of recylability

Storage method and conversion technologies

- Due to solar inconsistency etc
- Same manufacturing concerns covered in components section above (eg mining materials, labor malpractice and costs/lifetime of batteries etc etc)

Other factors

- Useable land for power plant/facility (eg is there enough sacrificial space required to do this type of energy collection)
- Destructive byproduct of using a technology / facility (eg hydroelectric dams wiping out villages due to reservoir above dam, and causing water shortages downstream due to flow constriction)
- Wind farms disrupting wildlife - danger to birds/aviation
- Residents objection to noise of proximity to turbines
- Readiness of energy source in the future
- Cost to invest in clean tech relative to GDP of country or current financial situation. Prioritising this over other issues

To investigate:

- Net neutral commitments by country
- Current supply chain monopolies and leaders




# README for Base Python Docker  

Builds ubuntu docker container, installing pip requirements for python and running jupyter notebook in your local browser.

Maps this repo folder into Docker so you can create and save notebooks and then git push outside of docker afterwards.

# Setup:

### Build and start container  
`bash go.sh`

### Stop container 
`bash stop.sh`  
(OR: `docker stop base_python`)
note: each time you run `bash go.sh`, it will stop the container that is currently running, so be careful if you havent saved changes in notebooks.

### Remove all stopped containers
`docker container rm $(docker ps -aq)`

## Optional:requirements.txt
You can change the packages in requirements.txt
After you run the container, it's recommended to do a pip freeze on the package versions, so this build will hold for future. Python version should be included too ideally.


## Version details
- python3.10 currently in ubuntu 22.04)  
- Works on Apple Silicon.  
- Updated June2022

## Author
George Goldberg
