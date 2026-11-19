# REPORT.md - Individual Assignment

Keep this concise and specific to your implementation.

## 1. Initial analysis

- How are locations and connections represented in the baseline
- Answer: Locations are represented as a ID, Name, Position and a type. For an example > "734, Stockholm, WorldPosition, City". 
Connections are represented as "FromLocationId, ToLocationId and TravelCost". Both classes have constructors. 
WorldData then takes the data from both Locations and Connectins, copies the collections from the lists and then copies it into arrays. 
Which is then passed through the WorldData Constructor. The WorldQueries searches through the stored data in WorldData. 

"FindLocationById" Goes through the whole world.locations.count one by one with ++i, untill it finds the right one and returns. 
"FindoutGoingConnections" iterates through the connections array to find all connections orignating from a specific location.

- Which operations appear frequent?
- Answer:

- Which operation(s) do you predict may scale poorly?
- Answer: And this way of doing things when searching throughout a large list is inefficient due to how much actuall computing power and time is wasted. 
Which both in hindsight can be negiable, but only negiable in small scale sitiuations.
When working with bigger databases this quickly builds up and makes everything worse fast.

Example: Imagine you have 2,500 locations and then you have to preform 5000 searches. That is 2500x5000 and is then 12,500,000 searches.

- What will you investigate first?
- Answer:

## 2. Data representation

Describe important changes/retained choices, operations affected, and time/memory trade-offs.

## 3. Algorithms and adaptation

Explain your route finder at a useful high level and how the travel-budget query adapts the same ideas.

## 4. Complexity

| Operation | Your representation/algorithm | Complexity | Short explanation |
| --- | --- | --- | --- |
| Find location by ID | | | |
| Get outgoing connections | | | |
| Priority queue enqueue | | | |
| Priority queue dequeue-min | | | |
| Route finding | | | |

## 5. Correctness and testing

Important tests/edge cases and what they demonstrate.

## 6. Performance investigation

Record reproducible before/after measurements for loading/preparation, repeated runtime work, and relevant allocation behavior. Explain what changed and why.

## 7. Development reflection

Describe one bug, wrong assumption, failed approach, or surprising result and how you investigated it.

## 8. Tools and AI assistance

Briefly describe relevant assistance, if any.

## 9. VG extension

Only if attempting VG: heuristic, traversal constraints, correctness, and Dijkstra/A* comparison.
