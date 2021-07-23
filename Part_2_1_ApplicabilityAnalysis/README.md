# :mortar_board: AUTOMATION SERVICE CHOREOGRAPHY

[:rewind:back](../README.md)

Editing Status: :construction: (under construction)

Last Modification: 09.05.2021

---

## :two: Applicability analysis of association mechanisms in automation based on presented adaptability use cases






Adaptability refers to structural changes of the production system. Structural changes are preceded by changings of the system in terms of design and automation. From a design point of view, a modular production
system can be separated into four different physical levels:

The use cases in Figure 1 and Figure 2 to adapt the PEA by
changing a COMP or changing a FEA, should be preferably
solved by decentral orchestration. The COMP respectively the
FEA are orchestrated by the PEA. For plant automation (see
Figure 4), a central orchestration is the best solution due
to the amount of services and the complexity. Both types
of orchestration have a centrally located orchestrating node
that is responsible for execution and interconnection of the
automation functions with respect to the three logic levels.
The use case in Figure 3 pointed out, that with regard to stricter
latency requirements a choreography-based mechanism should
preferably be used. An orchestration always has higher latency
times due to the broker-like communication and interaction
structure. This leads to disadvantages regarding regulatory
and interlocking logic associations. A mechanism following
the principles of choreographies results in a more interactive
association to define the collaboration between each of the
involved automation services. This leads to smaller latency
times regarding regulatory and interlocking logic and enables
a wider range of applications.
As published in [8], choreography is a rather unknown and
unexplored approach compared to orchestration in the context
of industrial automation systems. For this reason, this paper
presents a first concept in which the principles of a choreography
is investigated and implemented according to determined
requirements for industrial automation.

