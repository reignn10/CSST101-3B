# CSST101-3B

[Introduction Video](https://www.youtube.com/watch?v=mUMcwxoxHbg)  
*Click the image to watch the video.*


# Introduction to AI and Knowledge Representation in Beauty Industry

With the use of artificial intelligence (AI), machines can replicate human intelligence and be capable of learning, reasoning, and decision-making. AI-driven solutions are transforming customer experience and personalization in the cosmetics business. **Knowledge Representation (KR)**, which describes how AI systems represent, organize, and manipulate knowledge to carry out difficult tasks, is one essential component of AI systems.

---

## Forms of Knowledge Representation in AI

1. **Semantic Networks:** Concept relationships represented graphically. Semantic networks, for instance, are used by AI in the cosmetics industry to link items to user preferences, ingredients, and skin types.
2. **Frames:** Data structures used to group knowledge into smaller sections. A frame may convey information about a cosmetic product, such as its aim, ingredients, and skin-benefiting properties.
3. **Logic-Based Representations:** These represent knowledge and make inferences using formal logic. AI can apply reasoning to assess user reviews and choose the best products to recommend depending on skin issues.

---

## AI Application in the Beauty Industry

### **Skincare Recommendation System**

An AI-powered Skincare Recommendation System personalizes product recommendations according to skin type, preferences, and weather conditions. This system uses **frames** and **semantic networks** to comprehend the connections between skin types and product characteristics like ingredients and moisture content.

#### Problems it addresses:
- **Personalization:** Adapting suggestions to meet the needs of each client.
- **Decision Making:** Choosing the best product based on a variety of factors like skin type and seasonal variations.

---

## Model for Personalized Skincare Recommendations

Our model represents knowledge using a **Semantic Network**. The network connects the following:
- **Skin Types:** (combination, dry, oily)
- **Product Ingredients:** (e.g., salicylic acid, hyaluronic acid)
- **Results:** (e.g., remedy for acne, hydration)

The AI system uses this model to evaluate user input (skin issues) and match it with suitable products. It then makes individualized skincare regimen recommendations based on the link between skin type, ingredient, and effect.

---

## Importance of Knowledge Representation in AI

AI systems need effective knowledge representation to learn, reason, and make decisions. In the beauty industry, this facilitates highly customized recommendations, enhancing customer satisfaction. Structured knowledge representation enables AI to process complex data and generate valuable insights.

---

## References

- Russell, S., & Norvig, P. (2021). *Artificial Intelligence: A Modern Approach*. Pearson.
- Brachman, R. J., & Levesque, H. J. (2004). *Knowledge Representation and Reasoning*. Elsevier.
- Li, F., Zhang, Y., & Liu, W. (2023). "AI-Powered Personalization in the Beauty Industry." *Journal of AI Applications*, 45(2), 189-202.






# Propositional and Predicate Logic Implementation

## 1. Propositional Logic Operations
This section implements basic propositional logic operations such as **AND**, **OR**, **NOT**, and **IMPLIES** using Python functions:
- `and_operation(p, q)` returns `True` if both `p` and `q` are true.
- `or_operation(p, q)` returns `True` if either `p` or `q` is true.
- `not_operation(p)` returns `True` if `p` is false.
- `implies_operation(p, q)` represents the logical implication (p → q), which is equivalent to `not p or q`.

### Example:
For `p = True` and `q = False`, the operations return:
- **AND**: False
- **OR**: True
- **NOT**: False
- **IMPLIES**: False

## 2. Evaluating Logical Statements
The `evaluate` function allows users to evaluate logical expressions dynamically. It takes a logical statement as a string and a dictionary of truth values for variables.

### Example:
Evaluating the statement `implies_operation(p, q)` where `p = True` and `q = False` returns `False`.

## 3. Predicate Logic with Quantifiers
This section introduces **predicate logic** with two common quantifiers: `forall` (universal quantifier) and `exists` (existential quantifier).
- `forall(predicate, domain)` returns `True` if the predicate holds true for all elements in the domain.
- `exists(predicate, domain)` returns `True` if the predicate holds true for at least one element in the domain.

### Example:
A predicate function `is_even(x)` checks whether a number is even. Using this predicate:
- **forall** over the domain `[1, 2, 3, 4, 5]` returns `False` (not all numbers are even).
- **exists** over the same domain returns `True` (there is at least one even number).

## 4. AI Agent Making Decisions using Logic
The `ai_decision` function demonstrates a simple AI agent that makes decisions based on environmental conditions.

### Example:
For the condition `{'is_raining': True, 'is_sunny': False}`, the AI decides to **"Take an umbrella"**.

## Conclusion
This implementation of propositional and predicate logic in Python provides a basic foundation for logical reasoning and decision-making. The code can be extended to more complex scenarios in AI, including knowledge representation and inference systems.
