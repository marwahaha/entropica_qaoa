# Renaming Suggestions
 - QAOAParameter classes:
   [JL] Currently we do e.g.
    `from qaoa.parameters import AlternatingOperatorsQAOAParameters` which sounds very redundant if your read it out loud. Also the names are very long... Also some of the names (`General` and `AlternatingOperators` e.g.) are not very descriptive. Any suggestions for better names, for these? Drop the `*QAOAParameterers` in the names altogether? Shorten `*QAOAParameters` to `*Params`?

 - `hamiltonian_list_expectation_value`:
   [JL] -> `measurement_expectation` is shorter and (arguably) a bit more concise

 - `hamiltonian_expectation_value`:
   [JL] -> `measurement_expectation_z_base` should have the same name as above, with sth indicating, that this function is limited to diagonal hamiltonians

 - `create_random_hamiltonian`, `create_...`:
   [JL] Drop the `create` part in most of those? It is kind of obvious, that these functions will return you e.g. a random hamiltonian. I guess this applies to all function names that start with a somewhat redundant verb like `create` or `get`, where the rest of the name already tells you what will be returned.

# All top level names
Here a list of all the top-level(!) names in our packages sorted by length.
If someone knows how to recursively get _all_ names defined by us, feel free to update this list 

['hamiltonian_list_expectation_value',
 'AlternatingOperatorsQAOAParameters',
 'AdiabaticTimestepsQAOAParameters',
 'hamiltonian_expectation_value',
 'address_qubits_hamiltonian',
 'create_gaussian_2Dclusters',
 'create_random_hamiltonian',
 'PrepareAndMeasureOnWFSim',
 'create_circular_clusters',
 'prepare_sweep_parameters',
 'append_measure_register',
 'commuting_decomposition',
 'measurement_base_change',
 'QAOACostFunctionOnWFSim',
 'PrepareAndMeasureOnQVM',
 'AbstractQAOAParameters',
 'hamiltonian_from_edges',
 'WavefunctionSimulator',
 'GeneralQAOAParameters',
 'QAOACostFunctionOnQVM',
 'FourierQAOAParameters',
 'QAOAParameterIterator',
 'create_networkx_graph',
 'AbstractCostFunction',
 'make_qaoa_memory_map',
 'prepare_qaoa_ansatz',
 'distances_dataset',
 'QubitPlaceholder',
 'QuantumComputer',
 'scipy_optimizer',
 'MemoryReference',
 'address_qubits']