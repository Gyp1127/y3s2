# Feedforward Networks
- Practice reading the simple neural network, constructing your own, graphing it out and putting it on a truth table.
- Understand the different activation functions (Threshold, Linear, Gaussian, Sigmoid)
- Understand how a neural network can recognise if a given character is an 'I', 'L' or 'T'

# The Interactive Activation and Competition Network

<details>
<summary>1. What does the Interactive Activation and Competition Network consist of?</summary>
It consists of a number of competitive pools of units where each unit represents some micro-hypothesis or feature.
</details>

<details>
<summary>2. How are units within each competitive pool related?</summary>
Units within each competitive pool are mutually exclusive features and are interconnected with negative weights.
</details>

<details>
<summary>3. What do positive weights between the pools indicate?</summary>
Between the pools, positive weights indicate features or micro-hypotheses which are consistent.
</details>

<details>
<summary>4. What happens to units connected by positive weights to active units during the network cycle?</summary>
When the network is cycled, units connected by positive weights to active units become more active.
</details>

<details>
<summary>5. How do negative weights impact the active units?</summary>
Units connected by negative weights to active units are inhibited.
</details>

<details>
<summary>6. Are the connections in the network unidirectional?</summary>
No, connections are, in general, bidirectional making the network interactive.
</details>

<details>
<summary>7. What does the Jets and Sharks Network represent?</summary>
The network represents information about two rival gangs - the Jets and Sharks.
</details>

<details>
<summary>8. What do the central pool of units in the Jets and Sharks Network represent?</summary>
The central pool of units represent members of the two gangs.
</details>

<details>
<summary>9. What do the pools around the edges represent?</summary>
The pools around the edges represent features of these members including their name, occupation, marital status, gang membership, age, and educational level.
</details>

<details>
<summary>10. How are the units within each pool of the Jets and Sharks Network connected?</summary>
Within each pool, the units are connected with negative weights indicating that they are mutually exclusive.
</details>

<details>
<summary>11. Give an example to explain the mutual exclusivity of units within the pool in the Jets and Sharks Network.</summary>
If you are in your 20s, you can't also be in your 30s.
</details>

<details>
<summary>12. How is specific information about each gang member held in the Jets and Sharks Network?</summary>
Between the pools, positive weights hold the specific information about each gang member.
</details>

<details>
<summary>13. How can the activations of each of the units be perceived?</summary>
The activations of each of the units can be thought of as the "degree of belief" in that hypothesis or the existence of that feature.
</details>

<details>
<summary>14. How do weights indicate the connection between beliefs in the Interactive Activation and Competition Mechanism?</summary>
The weights are an indication of how strongly belief in one hypothesis or feature implies belief in another hypothesis or feature.
</details>

<details>
<summary>15. How is the net input for a unit determined?</summary>
The net input for unit i is: net i = ∑w ij a j where w ij is the weight from unit j to unit i and a j is the activation of unit j.
</details>

<details>
<summary>16. What happens to the activation function if net i < 0?</summary>
If (net i < 0), Δa i = (max - a i ) net i - decay (a i - rest).
</details>

<details>
<summary>17. When does the network believe the hypothesis completely?</summary>
If the activation of a unit is equal to max, then the net believes the hypothesis completely.
</details>

<details>
<summary>18. What are the default values for max, min, rest, and decay in the Activation Function?</summary>
By default, max is set to 1, min is set to -0.2, rest is set to -0.1, and decay is 0.1.
</details>

<details>
<summary>19. What is Decay in the context of IAC Networks?</summary>
Decay is the tendency for a unit to return to the rest value.
</details>

<details>
<summary>20. What is the significance of Equilibrium in IAC Networks?</summary>
Equilibrium is the point to which a network will settle.
</details>

<details>
<summary>21. What does Competition refer to in IAC Networks?</summary>
Competition is the tendency for units connected by negative weights to turn each other off. A unit that begins with a small advantage eventually "wins" the competition.
</details>

<details>
<summary>22. Define Resonance in IAC Networks.</summary>
Resonance is the tendency for units connected by positive weights to make each other active and keep each other active in the face of external competition.
</details>

<details>
<summary>23. What is the Blocking and Hysteresis phenomenon in IAC Networks?</summary>
Blocking and Hysteresis refer to the ability of one active unit to stop a unit to which it is connected with a negative weight from becoming active.
</details>

<details>
<summary>24. What is Oscillation in the context of IAC Networks?</summary>
Oscillation is the ability of some networks to turn on and off on consecutive timesteps and never settle to a stable point.
</details>

