**1. Hoja de referencia de aprendizaje profundo**

&#10230;

<br> 

**2. Redes Neuronales**

&#10230;

<br> 

**3. Las redes neuronales son una clase de modelos que an sido construidos con capas. Los tipos de redes neuronales comúnmente utilizados incluyen redes neuronales convolucionales y recurrentes.**

&#10230;

<br>

**4. Arquitectura - el vocabulario relacionados con la arquitectura de las redes neuronales es descrito en la siguiente figura:**

&#10230;

<br> 

**5. [Input layer, hidden layer, output layer]**

&#10230;

<br>

**6. By noting i the ith layer of the network and j the jth hidden unit of the layer, we have:**

&#10230;

<br>

**7. where we note w, b, z the weight, bias and output respectively.**

&#10230;

<br>

**8. Función de activación - Las funciones de activación son usadas al final de una unidad oculta a para introducir complejidades no lineales en el modelo. Aqui estan los más comunes:**

&#10230;

<br> 

**9. [Sigmoid, Tanh, ReLU, Leaky ReLU]**

&#10230;

<br>

**10. Perdida de entropía cruzada . En el contexto de las redes neuronales, la perdida de entropía cruzada L(z,y) es comunmente usada y se define de la siguiente manera:**

&#10230;

<br>

**11. Tasa de aprendizaje - la taza de aprendizaje, amenudo anotado  α o a veces η, indica a que ritmo se actualizan los pesos. Este puede ser fijo o adaptivo. El metodo actual más popular es llamado Adam, que es un metodo que se adapta a la taza de aprendizaje.**	

&#10230;

<br> 

**12. Propagación hacia atrás - La propagación hacia atrás es un metodo para actualizar los pesos en la red neuroral tomando en consideración la salida actual y la salida deseada. La derivada con respecto al peso w se calcula utilizando la regla de la cadena y es de la siguiente forma:**

&#10230;

<br> 

**13. Como resultado, el peso es actualizado de la siguiente manera:**

&#10230;

<br> 

**14. Updating weights ― In a neural network, weights are updated as follows:**

&#10230;

<br>

**15. Step 1: Take a batch of training data.**

&#10230;

<br>

**16. Step 2: Perform forward propagation to obtain the corresponding loss.**

&#10230;

<br>

**17. Step 3: Backpropagate the loss to get the gradients.**

&#10230;

<br>

**18. Step 4: Use the gradients to update the weights of the network.**

&#10230;

<br>

**19. Dropout ― Dropout is a technique meant at preventing overfitting the training data by dropping out units in a neural network. In practice, neurons are either dropped with probability p or kept with probability 1−p**

&#10230;

<br>

**20. Convolutional Neural Networks**

&#10230;

<br>

**21. Convolutional layer requirement ― By noting W the input volume size, F the size of the convolutional layer neurons, P the amount of zero padding, then the number of neurons N that fit in a given volume is such that:**

&#10230;

<br>

**22. Batch normalization ― It is a step of hyperparameter γ,β that normalizes the batch {xi}. By noting μB,σ2B the mean and variance of that we want to correct to the batch, it is done as follows:**

&#10230;

<br>

**23. It is usually done after a fully connected/convolutional layer and before a non-linearity layer and aims at allowing higher learning rates and reducing the strong dependence on initialization.**

&#10230;

<br>

**24. Recurrent Neural Networks**

&#10230;

<br>

**25. Types of gates ― Here are the different types of gates that we encounter in a typical recurrent neural network:**

&#10230;

<br>

**26. [Input gate, forget gate, gate, output gate]**

&#10230;

<br>

**27. [Write to cell or not?, Erase a cell or not?, How much to write to cell?, How much to reveal cell?]**

&#10230;

<br>

**28. LSTM ― A long short-term memory (LSTM) network is a type of RNN model that avoids the vanishing gradient problem by adding 'forget' gates.**

&#10230;

<br>

**29. Reinforcement Learning and Control**

&#10230;

<br>

**30. The goal of reinforcement learning is for an agent to learn how to evolve in an environment.**

&#10230;

<br>

**31. Definitions**

&#10230;

<br>

**32. Markov decision processes ― A Markov decision process (MDP) is a 5-tuple (S,A,{Psa},γ,R) where:**

&#10230;

<br>

**33. S is the set of states**

&#10230;

<br>

**34. A is the set of actions**

&#10230;

<br>

**35. {Psa} are the state transition probabilities for s∈S and a∈A**

&#10230;

<br>

**36. γ∈[0,1[ is the discount factor**

&#10230;

<br>

**37. R:S×A⟶R or R:S⟶R is the reward function that the algorithm wants to maximize**

&#10230;

<br>

**38. Policy ― A policy π is a function π:S⟶A that maps states to actions.**

&#10230;

<br>

**39. Remark: we say that we execute a given policy π if given a state a we take the action a=π(s).**

&#10230;

<br>

**40. Value function ― For a given policy π and a given state s, we define the value function Vπ as follows:**

&#10230;

<br>

**41. Bellman equation ― The optimal Bellman equations characterizes the value function Vπ∗ of the optimal policy π∗:**

&#10230;

<br>

**42. Remark: we note that the optimal policy π∗ for a given state s is such that:**

&#10230;

<br>

**43. Value iteration algorithm ― The value iteration algorithm is in two steps:**

&#10230;

<br>

**44. 1) We initialize the value:**

&#10230;

<br>

**45. 2) We iterate the value based on the values before:**

&#10230;

<br>

**46. Maximum likelihood estimate ― The maximum likelihood estimates for the state transition probabilities are as follows:**

&#10230;

<br>

**47. times took action a in state s and got to s′**

&#10230;

<br>

**48. times took action a in state s**

&#10230;

<br>

**49. Q-learning ― Q-learning is a model-free estimation of Q, which is done as follows:**

&#10230;
