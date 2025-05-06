# Identifying Key Entities in Recipe Data

## Business Objective
The goal of this project is to train a Named Entity Recognition (NER) model using Conditional Random Fields (CRF) to extract key entities from recipe data. The model will classify words into predefined categories such as **ingredients, quantities, and units**, enabling the creation of a structured database of recipes and ingredients. This structured data can be utilized for advanced applications such as:
- Recipe management systems
- Dietary tracking apps
- E-commerce platforms

## Data Description
The provided dataset is in **JSON format**, representing structured ingredient lists with Named Entity Recognition (NER) labels. The dataset consists of:
- **`input`**: A raw ingredient list extracted from a recipe.
- **`pos`**: Corresponding part-of-speech (POS) or NER labels, categorizing tokens as quantities, units, or ingredients.

### **Sample Data Format**
```json
[
    {
        "input": "6 Karela Bitter Gourd Pavakkai Salt 1 Onion 3 tablespoon Gram flour besan 2 teaspoons Turmeric powder Haldi Red Chilli Cumin seeds Jeera Coriander Powder Dhania Amchur Dry Mango Sunflower Oil",
        "pos": "quantity ingredient ingredient ingredient ingredient ingredient quantity ingredient quantity unit ingredient ingredient ingredient quantity unit ingredient ingredient ingredient ingredient ingredient ingredient ingredient ingredient ingredient ingredient ingredient ingredient ingredient ingredient ingredient ingredient"
    },
    {
        "input": "2-1/2 cups rice cooked 3 tomatoes teaspoons BC Belle Bhat powder 1 teaspoon chickpea lentils 1/2 cumin seeds white urad dal mustard green chilli dry red 2 cashew or peanuts 1-1/2 tablespoon oil asafoetida",
        "pos": "quantity unit ingredient ingredient quantity ingredient unit ingredient ingredient ingredient ingredient quantity unit ingredient ingredient quantity ingredient ingredient ingredient ingredient ingredient ingredient ingredient ingredient ingredient ingredient quantity ingredient ingredient ingredient quantity unit ingredient ingredient"
    }
]