<details>
<summary>25. How do Boundaries function in IAC Networks?</summary>
Boundaries refer to the tendency for a unit to remain between the max and min values.
</details>


# Characteristics of Neural Processing

<details>
<summary>1. What is content addressability?</summary>
Content addressability refers to the ability to access memories given any of the components of the fact or episode.
</details>


<details>
<summary>2. What is the significance of robustness to noise in the IAC network?</summary>
Robustness to noise implies the ability of the IAC network to provide a best guess of the information to be retrieved, even when the information is incomplete or incorrect. This is possible due to the redundancy in its structure, allowing correct features to override incorrect activation values.
</details>

<details>
<summary>3. How does a Von Neumann architecture store data, and how is it different from human memory?</summary>

In a Von Neumann architecture, data is stored at specific locations or addresses in the computer's memory. To retrieve that data, its unique address must be known. This is in contrast to human memory, which seems capable of locating records (or memories) based on any of the information stored in that record.
</details>


<details>
<summary>4. What is meant by generalization in the context of neural networks?</summary>

Generalization refers to the ability to collapse over a set of instances to establish a general trend. The IAC network can accomplish spontaneous generalization by activating a property and cycling, and the resulting pattern of activation represents the sorts of features most commonly associated with that property.
</details>


<details>
<summary>5. How is the IAC network useful in situations of extreme noise?</summary>

The IAC network uses its structural redundancy to make a best guess of the information to be retrieved. In situations of extreme noise, such as speech recognition where the information might be incomplete or incorrect, provided there are enough correct features, the incorrect activation values will be overridden by the network.
</details>


<details>
<summary>6. How do people typically determine if Americans are more extroverted than Australians, in the absence of studies?</summary>

People might typically collapse across the set of Americans and Australians they know and extract some form of central tendency measure on the extrovert/introvert dimension. This involves a complex computation, which people routinely perform.
</details>


<details>
<summary>7. What is the role of default assignment in the human memory system?</summary>

Default assignment refers to the human memory system's extensive use of plausible defaults. It involves the ability to assign plausible default values if a given fact is not in memory. People can often have difficulty distinguishing actual memories from those that have been reconstructed from other related information.
</details>


<details>
<summary>8. How is the provision of plausible defaults in the IAC network related to generalization?</summary>

In the IAC network, the provision of plausible defaults is closely related to generalization. Features that are not presented are filled in with the most likely value, based on the other instances that the network "knows" about.
</details>


<details>
<summary>9. Why is content addressability significant in neural networks?</summary>

Content addressability is significant because it allows neural networks to retrieve memories or records based on any component of the stored information, not just a specific address or location. This mirrors human memory's capability of recalling memories based on any fragment of the information.
</details>


<details>
<summary>10. How does the IAC network handle situations where certain features are not presented?</summary>

In the IAC network, when certain features are not presented, they are filled in with the most likely value given the existing information. This value is based on the other instances that the network is familiar with, effectively using plausible defaults.
</details>


# Context Effect
<details>
<summary>1. What is the "word superiority effect" in the context of letter perception?</summary>
The word superiority effect is the advantage found for the perception of a letter when it occurs in a word context compared to when it occurs in a non-word context, or by itself.
</details>

<details>
<summary>2. How might subjects perceive the non-word "FOYEVER"?</summary>
A related finding in letter perception is the misperception of letters to transform a non-word into a word. For instance, subjects might read the letters of "FOYEVER" as "FOREVER".
</details>

<details>
<summary>3. In what way does word context impact the perception of single letters?</summary>
Reicher (1969) demonstrated that word context improves the perception of single letters independent of word-level guessing. For example, subjects were better at identifying the letter "E" in a word context like "READ" than when it was presented in a non-pronounceable non-word or by itself.
</details>

<details>
<summary>4. What are the core assumptions of the IA Model of Letter Perception?</summary>
The assumptions include: Perception is a multilevel system; there are three levels of representation - feature, letter, and word; more abstract levels are accessed via intermediate levels; and processing combines both bottom-up and top-down information.
</details>

<details>
<summary>5. How is the letter "A" represented in the IA Model of Letter Perception?</summary>
The letter "A" is represented as 11111010100000.
</details>

<details>
<summary>6. What role do feature-to-letter weights play in the IA Model?</summary>
Feature units have excitatory connections to all of the letter units in the same spatial position that have those features and inhibitory weights to those that do not have those features. These weights represent the bottom-up knowledge of the network.
</details>

