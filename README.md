# Problem Statement
Natural disasters can cause substantial damage to buildings, making accurate damage assessment essential for emergency response. This project resolves deep learning approaches for detecting buildings and quantifying damage score by analyzing satellite imagery that captures before and after natural disasters.

# Dataset
To train the models we use the [xBD Dataset](https://xview2.org/dataset) which contains annotated high-resolution satellite imagery for building damage assessment. The dataset consists of:
- Six disaster types(Earthquake/Tsunami, Flood, Volcanic Eruption, Wildfire and Wind),
- 850,736 buildings and 
- 45,361 sq km.

Each building is assessed in one of the following categories based on its damage:
|Label|Description|
|-|-|
|No Damage| No signs of water, structural damage, shingle damage or burn marks.|
|Minor Damage | Building partialy burn, water surrounding the structure, volcanic flow nearby, roof elements missing or visible cracks.|
| Major Damage | Partial wall of roof collapse, encroaching voicanic flow, or the structure is surrounded by water or mud.|
| Destroyed | Structure is scorched, completely collapsed, partially or completely covered with water or mud, or no longer present.|

# Problem Challenge
In this project, we implement a model that does **binary semantic segmentation** in order to identify whether a building has been damaged and **classify** the extent of the damage. The main challenge is that most pixels in the images correspond to the background rather than buildings, resulting in a highly imbalanced problem.
