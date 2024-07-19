# Round-Table-Seating-Arrangement-Search-and-Heuristic

In this project, the Round Table Seating arrangemnet is approached diffrently formulated as a search problem. The approchaes are ucs, greedy and A* searches. Then a comparison is made between them. Throughout this report, the theory, implemnattions, discussion and conclusion are presented. It is required that rach person should be seated next to their neighbors on the left and right to facilitate conversation. It also should form a closed loop, as it is a round table.

## Algorthims Comparision

|Algorithm|Path|Minium Cost|CPU Times|Wall time|Time complexity|Completeness|Optimality|
|---|---|---|---|---|---|----|---|
|Uniform Cost Search|['Khalid', 'Samir', 'Kamal', 'Ibrahim', 'Hani', 'Salem', 'Fuad', 'Ahmed', 'Hakam', 'Ayman']|15394.0|14.1 s|17.3 s|O(b^(1 + C/min)|Complete|Optimal|
|Greedy search|['Khalid', 'Samir', 'Ibrahim', 'Kamal', 'Ayman', 'Ahmed', 'Fuad', 'Salem', 'Hani', 'Hakam']|23958.0|0 ns|995 µs|O(b^(1 + C/min)|Not complete|Not optimal|
|A* Search|Was not able to find a path |-|0 ns|2.07 ms|O(b^(1 + C/min)|Complete|Optimal|

> It is noticed that both Uniform Cost Search and Greedy serach have succeeded to find a path of a round table arrangement, howevere A* serach fails to do so. To start the evaluation between UCS and Greedy multi factors were considered: such as finding the best seating arrangement based on the conflict minimization objective (minimum cost), and (CPU time, wall time). In this case we have obtained a tradeoff, that is between the conflict minimization objective and the times. Because UCS had the lowest minimum cost 15394 and greedy has higher 23958 but in terms of time greedy was much faster with (0 CPU time and 995 µs) in comparision to USC needed more time with seconds (14.1 s CPU times) and (17.3 s for wall time).
> So the strengths of UCS was in reacheing the conflict minimization objective while it's weaknesses is related to the time consuming it takes longes as mentioned earlier. While greedy finds a good solution but it fails to reach the optimal since the minumm cost is much heigher than that the UCS finds. On the other hand, A* faild to find a solution, that could be due to the reason of the heuristic funct

## Conclusion
In conclusion, the objectives are met where three algorithms were implemnted to find the optimal round arrangement. The implemnations were called and evaluated mainly based on the minimum cost that they had but also considering other features too such as CPU time, time compelxity and completenss. While UCS was able to find the optimal solution in less cost than the greedy one (which is like in theory), Greedy search was faster in terms of both (CPU time) and (Wall time). Finally, the A star implemnatiions faild to find a solution and that might be due the heuristic function not being addmissable.

So the final seating arrangemnet was chosen to be the one that UCS obtained, which is the minumum conflict between seats. Folwoing is it's visulization:
<div align="center" >
<img src="https://github.com/sondosaabed/Round-Table-Seating-Arrangement/assets/65151701/48d46a7e-43d8-441d-9159-901aea7c3cd9" height="300">
</div>