<details>
<summary>7. How do letter-to-word weights function in the IA Model?</summary>
Each letter unit in a given position has excitatory connections to the word units that have that letter in that position, and inhibitory connections to all of the word units that do not have that letter in that position. These weights also embody the bottom-up knowledge of the network.
</details>

<details>
<summary>8. What is the significance of word-to-letter weights in the IA Model?</summary>
Each word unit has excitatory connections to all of the letter units which compose that word. These weights represent the top-down knowledge of the network.
</details>

<details>
<summary>9. How do within-level weights operate in the IA Model?</summary>
All of the word units are mutually inhibitory, meaning each word unit has negative connections to every other word unit. This allows for simultaneous consideration of multiple hypotheses.
</details>

<details>
<summary>10. Can the IA Model account for letters being misperceived to complete a word?</summary>
Yes, one of the questions posed about the IA Model of Letter Perception is whether it can account for the finding that letters are sometimes misperceived so as to complete a word.
</details>


# Tutorial Material

<details>
<summary>1. What does the IAC network embody?</summary>
It embodies many of the properties that make neural networks useful information processing models including content addressability, robustness in the face of noise, generalisation across exemplars and the ability to provide plausible default values for unknown variables.
</details>

<details>
<summary>2. What does each unit in an IAC network represent?</summary>
Each unit represents some micro-hypothesis or feature.
</details>

<details>
<summary>3. How do units within each competitive pool in the IAC network relate to each other?</summary>
The units within each competitive pool are mutually exclusive features and are interconnected with negative weights.
</details>

<details>
<summary>4. What role do positive weights play between the pools in the IAC network?</summary>
Between the pools, positive weights indicate features or micro-hypotheses which are consistent.
</details>

<details>
<summary>5. How do neural networks differ from standard computers based on the Von Neumann architecture?</summary>
Neural networks process information in a very different way: they are highly parallel and continuous in nature, whereas Von Neumann machines rely on discrete sequential processing.
</details>

<details>
<summary>6. What are the four properties of neural networks that are demonstrated in this lecture?</summary>
Content addressability, robustness to noise, generalization, and default assignment.
</details>

<details>
<summary>7. How is data stored in a Von Neumann architecture?</summary>
In a Von Neumann architecture, data is stored at specific locations or addresses in the computer's memory.
</details>

<details>
<summary>8. How does human memory retrieval differ from computer databases?</summary>
In human memory, retrieval from the content of a memory is automatic, making human memory fundamentally content addressable.
</details>

<details>
<summary>9. How does the discrete nature of Von Neumann architectures benefit data retention?</summary>
It allows them to retain information completely faithfully when subjected to small amounts of noise.
</details>

<details>
<summary>10. How do neural networks manage erroneous information?</summary>
Neural networks use redundancy in their structure to provide a best guess of the information to be retrieved.
</details>

<details>
<summary>11. What is an example of spontaneous generalization that people commonly perform?</summary>
Collapsing over a set of instances to establish a general trend, such as determining if Americans are more extroverted than Australians based on personal experiences.
</details>

<details>
<summary>12. How does the IAC network achieve spontaneous generalisation?</summary>
By activating a property and cycling.
</details>

<details>
<summary>13. What is the significance of the human memory system using plausible defaults?</summary>
People can have difficulty distinguishing actual memories from those that have been reconstructed from other related information.
</details>

<details>
<summary>14. How does the IAC network provide plausible default values for unknown information?</summary>
Items which are similar to the target item are used to extrapolate what the missing information should be.
</details>

<details>
<summary>15. In terms of the IAC network, how are plausible defaults related to generalisation?</summary>
The provision of plausible defaults is closely related to generalisation.
</details>

<details>
<summary>16. Who developed the IAC network model?</summary>
McClelland 1981; McClelland & Rumelhart 1981; Rumelhart & McClelland 1982.
</details>

<details>
<summary>17. How is activation propagated in the IAC network?</summary>
When the network is cycled, units connected by positive weights to active units become more active, while units connected by negative weights to active units are inhibited.
</details>

<details>
<summary>18. How are connections generally characterized in the IAC network?</summary>
The connections are, in general, bidirectional making the network interactive.
</details>

<details>
<summary>19. What does it mean for human memory to be fundamentally content addressable?</summary>
It means that humans can be reminded of facts and episodes from often quite obscure cues which are not unique when taken in isolation.
</details>

<details>
<summary>20. Why is the discrete nature of Von Neumann architectures important for applications like banking?</summary>
Because it ensures that the exact balance of an account is retained, rather than an approximation or best guess.
</details>
